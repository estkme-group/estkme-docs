+++
title = "ARA-M SHA-1"
date =  2023-12-17T21:48:31+08:00
weight = 1
+++

## Memberikan akses aplikasi

ARA-M digunakan sebagai atribut khusus _SmartCard_ untuk mengontrol aplikasi mana yang dapat mengakses antarmuka _SmartCard_ pada sistem operasi modern. ARA-M sudah digunakan secara luas dalam sistem operasi Android, yang mendukung OMAPI (_Open Mobile API_).  
_SmartCard_ menggunakan ARA-M untuk memberi tahu sistem operasi aplikasi pengembang mana yang dapat mengaksesnya dengan menggunakan nilai SHA-1 atau SHA-256 dari sertifikat pengembang.

{{% notice style="note" title="Tindakan Perhatian Ekstra" %}}
1. Anda bebas mencoba fungsi ini.
2. Hasil operasi dapat dikembalikan, atau setidaknya ada cara untuk mengembalikan ke kondisi sebelumnya.
3. Nilai ARA-M SHA-1 yang salah dapat menyebabkan aplikasi LPA (_Local Profile Assistant_) tidak dapat mengelola eUICC. Anda harus memastikan bahwa Anda memiliki akses normal ke STK (_SIM ToolKit_) atau memiliki pembaca PC/SC.
{{% /notice %}}

Mengetuk item menu ini akan menampilkan daftar 5 nilai ARA-M yang telah disimpan dalam kartu, atau semua angka nol jika belum pernah ditetapkan.

Ketuk nilai mana saja untuk masuk ke mode edit. Ada dua operasi dalam mode edit sebagai berikut:

1. Masukkan nilai SHA-1 yang diharapkan yang akan disimpan dalam kartu.
2. Masukkan nilai apa pun dan kirim, nilai yang dipilih sebelumnya akan dikosongkan menjadi nol.

{{% notice style="note" title="Catatan" %}}
Bila nilai ARA-M SHA-1 salah diubah dan menu STK (_SIM ToolKit_) tidak dapat diakses dengan benar, Anda perlu merujuk ke bagian "Pembaruan _Firmware_" untuk mengembalikan pengaturan ke kondisi pabrik. 
{{% /notice %}}

{{% notice style="tip" title="Tips" %}}
eSTK.me saat ini mendukung hingga 5 ARA-M yang berbeda. Ini berarti Anda dapat mengotorisasi aplikasi dari hingga 5 pengembang yang berbeda untuk manajemen kartu.
{{% /notice %}}

{{% expand title="Sebelum _firmware_ 1.2.3"%}}
{{% /expand %}}