# FFUF Report

  Command line : `ffuf -u http://10.10.11.104/FUZZ.php -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common_php.md`
  Time: 2021-11-22T12:47:18-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://10.10.11.104/.php |  | 1 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .hta | http://10.10.11.104/.hta.php |  | 11 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | accounts | http://10.10.11.104/accounts.php | login.php | 252 | 302 | 3994 | 1096 | 94 | text/html; charset=UTF-8 |  |
  | .htaccess | http://10.10.11.104/.htaccess.php |  | 12 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | .htpasswd | http://10.10.11.104/.htpasswd.php |  | 13 | 403 | 277 | 20 | 10 | text/html; charset=iso-8859-1 |  |
  | config | http://10.10.11.104/config.php |  | 994 | 200 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | download | http://10.10.11.104/download.php | login.php | 1340 | 302 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | files | http://10.10.11.104/files.php | login.php | 1605 | 302 | 4914 | 1531 | 113 | text/html; charset=UTF-8 |  |
  | footer | http://10.10.11.104/footer.php |  | 1652 | 200 | 217 | 10 | 6 | text/html; charset=UTF-8 |  |
  | header | http://10.10.11.104/header.php |  | 1877 | 200 | 980 | 183 | 21 | text/html; charset=UTF-8 |  |
  | index | http://10.10.11.104/index.php | login.php | 2017 | 302 | 2801 | 737 | 72 | text/html; charset=UTF-8 |  |
  | login | http://10.10.11.104/login.php |  | 2347 | 200 | 2224 | 486 | 54 | text/html; charset=UTF-8 |  |
  | logout | http://10.10.11.104/logout.php | login.php | 2362 | 302 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | logs | http://10.10.11.104/logs.php | login.php | 2363 | 302 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | nav | http://10.10.11.104/nav.php |  | 2646 | 200 | 1248 | 462 | 32 | text/html; charset=UTF-8 |  |
  | status | http://10.10.11.104/status.php | login.php | 3850 | 302 | 2968 | 749 | 75 | text/html; charset=UTF-8 |  |
  