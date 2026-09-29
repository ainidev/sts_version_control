**Nama:** Aini Nur Halimah  
**Kelas:** 12 PPLG  1

---

### 1. Keuntungan Utama Pembatasan Branch `main`
* **Menjaga Stabilitas Kode Utama:** Mencegah terjadinya *production crash* akibat kodingan yang belum diuji coba atau masih memiliki *bug*.
* **Mempermudah Code Review:** Mengontrol kualitas kode melalui proses review sebelum kodingan digabungkan (*merge*).
* **Isolasi Fitur:** Memungkinkan pengembang mengerjakan fitur baru secara mandiri tanpa menggangu kodingan utama anggota tim lainnya.

```bash
# Membuat dan berpindah ke branch fitur baru
git checkout -b feature/mfa-auth

# Menambahkan file yang telah diubah ke staging area
git add .

# Menyimpan perubahan secara lokal dengan commit message terstruktur
git commit -m "feat: tambahkan fitur autentikasi multi-faktor (MFA)"

# Mengirimkan branch fitur ke remote repository (GitHub)
git push -u origin feature/mfa-auth