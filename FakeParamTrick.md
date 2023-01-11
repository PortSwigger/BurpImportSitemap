## Enable Fakeparam Trick 

![Load CSV](img/load.png "Logo Title Text 1")

There is a checkbox called "Enable Fakeparam Trick", which is disabled by default. When enabled, a new artificial parameter "wstalkerfakeparam" is added to each request. The reason to do this is because some time ago sitemap did not add several requests with the same URL, so adding a fake parameter with random value guaranteed that every request/response is sucessfully imported. This is no longer necessary in modern Burp versions, but it is kept just in case the extension is loaded in an old version.

![Fakeparam](img/fakeparam.png "Logo Title Text 1")