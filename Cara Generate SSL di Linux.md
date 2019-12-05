---
published: true
layout: post
excerpt: Generate SSL HTTPS
tag: Linux
comments: true
tittle: Cara Generate SSL di Linux
date: 2019-12-05T00:00:00.000Z
---
```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```

Untuk referensi lainnya bisa dilihat disini https://www.freecodecamp.org/news/openssl-command-cheatsheet-b441be1e8c4a/
