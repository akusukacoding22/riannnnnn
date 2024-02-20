## Membuat situs web statis di GitHub menggunakan Jekyll adalah pilihan yang baik, karena GitHub secara otomatis mendukung Jekyll untuk meng-host situs web statis. Berikut adalah langkah-langkah dasar untuk membuat situs web statis menggunakan Jekyll di GitHub:

1. ### Buat Repositori di GitHub:

   Buat repositori baru di GitHub.
   Pastikan untuk menambahkan file README.md untuk memulai repositori.
2. ### Instalasi Jekyll secara Lokal (Opsional):

   Jika Anda ingin mengedit situs web secara lokal sebelum mengunggahnya ke GitHub, instal Jekyll secara lokal. Pastikan sudah memiliki Ruby dan RubyGems diinstal.
   Buka terminal dan jalankan perintah:
   
   gem install jekyll bundler
3. ### Buat Situs Jekyll:

   Gunakan perintah berikut untuk membuat situs Jekyll baru:

   jekyll new nama-situs
   Ganti nama-situs dengan nama yang Anda inginkan.
4. ### Uji Situs Lokal (Opsional):

   Pindah ke direktori situs yang baru dibuat:

   cd nama-situs
   Jalankan server lokal untuk melihat situs:

   bundle exec jekyll serve
   Buka browser dan kunjungi http://localhost:4000 untuk melihat situs Anda secara lokal.
5. ### Edit Konten:

Sesuaikan konten situs web sesuai kebutuhan Anda. Template dan struktur umumnya berada di folder _layouts dan _posts.
6. ### Konfigurasi:

  Jelajahi dan edit file _config.yml untuk mengonfigurasi pengaturan situs, seperti judul, deskripsi, dan pengaturan lainnya.
7. ### Commit dan Push ke GitHub:

  Tambahkan semua perubahan ke git, buat commit, dan dorong ke repositori GitHub:

  git add .
  git commit -m "Menambahkan situs Jekyll"
  git push origin master
8. ### Aktifkan GitHub Pages:

  Buka halaman repositori di GitHub.
  Pergi ke tab "Settings".
  Gulir ke bawah hingga bagian "GitHub Pages".
  Pilih branch yang mengandung situs web Anda (biasanya "master").
  Tekan "Save" untuk mengaktifkan GitHub Pages.
Sekarang, situs web Anda akan dapat diakses di https://username.github.io/nama-repositori. Pastikan untuk mengganti username dengan nama pengguna GitHub Anda dan nama-repositori dengan nama repositori GitHub Anda. Setelah mengikuti langkah-langkah ini, situs web statis Anda akan di-host di GitHub Pages.
