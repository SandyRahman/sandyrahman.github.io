---
published: false
layout: post
date: 2019-12-05T00:00:00.000Z
excerpt: Generate ssl https
tag:
  - Linux
comments: true
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```