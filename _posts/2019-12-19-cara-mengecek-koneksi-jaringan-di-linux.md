---
published: false
layout: post
excerpt: Fungsi ping di command line
tag: Linux
title: Cara Mengecek koneksi Jaringan di Linux
raw_title: true
---
Perintah **ping** adalah perintah yang paling sering dipakai dalam menganalisa permasalahan di jaringan. Kegunaan utama dari **Ping** adalah mengecek apakah ip/domain tertentu dalam kondisi hidup atau tidak. Ping sendiri mempunyai banyak parameter dan manfaat yang jarang di gunakan.

Berikut dibawah ini mengoptimalkan perintah Ping :

### 1.Memeriksa apakah interface lokal sudah aktif dan berjalan
```sh
$ ping 0
```
### 2. Memeriksa apakah interface ekternal sudah aktif dan berjalan
```sh
$ ping google.com
```
### 3. Kirim paket N dan berhenti
Kirim paket N yang ditentukan dengan opsi -c dan kemudian ping akan berhenti dengan sendirinya. Dengan cara ini perintah ping dapat keluar secara otomatis tanpa menekan CTRL + C untuk keluar.
```sh
$ ping -c 5 0
```
atau
```sh
$ ping -c 5 google.com
```
### 4. Tampilkan version ping
```sh
$ ping -V
```
### 5. Mencatat dan menampilkan bagaimana rute ECHO_REQUEST dikirim dan ECHO_REPLY diterima
```sh
$ ping -R ip/host
```
