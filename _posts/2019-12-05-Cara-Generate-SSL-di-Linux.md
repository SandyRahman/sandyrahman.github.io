---
published: false
layout: post
excerpt: Generate SSL HTTPS
tag:
  - Linux
comments: true
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```
