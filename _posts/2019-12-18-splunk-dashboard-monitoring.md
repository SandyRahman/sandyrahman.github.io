---
published: true
layout: post
excerpt: Splunk Search Processing language
tag: Splunk
title: Splunk Dashbord Monitoring
raw_title: true
---
**Splunk** adalah sebuah platform untuk memonitoring atau merekam semua data log dari server dan kemudian dilakukan proses indexing.

Platform monitoring selain **Splunk** yaitu **Kibana**, **Grafana**, dan lainnya.

**Splunk Search Processing Language (SPL)** adalah sebuah query yang berisi banyak perintah untuk menampilkan atau memfilter kumpulan data log dari server secara spesifik agar bisa di lakukan monitoring dan analisis.

Beberapa referensi splunk bisa dilihat dibawah ini :
1. <a href="https://www.tutorialspoint.com/splunk/index.htm" 				
     title="tutorialsplunk">Tutorial Splunk</a>

Berikut dibawah ini contoh kumpulan SPL di Splunk yang saya buat :
>	spath	--> commends untuk mengambil sebuah data, berdasarkan nama field yang ada di dalam index dan data outpunya bisa kita tampilkan di sebuah table.
	search	--> commends untuk mencari sebuah data.
	rename	--> commends untuk mengubah sebuah field.
	table	--> commends untuk membuat sebuah kolom didalam table.

```sh
index=apigateway
host="appapiprd0*.corp.bankbtpn.co.id" OR  host="appapidrc0*.corp.bankbtpn.co.id"
| spath output=path path=legs{0}.uri 
| spath output=serviceName path=legs{0}.serviceName 
| spath output=method path=legs{0}.method 
| spath output=code path=legs{0}.status 
| spath output=Operation path=legs{0}.operation 
| search path=* 
| search serviceName="*"
| search code="*" 
| search Operation="*" 
| rename correlationId as transaction-id
| table _time, serviceName ,method , path , Operation, transaction-id, code, duration
```
