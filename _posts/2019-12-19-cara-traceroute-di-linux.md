---
published: true
layout: post
excerpt: Traceroute menggunkaan command line di server linux
tag: Linux
title: Cara Traceroute di Linux
raw_title: true
---
**Traceroute(tracert)** adalah perintah untuk menunjukkan rute yang dilewati paket untuk mencapai tujuan. Ini dilakukan dengan mengirim pesan Internet Control Message Protocol (ICMP) Echo Request Ke tujuan dengan nilai Time to Live yang semakin meningkat. Rute yang ditampilkan adalah daftar interface router (yang paling dekat dengan host) yang terdapat pada jalur antara host dan tujuan.

Berikut dibawah ini :
```sh
$ traceroute ip/host
```
