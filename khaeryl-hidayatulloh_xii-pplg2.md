# Jawaban Studi Kasus Version Control

## 1. Keuntungan Utama Pembatasan Branch Main
- Menjaga stabilitas sistem (production stability) dari bug atau kode yang belum matang.
- Kolaborasi tim menjadi lebih aman dan terstruktur secara paralel.
- Memungkinkan proses Code Review melalui Pull Request sebelum kode digabung.

## 2. Perintah Git yang Digunakan
```bash
git checkout main
git pull origin main
git checkout -b jawaban-khaeryl-hidayatulloh_xii-pplg2
git status
git add .
git commit -m "feat: menambahkan jawaban studi kasus version control mfa"
git push origin jawaban-khaeryl-hidayatulloh_xii-pplg2 
