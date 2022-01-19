# FFUF Report

  Command line : `ffuf -u http://driver.htb/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -e php -o dirscan/common_with_php.md`
  Time: 2021-12-30T09:19:57-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://driver.htb/ |  | 1 | 401 | 20 | 2 | 2 | text/html; charset=UTF-8 |  |
  | Images | http://driver.htb/Images | http://driver.htb/Images/ | 3983 | 301 | 148 | 9 | 2 | text/html; charset=UTF-8 |  |
  | images | http://driver.htb/images | http://driver.htb/images/ | 3981 | 301 | 148 | 9 | 2 | text/html; charset=UTF-8 |  |
  | index.php | http://driver.htb/index.php |  | 4041 | 401 | 20 | 2 | 2 | text/html; charset=UTF-8 |  |
  