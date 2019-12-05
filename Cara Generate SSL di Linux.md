---
published: true
layout: post
excerpt: Generate SSL https
tag:
  - Linux
comments: true
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```
