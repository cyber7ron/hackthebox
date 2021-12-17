# FFUF Report

  Command line : `ffuf -u http://10.10.11.104/FUZZ -w /usr/share/wordlists/dirb/big.txt -e php -of md -o dirscan/big_php.md`
  Time: 2021-11-22T13:17:16-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  | .htpasswdphp | http://10.10.11.104/.htpasswdphp |  | 32 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htpasswd | http://10.10.11.104/.htpasswd |  | 31 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htaccessphp | http://10.10.11.104/.htaccessphp |  | 30 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htaccess | http://10.10.11.104/.htaccess |  | 29 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | css | http://10.10.11.104/css | http://10.10.11.104/css/ | 11033 | 301 | 310 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | favicon.ico | http://10.10.11.104/favicon.ico |  | 14853 | 200 | 15406 | 15 | 10 | image/vnd.microsoft.icon |  |
  | js | http://10.10.11.104/js | http://10.10.11.104/js/ | 20379 | 301 | 309 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | server-status | http://10.10.11.104/server-status |  | 32429 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  