1. Apa yang dimaksud dengan GitHub?

```jawaban```

GitHub adalah platform berbasis web untuk pengontrol versi (version control) dan kolaborasi pengembangan perangkat lunak. GitHub menggunakan sistem Git untuk melacak perubahan pada kode sumber, memungkinkan banyak pengembang bekerja sama dalam sebuah proyek secara bersama-sama dari berbagai lokasi, serta menyediakan ruang penyimpanan (repository) untuk kode program secara publik maupun privat.

2. Apa Fitur dan Komponen Utama GitHub?

``jawaban``

Beberapa fitur dan komponen utama yang ada di GitHub meliputi:
Repository (Repo): Tempat penyimpanan seluruh file proyek beserta riwayat versinya.
Commit: Rekaman perubahan atau pembaruan kode yang telah disimpan dalam riwayat repository.
Branch: Jalur pengembangan terpisah dari proyek utama, memungkinkan pengembang membuat perubahan tanpa mengganggu kode yang sedang berjalan (main).
Pull Request (PR): Fitur untuk mengajukan dan mendiskusikan penggabungan perubahan kode dari suatu branch ke branch lainnya (misalnya dari feature branch ke main).
Issues: Alat untuk melacak tugas, melaporkan bug, atau mendiskusikan ide/fitur baru dalam proyek.
Actions: Fitur otomatisasi (CI/CD) untuk membangun, menguji, dan menerapkan kode secara otomatis.

3. Sebutkan Alur Utama (GitHub Workflow)?

```jaawaban```

Alur kerja standar dalam menggunakan GitHub umumnya meliputi tahapan berikut:
Clone / Fork: Mengambil salinan repository (ke akun pribadi atau langsung ke komputer lokal).
Create Branch: Membuat branch baru untuk mengerjakan fitur atau tugas tertentu agar tidak mengubah kode utama secara langsung.
Make Changes & Commit: Melakukan penulisan/perubahan kode di komputer lokal, lalu menyimpan perubahannya menggunakan perintah commit.
Push: Mengirimkan commit dari komputer lokal ke repository di GitHub.
Pull Request: Mengajukan pull request untuk menggabungkan kode dari branch baru ke branch utama setelah diperiksa.

4. Apa keuntungan utama dari pembatasan branch main?

```jawaban```

Keuntungan utama dari pembatasan (protection) pada branch main adalah menjaga stabilitas dan keamanan kode utama. Dengan pembatasan ini:
Kode yang belum diuji atau masih memiliki bug tidak bisa langsung dimasukkan (merge) secara sembarangan.
Mencegah kesalahan fatal (human error) yang dapat merusak aplikasi atau sistem yang sedang berjalan.
Memaksa adanya proses code review atau pengujian otomatis melalui Pull Request sebelum perubahan disetujui dan digabungkan.