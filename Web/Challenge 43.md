<H1>Challenge 43: Headache </H1>
<p> As the name suggest there is something inside the Header.</p>

1. So to find the flag, we need to send a get request and analyze the Header.

2. To get the request I used the Simple REST Client plugin on chrome.

3. I receive this respond to the request:
```
Flag: FLAG-*******
Pragma: no-cache
Date: Sun, 13 Dec 2015 21:21:39 GMT
Content-Encoding: gzip
Server: Apache
X-Powered-By: PHP/5.4.45-0+deb7u2
Vary: Accept-Encoding
Content-Type: text/html
Cache-Control: no-store, no-cache, must-revalidate, post-check=0, pre-check=0
Connection: Keep-Alive
Keep-Alive: timeout=5, max=100
Content-Length: 2156
Expires: Thu, 19 Nov 1981 08:52:00 GMT
```
4. There is the flag.
