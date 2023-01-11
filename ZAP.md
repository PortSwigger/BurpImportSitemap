This documentation file pretends to explain how to export HTTP request captured using [ZAP Proxy](https://www.zaproxy.org).

Since the standard session files used by ZAP are binary and parsing them would require a reverse engineering process, we need to export the content in a different format.

The following steps are needed:

1. Open OWASP Zap with the HTTP requests you want to export.
2. Go to the "History" tab and select all the desired requests (usually all of them).
3. Go to menu "Report" and then "Export Messages to File..."
4. Choose folder and file name.

The resulting file should have the following format:

```
===1 ==========
GET https://whatever.com/foo/ HTTP/1.1
[REQUEST]


[RESPONSE]
===2 ==========
[...]
```

This file can be imported directly into burp-wstalker, as explained in [README.md](README.md).
