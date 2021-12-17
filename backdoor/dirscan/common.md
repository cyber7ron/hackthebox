# FFUF Report

  Command line : `ffuf -u http://10.10.11.125/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common.md`
  Time: 2021-12-06T14:14:41-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  | .hta | http://10.10.11.125/.hta |  | 11 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htaccess | http://10.10.11.125/.htaccess |  | 12 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htpasswd | http://10.10.11.125/.htpasswd |  | 13 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  |  | http://10.10.11.125/ |  | 1 | 200 | 63830 | 3830 | 330 | text/html; charset=UTF-8 |  |
  | index.php | http://10.10.11.125/index.php | http://10.10.11.125/ | 2021 | 301 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | server-status | http://10.10.11.125/server-status |  | 3588 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | wp-admin | http://10.10.11.125/wp-admin | http://10.10.11.125/wp-admin/ | 4485 | 301 | 315 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | wp-content | http://10.10.11.125/wp-content | http://10.10.11.125/wp-content/ | 4495 | 301 | 317 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | wp-includes | http://10.10.11.125/wp-includes | http://10.10.11.125/wp-includes/ | 4501 | 301 | 318 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | xmlrpc.php | http://10.10.11.125/xmlrpc.php |  | 4568 | 405 | 42 | 6 | 1 | text/plain;charset=UTF-8 |  |
  