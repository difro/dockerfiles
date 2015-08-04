This is Dockerfile for node [caniuse-cmd](https://www.npmjs.com/package/caniuse-cmd)

Usage
=====

```
$ docker run -t --rm difro/caniuse-cmd indexeddb
IndexedDB ✔ 59.46% ◒ 18.58% [W3C Candidate Recommendation]
  Method of storing data client-side, allows indexed database queries. #JSAPI

  IE ✘ 5.5+ ◒ 10+¹
  Edge ◒ ¹
  Firefox ✘ 2+ ◒ 4+ᵖ ✔ 10+ᵖ ✔ 16+
  Chrome ✘ 4+ ◒ 11+ᵖ ✔ 23+ᵖ ✔ 24+
  Safari ✘ 3.1+ ◒ 7.1+²
  Opera ✘ 9+ ✔ 15+

    ¹Partial support in IE 10 & 11 refers to a number of subfeatures [not being supported](http://codepen.io/cemerick/pen/Itymi).
    ²Partial support in iOS 8 refers to [seriously buggy behavior](http://www.raymondcamden.com/2014/9/25/IndexedDB-on-iOS-8--Broken-Bad).

$ docker run -t --rm difro/caniuse-cmd http2
HTTP/2 protocol ✔ 48.92% ◒ 7.6% [Other]
  Networking protocol for low-latency transport of content over the web. Originally started out from the SPDY protocol, now standardized as HTTP version 2. #Other

  IE ✘ 5.5+ ◒ 11¹
  Edge ✔
  Firefox ✘ 2+ ✔ 36+
  Chrome ✘ 4+ ✔ 41+
  Safari ✘
  Opera ✘ 9+ ✔ 28+

    ¹Partial support in IE11 refers to being limited to Windows 10.
  ⓘ  See also support for [the SPDY protocol](http://caniuse.com/#feat=spdy), precursor of HTTP2

```
