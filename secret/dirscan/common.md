# FFUF Report

  Command line : `ffuf -u http://10.10.11.120/api/FUZZ -w /usr/share/wordlists/dirb/common.txt -of md -o dirscan/common.md -fs 93`
  Time: 2021-12-19T10:44:26-05:00

  | FUZZ | URL | Redirectlocation | Position | Status Code | Content Length | Content Words | Content Lines | Content Type | ResultFile |
  | :- | :-- | :--------------- | :---- | :------- | :---------- | :------------- | :------------ | :--------- | :----------- |
  | logs | http://10.10.11.120/api/logs |  | 2363 | 401 | 13 | 2 | 1 | text/html; charset=utf-8 |  |
  | Logs | http://10.10.11.120/api/Logs |  | 2364 | 401 | 13 | 2 | 1 | text/html; charset=utf-8 |  |
  | priv | http://10.10.11.120/api/priv |  | 3110 | 401 | 13 | 2 | 1 | text/html; charset=utf-8 |  |
  