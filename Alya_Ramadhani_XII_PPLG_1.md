1. Keuntungannya yaitu supaya kode yang masih dalam proses atau belum diuji tidak langsung masuk ke branch main. Jadi kalau ada error, branch main tetap aman dan tidak mengganggu sistem yang sedang digunakan.
2. Perintah Git yang digunakan adalah
  git clone <URL-repository>
  cd sts_version_control
  git checkout -b jawaban-Alya_Ramadhani_XII_PPLG_1
  git add Alya_Ramadhani_XII_PPLG_1.md
  git commit -m "Menambahkan jawaban studi kasus MFA"
  git push -u origin jawaban-Alya_Ramadhani_XII_PPLG_1
