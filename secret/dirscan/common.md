# FFUF Report

  Command line : `ffuf -u http://10.10.11.120/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common.md`
  Time: 2021-12-12T15:48:36-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  | api | http://10.10.11.120/api |  | 428 | 200 | 93 | 12 | 1 | application/json; charset=utf-8 |  |
  | assets | http://10.10.11.120/assets | /assets/ | 499 | 301 | 179 | 7 | 11 | text/html; charset=UTF-8 |  |
  | docs | http://10.10.11.120/docs |  | 1319 | 200 | 20720 | 6752 | 487 | text/html; charset=utf-8 |  |
  | download | http://10.10.11.120/download | /download/ | 1340 | 301 | 183 | 7 | 11 | text/html; charset=UTF-8 |  |
  