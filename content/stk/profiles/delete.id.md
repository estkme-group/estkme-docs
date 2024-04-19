+++
title = "Hapus Profil"
date =  2023-12-17T21:23:18+08:00
weight = 4
+++

## Menghapus profil yang dipilih

{{% notice style="warning" title="Operasi berbahaya" %}}
1. Hasil dari operasi ini dalam banyak kasus tidak dapat diubah dan hanya sekali saja.
2. Anda harus sangat menyadari apa yang Anda lakukan dan tidak boleh menerima begitu saja saran dari orang lain.
3. Penghapusan di dalam STK (_SIM ToolKit_) merupakan "penghapusan luring", yang berarti bahwa server manajemen tidak akan segera diberitahu jika ada penghapusan yang dilakukan.
{{% /notice %}}

Prosedur Operasi

1. Kotak _pop-up_ akan muncul untuk mengkonfirmasi penghapusan dan peringatan risiko akan ditampilkan.
2. Pengguna harus memasukkan _string_ yang ditentukan untuk mengonfirmasi penghapusan dua kali.
3. Kotak _pop-up_ untuk penghapusan berhasil atau dibatalkan.

{{% notice style="info" title="Tentang pemberitahuan penghapusan" %}}
STK (_SIM ToolKit_) tidak membuang "Pemberitahuan Penghapusan" yang seharusnya dikirim ke server manajemen, sebenarnya masih tersimpan di dalam chip dan dapat dikirim lagi ke server manajemen oleh perangkat lunak LPA untuk menyelesaikan "Penghapusan Daring" saat terhubung ke internet.
{{% /notice %}}
