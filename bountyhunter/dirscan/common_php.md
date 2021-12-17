# FFUF Report

  Command line : `ffuf -u http://10.10.11.100/FUZZ.php -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common_php.md`
  Time: 2021-10-28T10:54:00-04:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://10.10.11.100/.php |  | 1 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htaccess | http://10.10.11.100/.htaccess.php |  | 12 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htpasswd | http://10.10.11.100/.htpasswd.php |  | 13 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .hta | http://10.10.11.100/.hta.php |  | 11 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | db | http://10.10.11.100/db.php |  | 1171 | 200 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | index | http://10.10.11.100/index.php |  | 2017 | 200 | 25169 | 10028 | 389 | text/html; charset=UTF-8 |  |
  | portal | http://10.10.11.100/portal.php |  | 3043 | 200 | 125 | 11 | 6 | text/html; charset=UTF-8 |  |
  