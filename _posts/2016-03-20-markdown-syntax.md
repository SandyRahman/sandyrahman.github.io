---
layout: post
title: Cara Generate SSL di Linux
date: 2016-03-15T00:00:00.000Z
excerpt: >-
  Just about everything you'll need to style in the theme: headings, paragraphs,
  blockquotes, tables, code blocks, and more.
tag:
  - Linux
comments: true
published: true
---

```sh
$ openssl s_client -showcerts -servername hostname -connect hostname:port
```

