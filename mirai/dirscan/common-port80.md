# FFUF Report

  Command line : `ffuf -u http://10.10.10.48/FUZZ -w /usr/share/wordlists/dirb/common.txt -fc 404 -of md -o dirscan/common-port80.md`
  Time: 2020-11-28T07:59:02-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- |
  | admin | http://10.10.10.48/admin | http://10.10.10.48/admin/ | 286 | 301 | 0 | 1 | 1 |  |
  | swfobject.js | http://10.10.10.48/swfobject.js |  | 3928 | 200 | 61 | 10 | 2 |  |
  