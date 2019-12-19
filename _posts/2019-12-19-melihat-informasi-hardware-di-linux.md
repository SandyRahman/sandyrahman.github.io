---
published: true
layout: post
excerpt: Command line melihat detail informasi hardware di server linux.
tag: Linux
title: Melihat Informasi Hardware di Linux
raw_title: true
---
Berikut dibawah ini :

### Melihat Prosesor
```sh
$ cat /proc/cpuinfo |grep "model name"
```
```sh
$ lscpu
```
### Melihat Ukuran Memori
```sh
$ cat /proc/meminfo |head -2
```
### Melihat partisi Hardisk
```sh
$ sudo cfdisk
```
### Melihat penggunaan hardisk
```sh
$ df -h
```
```sh
$ lsblk
```
### melihat periperal yang terinstall
```sh
$ lspci
```
