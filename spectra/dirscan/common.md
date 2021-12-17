# FFUF Report

  Command line : `ffuf -u http://10.10.10.229/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common.md`
  Time: 2021-06-21T15:07:20-04:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  |  | http://10.10.10.229/ |  | 1 | 200 | 283 | 22 | 7 | text/html |  |
  | index.html | http://10.10.10.229/index.html |  | 2020 | 200 | 283 | 22 | 7 | text/html |  |
  | main | http://10.10.10.229/main | http://10.10.10.229/main/ | 2416 | 301 | 169 | 5 | 8 | text/html |  |
  | testing | http://10.10.10.229/testing | http://10.10.10.229/testing/ | 4020 | 301 | 169 | 5 | 8 | text/html |  |
  