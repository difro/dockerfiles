This is Dockerfile for http2 enabled build of curl (with nghttp2).

Usage
=====

```
$ docker run --rm difro/curl-h2 --http2 -s -D- -o/dev/null https://http2.akamai.com
HTTP/2.0 200
server:Apache
content-type:text/html
etag:"4d58eb3716b254a609bb752d564ad956:1432244356"
strict-transport-security:max-age=31536000 ; includeSubDomains
access-control-allow-origin:*
access-control-allow-methods:GET,HEAD,POST
access-control-allow-headers:*
access-control-allow-credentials:false
access-control-max-age:86400
protocol_negotiation:h2
myproto:h2-14
client_ip:111.91.137.46
client_real_ip:111.91.137.46
ghost_service_ip:23.67.53.95
ghost_ip:104.76.68.45
rtt:4
x-akamai-transformed:9 8490 0 pmb=mRUM,1
cache-control:max-age=43200
expires:Wed, 15 Jul 2015 20:41:06 GMT
date:Wed, 15 Jul 2015 08:41:06 GMT
```
