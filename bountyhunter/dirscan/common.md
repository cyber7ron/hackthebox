# FFUF Report

  Command line : `ffuf -u http://10.10.11.100/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common.md`
  Time: 2021-10-28T10:52:40-04:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://10.10.11.100/ |  | 1 | 200 | 25169 | 10028 | 389 | text/html; charset=UTF-8 |  |
  | .htpasswd | http://10.10.11.100/.htpasswd |  | 13 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htaccess | http://10.10.11.100/.htaccess |  | 12 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .hta | http://10.10.11.100/.hta |  | 11 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | assets | http://10.10.11.100/assets | http://10.10.11.100/assets/ | 499 | 301 | 313 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | css | http://10.10.11.100/css | http://10.10.11.100/css/ | 1114 | 301 | 310 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | index.php | http://10.10.11.100/index.php |  | 2021 | 200 | 25169 | 10028 | 389 | text/html; charset=UTF-8 |  |
  | js | http://10.10.11.100/js | http://10.10.11.100/js/ | 2179 | 301 | 309 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | resources | http://10.10.11.100/resources | http://10.10.11.100/resources/ | 3404 | 301 | 316 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | server-status | http://10.10.11.100/server-status |  | 3588 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  