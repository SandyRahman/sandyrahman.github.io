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

Berikut cara menggunakan command netstat :

1. Melihat koneksi ip/hostname dan port dalam satu server.
```sh
$ netstat -tlp | grep 9042
```
```sh
$ netstat -tlp | grep APPAPISIT01
```

2. Melihat Domain dan layanan yang sedang diakses.
```sh
$ netstat
```

3. Melihat IP dan Port yang sedang diakses.
```sh
$ netstat -n
```

4. Melihat nama program /aplikasi yang mengakses jaringan.
```sh
$ netstat -b
```

5. Melihat statistik jaringan.
```sh
$ netstat -s
```