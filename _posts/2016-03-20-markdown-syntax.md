---
layout: post
title: '    _posts/2019-12-05-Cara Generate SSL di Linux.md'
date: {}
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