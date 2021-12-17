# FFUF Report

  Command line : `ffuf -u http://10.10.10.233/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common.md`
  Time: 2021-06-26T16:02:56-04:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://10.10.10.233/ |  | 1 | 200 | 7440 | 808 | 157 | text/html; charset=utf-8 |  |
  | .hta | http://10.10.10.233/.hta |  | 11 | 403 | 206 | 15 | 9 | text/html; charset=iso-8859-1 |  |
  | .htpasswd | http://10.10.10.233/.htpasswd |  | 13 | 403 | 211 | 15 | 9 | text/html; charset=iso-8859-1 |  |
  | .htaccess | http://10.10.10.233/.htaccess |  | 12 | 403 | 211 | 15 | 9 | text/html; charset=iso-8859-1 |  |
  | cgi-bin/ | http://10.10.10.233/cgi-bin/ |  | 820 | 403 | 210 | 15 | 9 | text/html; charset=iso-8859-1 |  |
  | includes | http://10.10.10.233/includes | http://10.10.10.233/includes/ | 2013 | 301 | 237 | 14 | 8 | text/html; charset=iso-8859-1 |  |
  | index.php | http://10.10.10.233/index.php |  | 2021 | 200 | 7440 | 808 | 157 | text/html; charset=utf-8 |  |
  | misc | http://10.10.10.233/misc | http://10.10.10.233/misc/ | 2535 | 301 | 233 | 14 | 8 | text/html; charset=iso-8859-1 |  |
  | modules | http://10.10.10.233/modules | http://10.10.10.233/modules/ | 2567 | 301 | 236 | 14 | 8 | text/html; charset=iso-8859-1 |  |
  | profiles | http://10.10.10.233/profiles | http://10.10.10.233/profiles/ | 3161 | 301 | 237 | 14 | 8 | text/html; charset=iso-8859-1 |  |
  | robots.txt | http://10.10.10.233/robots.txt |  | 3436 | 200 | 2189 | 158 | 91 | text/plain; charset=UTF-8 |  |
  | scripts | http://10.10.10.233/scripts | http://10.10.10.233/scripts/ | 3520 | 301 | 236 | 14 | 8 | text/html; charset=iso-8859-1 |  |
  | sites | http://10.10.10.233/sites | http://10.10.10.233/sites/ | 3699 | 301 | 234 | 14 | 8 | text/html; charset=iso-8859-1 |  |
  | themes | http://10.10.10.233/themes | http://10.10.10.233/themes/ | 4037 | 301 | 235 | 14 | 8 | text/html; charset=iso-8859-1 |  |
  | web.config | http://10.10.10.233/web.config |  | 4365 | 200 | 2200 | 416 | 47 | text/xml |  |
  | xmlrpc.php | http://10.10.10.233/xmlrpc.php |  | 4568 | 200 | 42 | 6 | 1 | text/html; charset=UTF-8 |  |
  