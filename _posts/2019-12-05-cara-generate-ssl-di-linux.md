---
published: true
layout: post
excerpt: Generate SSL HTTPS
tag: Linux
comments: true
title: Cara Generate SSL di Linux
raw_title: true
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```
