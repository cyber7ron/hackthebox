# FFUF Report

  Command line : `ffuf -u http://10.10.11.104/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common.md`
  Time: 2021-11-22T12:45:52-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://10.10.11.104/ | login.php | 1 | 302 | 2801 | 737 | 72 | text/html; charset=UTF-8 |  |
  | .htpasswd | http://10.10.11.104/.htpasswd |  | 13 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htaccess | http://10.10.11.104/.htaccess |  | 12 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .hta | http://10.10.11.104/.hta |  | 11 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | css | http://10.10.11.104/css | http://10.10.11.104/css/ | 1114 | 301 | 310 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | favicon.ico | http://10.10.11.104/favicon.ico |  | 1575 | 200 | 15406 | 15 | 10 | image/vnd.microsoft.icon |  |
  | index.php | http://10.10.11.104/index.php | login.php | 2021 | 302 | 2801 | 737 | 72 | text/html; charset=UTF-8 |  |
  | js | http://10.10.11.104/js | http://10.10.11.104/js/ | 2179 | 301 | 309 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | server-status | http://10.10.11.104/server-status |  | 3588 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  