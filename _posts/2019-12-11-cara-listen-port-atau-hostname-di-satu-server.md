---
published: true
layout: post
excerpt: Listen port/hostname di dalam server menggunakan netstat
tag: Linux
title: Cara Listen Port atau Hostname di Satu Server
raw_title: true
---
**Netstat** digunakan untuk monitoring jaringan dan informasi yang terkait dengan koneksi port, antara lain alamat IP yang terhubung, status koneksi dan aplikasi yang digunakan. Netstat digunakan untuk protocol **IPv4**, **ICMPv4**, **TCP over IPv4**, **UDP over IPv4**, **IPv6**, **ICMPv6**, **TCP over IPv6**, and **UDP over IPv6**.

Netstat bisa digunakan untuk melacak sumber paket yang didapat. Netstat juga bisa disebut sebagai port scanner.

Berikut cara menggunakannya :

* Jika Port
```sh
$ netstat -tlp | grep 9042
```

* Jika Hostname
```sh
$ netstat -tlp | grep APPAPISIT01
```
