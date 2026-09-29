# Jawaban Studi Kasus Git & GitHub

## 1. Apa yang Dimaksud dengan GitHub?
**GitHub** adalah platform berbasis web yang digunakan untuk meng-host, mengelola, dan meninjau kode sumber proyek perangkat lunak. GitHub memanfaatkan sistem kontrol versi **Git**, sehingga memungkinkan para pengembang (developer) untuk melacak perubahan kode, berkolaborasi dalam tim, serta mengelola versi proyek secara efisien dari mana saja.

---

## 2. Fitur dan Komponen Utama GitHub
* **Repository (Repo):** Ruang penyimpanan untuk menyimpan seluruh berkas proyek, termasuk riwayat perubahan kode.
* **Branch (Cabang):** Salinan independen dari kode utama yang digunakan untuk mengembangkan fitur baru atau memproses perbaikan tanpa mengganggu kode utama.
* **Commit:** Catatan snapshot atau penanda perubahan kode yang telah disimpan ke dalam riwayat repositori.
* **Pull Request (PR):** Fitur untuk mengajukan permohonan penggabungan kode (*merge*) dari satu branch ke branch lain (biasanya dari branch fitur ke branch `main`), sekaligus menjadi wadah untuk *code review*.
* **Issues:** Sistem pelacak kendala yang digunakan untuk mencatat bug, perbaikan, saran fitur, atau tugas-tugas proyek.
* **GitHub Actions:** Fitur otomatisasi alur kerja (CI/CD) untuk menjalankan pengujian otomatis, build, hingga pengunduhan/penyebaran (*deployment*) aplikasi.
* **Fork:** Fitur untuk menggandakan repositori milik orang lain ke dalam akun GitHub pribadi agar bisa dimodifikasi secara mandiri.

---

## 3. Alur Utama (GitHub Workflow)
Alur kerja standar di GitHub umumnya mengikuti langkah-langkah berikut:

1. **Create a Branch:** Membuat branch baru dari branch utama (`main`) khusus untuk pengerjaan tugas atau fitur tertentu.
2. **Make Changes & Commit:** Mengubah atau menambahkan kode di branch tersebut, lalu melakukan *commit* dengan pesan yang jelas.
3. **Open a Pull Request (PR):** Mengajukan *Pull Request* ke branch utama untuk memberitahukan tim/penilai bahwa pekerjaan telah selesai dan siap ditinjau.
4. **Review & Discuss:** Tim atau penguji melakukan pemeriksaan kode (*code review*), memberikan tanggapan, atau meminta revisi jika diperlukan.
5. **Merge:** Setelah persetujuan (*approval*) diberikan dan pengujian lolos, kode dari branch fitur digabungkan (*merge*) ke branch `main`.
6. **Delete Branch:** Menghapus branch fitur yang sudah tidak terpakai agar struktur repositori tetap rapi.

---

## 4. Keuntungan Utama dari Pembatasan Branch Main (*Branch Protection Rules*)
* **Menjaga Stabilitas Kode Utama:** Mencegah kode yang rusak, belum teruji, atau memiliki *bug* masuk secara tidak sengaja ke branch `main`.
* **Mewajibkan Proses Review:** Memastikan setiap perubahan kode harus diperiksa dan disetujui (*approval*) oleh anggota tim lain atau guru sebelum digabungkan.
* **Keamanan Akses:** Mencegah terjadinya tindakan penghapusan atau timpa kode (*force push*) secara tidak sengaja pada branch utama.
* **Otomatisasi Pengujian:** Memastikan seluruh pengujian otomatis (*automated tests/CI*) telah lulus terlebih dahulu sebelum kode diizinkan masuk ke `main`.