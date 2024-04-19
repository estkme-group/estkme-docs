+++
title = "EID Virtual"
date =  2023-12-17T21:53:42+08:00
weight = 3
+++

## Mengonfigurasi nilai EID virtual

Fitur ini memungkinkan Perangkat Lunak Manajemen eUICC (LPA) untuk mengambil nilai yang ditentukan pengguna, bukan nomor seri yang secara permanen tersimpan di eSE.  

{{% notice style="tip" title="Pengoperasian yang andal" %}}
1. Anda bebas mencoba fungsi ini.
2. Hasil operasi dapat dikembalikan, atau setidaknya ada cara untuk mengembalikan ke kondisi sebelumnya.
3. EID khusus dapat membuat beberapa perangkat lunak manajemen menjadi tidak normal.
{{% /notice %}}

Item menu ini akan muncul ketika Anda mengkliknya:
1. Nilai EID Virtual yang ada, dengan mengkliknya akan memunculkan kotak input untuk memperbaruinya.
2. Opsi mode kerja EID Virtual

> Mode EID Virtual yang tersedia saat ini.
1. _Enabled_: Mengaktifkan fungsi EID Virtual, dalam hal ini EID yang dibaca dari ISD-R akan diganti dengan nilai yang ditetapkan oleh EID Virtual.
2. _Disabled_: Fungsi EID Virtual tidak diaktifkan.

{{% notice style="note" title="Catatan" %}}
Harap diperhatikan bahwa saat berkomunikasi dengan Server Pengunduhan Profil (SM-DP+), EID Virtual tidak dapat efektif karena adanya sistem sertifikat GSMA PKI, dan SM-DP+ selalu dapat memperoleh nomor seri EID yang sebenarnya dari eUICC.
{{% /notice %}}