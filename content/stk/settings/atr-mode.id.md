+++
title = "Mode ATR"
date =  2023-12-17T21:53:52+08:00
weight = 5
+++

## Mengonfigurasi respons ATR untuk eSTK.me

ATR adalah bagian pertama dari data yang dikirim oleh kartu pintar ke terminal dan berisi berbagai informasi penting mulai dari metode komunikasi hingga struktur data.

{{% notice style="tip" title="Pengoperasian yang andal" %}}
1. Anda bebas mencoba fungsi ini.
2. Hasil operasi dapat dikembalikan, atau setidaknya ada cara untuk mengembalikan ke kondisi sebelumnya.
{{% /notice %}}

"Menu pemilihan ATR" memiliki awalan yang ditunjukkan dengan karakter "<>" atau "<\*>", di mana awalan "<\*>" menunjukkan konfigurasi yang sedang aktif.  

> Mode ATR yang Tersedia Saat Ini
1. Generik: Pengumuman ATR _SmartCard_ generik.
2. eUICC: _SmartCard_ yang berisi fungsi eUICC.

{{% notice style="warning" title="Pemberitahuan" %}}
Jika "[mode ISD-R](./isd-r-mode)"" diatur ke "mati" dan eUICC ATR diberitahukan pada saat yang sama, hal ini dapat menyebabkan beberapa terminal mengatakan "_SmartCard_ rusak"
{{% /notice %}}

{{% notice style="info" title="Batasan" %}}
Meskipun eSTK.me memiliki kemampuan untuk menyesuaikan ATR sepenuhnya, ATR yang salah dapat dengan mudah menyebabkan kerusakan perangkat lunak atau bahkan kerusakan perangkat keras permanen, dan pengguna akhir hanya boleh memilih dari data ATR yang telah teruji keamanannya. Untuk pengguna OEM, eSTK.me menawarkan penyesuaian ATR yang lebih kaya dan membantu dalam menguji keandalan ATR.
{{% /notice %}}
