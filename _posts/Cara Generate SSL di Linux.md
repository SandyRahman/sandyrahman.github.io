---
published: true
layout: post
date: {}
excerpt: Generate SSL HTTPS
tag: Linux
comments: true
title: Cara Generate SSL di Linux
raw_title: true
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```