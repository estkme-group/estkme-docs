+++
title = "Mode ISD-R"
date =  2023-12-17T21:54:23+08:00
weight = 6
+++

## Mengonfigurasi mode operasi domain ISD-R

ISD-R adalah antarmuka utama antara LPA dan eUICC, pengelolaan file konfigurasi (termasuk mengunduh, mengalihkan, menghapus, mengganti nama, dll.), dan akuisisi informasi eUICC, semuanya didasarkan pada domain manajemen ini.

{{% notice style="note" title="Catatan tambahan" %}}
1. Anda bebas mencoba fungsi ini.
2. Hasil operasi dapat dikembalikan, atau setidaknya ada cara untuk mengembalikan ke kondisi sebelumnya.
3. Mode operasi ISD-R yang tidak diinginkan dapat menyebabkan aplikasi LPA tidak dapat mengelola eUICC. Anda harus memastikan bahwa Anda memiliki akses normal ke STK atau memiliki pembaca PC/SC.
{{% /notice %}}

"Menu Pilihan ISD-R" memiliki awalan karakter "< >" atau "<\*>", di mana awalan "<\*>" menunjukkan konfigurasi yang sedang aktif.  

> Mode ISD-R yang tersedia saat ini
1. _Shared_: Mode _default_, domain ISD-R dapat diakses secara bersama dan semua permintaan akses diizinkan.
2. _Exclusive_: Mode akses eksklusif, Anda harus menunggu operasi saat ini selesai sebelum menerima permintaan akses lainnya.
3. Disabled: Mode dinonaktifkan, di mana domain ISD-R tidak dapat diakses oleh perangkat akhir.

{{% notice style="warning" title="Pemberitahuan" %}}
Jika Anda mengatur "[mode ATR](./atr-mode)" diatur ke "eUICC" dan pada saat yang sama "Nonaktifkan ISD-R", hal ini dapat menyebabkan beberapa terminal menampilkan pesan "_SmartCard_ rusak"
{{% /notice %}}
