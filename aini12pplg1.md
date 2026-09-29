1. Keuntungan Utama Pembatasan Branch main
Mencegah Production Crash: Branch main merupakan cerminan dari aplikasi yang siap dipakai (production). Melarang commit langsung memastikan kode yang belum teruji tidak merusak sistem.

Memfasilitasi Code Review: Perubahan harus diajukan melalui Pull Request (PR) terlebih dahulu, sehingga anggota tim atau ketua tim dapat meninjau kualitas kode dan keamanan sebelum digabungkan (merge).

Isolasi Fitur yang Aman: Pengembang dapat bebas bereksperimen atau mengerjakan fitur baru (seperti MFA) di branch terpisah tanpa mengganggu pekerjaan anggota tim lainnya.

Melacak History dengan Rapi: Memudahkan penelusuran riwayat commit dan mempermudah proses rollback jika ditemukan bug di masa mendatang.


# 1. Pindah ke branch fitur baru
git checkout -b feature/authentication-mfa

# 2. Mengecek status perubahan file di lokal
git status

# 3. Menambahkan file perubahan ke staging area
git add .

# 4. Menyimpan perubahan ke repository lokal dengan pesan terstruktur
git commit -m "feat: add multi-factor authentication (MFA) feature"

# 5. Mengirimkan branch fitur ke remote repository (GitHub)
git push -u origin feature/authentication-mfa