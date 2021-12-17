# FFUF Report

  Command line : `ffuf -u http://spectra.htb/main/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o wp_common.md`
  Time: 2021-06-21T15:17:33-04:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://spectra.htb/main/ |  | 1 | 200 | 25940 | 1217 | 347 | text/html; charset=UTF-8 |  |
  | index.php | http://spectra.htb/main/index.php | http://spectra.htb/main/ | 2021 | 301 | 0 | 1 | 1 | text/html; charset=UTF-8 |  |
  | wp-admin | http://spectra.htb/main/wp-admin | http://spectra.htb/main/wp-admin/ | 4485 | 301 | 169 | 5 | 8 | text/html |  |
  | wp-includes | http://spectra.htb/main/wp-includes | http://spectra.htb/main/wp-includes/ | 4501 | 301 | 169 | 5 | 8 | text/html |  |
  | wp-content | http://spectra.htb/main/wp-content | http://spectra.htb/main/wp-content/ | 4495 | 301 | 169 | 5 | 8 | text/html |  |
  | xmlrpc.php | http://spectra.htb/main/xmlrpc.php |  | 4568 | 405 | 42 | 6 | 1 | text/plain;charset=UTF-8 |  |
  