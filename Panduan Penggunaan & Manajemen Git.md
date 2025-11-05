# Panduan Penggunaan & Manajemen Git
Dokumen ini berisi langkah-langkah dasar untuk menggunakan Git dalam pengembangan proyek dan pengelolaan versi aplikasi.


## Create Group
Buat **group** dengan nama aplikasi yang diinginkan.  
Group berfungsi sebagai wadah utama untuk mengelompokkan seluruh proyek yang berkaitan dengan aplikasi tersebut.


## Membuat Project
Buat **project** baru berdasarkan nama fitur atau modul yang akan dikembangkan.  
Setiap fitur dapat dibuat dalam satu repository terpisah agar pengelolaan lebih mudah.


## Git Clone
Lakukan *clone* repository dari remote ke lokal menggunakan perintah: `git clone <url-repository>`


## Simpan Credential Git
Agar Git menyimpan kredensial (username & password/token) secara permanen, jalankan perintah: `git config --global credential.helper store`


## Membuat dan Berpindah ke Branch
- Gunakan perintah berikut untuk membuat branch: `git branch -b nama_branch`
- Gunakan perintah berikut untuk berpindah branch: `git checkout -b development`
- Untuk melihat riwayat commit secara ringkas: `git log --oneline`


## Membuat Tag Versi Rilis
Sebelum melakukan rilis, buat tag versi dengan perintah: `git tag -a v2.0.0 -m "release feature 2.0.0"`
```
Tujuan: Setiap rilis memiliki versi (versioning) yang jelas untuk memudahkan pelacakan perubahan dan pengelolaan rilis.
```


## Menggabungkan Beberapa Commit (Cherry-pick)
Untuk mengambil perubahan dari dua commit tertentu dan menggabungkannya dalam satu branch aktif, gunakan perintah: `git cherry-pick idcommit1 idcommit2`
```
Tujuan: Menggabungkan beberapa commit spesifik tanpa harus melakukan merge seluruh branch.
```


```
  Catatan Tambahan
```
- Gunakan pesan commit yang deskriptif dan konsisten.
- Lakukan pull secara berkala untuk memastikan repository lokal tetap sinkron dengan remote.
- Selalu gunakan branch khusus untuk setiap fitur atau perbaikan bug (feature branch / bugfix branch).
