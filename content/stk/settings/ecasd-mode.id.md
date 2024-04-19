+++
title = "Mode ECASD"
date =  2023-12-17T21:54:02+08:00
weight = 7
+++

## Mengonfigurasi perilaku domain manajemen ECASD

ECASD adalah domain manajemen khusus, berbeda dari ISD-R, ECASD memegang sertifikat paling penting dan data kunci eUICC, dapat dipahami sebagai _backend_ eUICC, biasanya, kecuali untuk produsen eSE, tidak perlu mengakses domain ECASD.

{{% notice style="tip" title="Mengkonfigurasi ECASD adalah operasi yang dapat diandalkan" %}}
1. Anda bebas mencoba fungsi ini.
2. Hasil operasi dapat dikembalikan, atau setidaknya ada cara untuk mengembalikan ke kondisi sebelumnya.
{{% /notice %}}

"Menu pilihan ECASD" memiliki awalan yang ditunjukkan dengan karakter "< >" atau "<\*>", di mana awalan "<\*>" menunjukkan konfigurasi yang sedang aktif.

> Mode ECASD yang tersedia saat ini
1. _Enabled_: Mode _default_, ECASD dapat diakses secara normal.
2. _Disabled_: Mode dinonaktifkan, di mana perangkat akhir tidak dapat mengakses domain ECASD.