---
published: false
layout: post
date: 2019-11-05T00:00:00.000Z
excerpt: Generate SSL HTTPS
tag: Linux
comments: true
title: Cara Generate SSL di Linux
raw_title: true
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```