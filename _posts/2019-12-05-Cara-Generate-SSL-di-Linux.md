---
published: true
layout: post
date: {}
excerpt: Generate ssl https
tag:
  - Linux
comments: true
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```
