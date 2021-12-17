# FFUF Report

  Command line : `ffuf -u http://10.10.11.125/FUZZ.php -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common_php.md`
  Time: 2021-12-06T14:16:24-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://10.10.11.125/.php |  | 1 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .hta | http://10.10.11.125/.hta.php |  | 11 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htaccess | http://10.10.11.125/.htaccess.php |  | 12 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htpasswd | http://10.10.11.125/.htpasswd.php |  | 13 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | index | http://10.10.11.125/index.php | http://10.10.11.125/ | 2017 | 301 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | wp-cron | http://10.10.11.125/wp-cron.php |  | 4496 | 200 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | wp-blog-header | http://10.10.11.125/wp-blog-header.php |  | 4489 | 200 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | wp-config | http://10.10.11.125/wp-config.php |  | 4493 | 200 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | wp-load | http://10.10.11.125/wp-load.php |  | 4503 | 200 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | wp-links-opml | http://10.10.11.125/wp-links-opml.php |  | 4502 | 200 | 223 | 12 | 12 | text/xml; charset=UTF-8 |  |
  | wp-login | http://10.10.11.125/wp-login.php |  | 4504 | 200 | 5674 | 282 | 99 | text/html; charset=UTF-8 |  |
  | wp-mail | http://10.10.11.125/wp-mail.php |  | 4505 | 403 | 2616 | 191 | 121 | text/html; charset=UTF-8 |  |
  | wp-trackback | http://10.10.11.125/wp-trackback.php |  | 4515 | 200 | 135 | 11 | 5 | text/xml; charset=UTF-8 |  |
  | wp-signup | http://10.10.11.125/wp-signup.php | http://10.10.11.125/wp-login.php?action=register | 4513 | 302 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | xmlrpc | http://10.10.11.125/xmlrpc.php |  | 4566 | 405 | 42 | 6 | 1 | text/plain;charset=UTF-8 |  |
  