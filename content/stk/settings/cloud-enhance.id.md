+++
title = "Peningkatan Awan"
date =  2023-12-17T21:54:11+08:00
weight = 2
+++

## Mengonfigurasi Peningkatan Awan

Peningkatan Awan bergantung pada server yang terletak di Internet untuk bekerja, dan pengguna perlu menentukan alamat server dan apakah akan mengaktifkan fitur tersebut atau tidak.

{{% notice style="note" title="Diperlukan Internet" %}}
Penggunaan fitur Peningkatan Awan tertentu mengharuskan Profil yang sedang diaktifkan memiliki akses ke Internet melalui lalu lintas data. Biasanya WiFi tidak dapat menggantikan persyaratan ini.
{{% /notice %}}

{{% notice style="warning" title="Harap waspadai keamanan jaringan" %}}
Selama penggunaan fitur yang disediakan oleh Peningkatan Awan, kartu akan mengirimkan datanya sendiri melalui Internet dan berinteraksi dengan sistem komputer eksternal.

Dalam skenario ini, Kartu akan terpapar pada ancaman keamanan siber yang sama dengan sistem komputer biasa.

1. Risiko kebocoran privasi: termasuk namun tidak terbatas pada informasi seperti Nomor Identifikasi Unik Kartu, Profil, dll.
2. Risiko server jahat: termasuk namun tidak terbatas pada data kartu yang dihapus, ditransfer, atau diberikan kepada pihak ketiga.
3. Risiko yang timbul dari keterbatasan buatan atau teknis lainnya.

Peningkatan Awan tidak dapat menghindari penyadapan dan pembajakan tingkat operator.
{{% /notice %}}

{{% notice style="tip" title="Pengoperasian yang andal" %}}
1. Anda bebas mencoba fungsi ini.
2. Hasil operasi dapat dikembalikan, atau setidaknya ada cara untuk mengembalikan ke kondisi sebelumnya.
{{% /notice %}}

Setelah mengklik item menu ini, maka akan muncul:
1. Alamat server RemoteLPA saat ini, klik untuk mengubahnya.
2. Opsi mode kerja Peningkatan Awan.

> Opsi mode Peningkatan Awan yang tersedia saat ini
1. Enabled : Diaktifkan
2. Disabled : Dinonaktifkan


{{% notice style="info" title="Tentang Server" %}}
Server RemoteLPA merupakan sumber terbuka dalam proyek lpac di bawah protokol AGPL v3, dan dapat diatur sendiri jika memenuhi persyaratan IPv4 publik dan salah satu port TCP yang dapat diakses.
{{% /notice %}}

{{% notice style="tip" title="Bukan tautan langsung" %}}
Mengaktifkan fitur Peningkatan Awan tidak akan membuat sambungan Internet; sambungan jaringan hanya dibuat ketika fitur Peningkatan Awan tertentu digunakan secara aktif. Tautan ke Internet akan terputus segera setelah operasi fitur berakhir.
{{% /notice %}}
