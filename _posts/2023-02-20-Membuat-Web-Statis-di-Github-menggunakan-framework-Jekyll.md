## Membuat Web Statis di Github menggunakan framework Jekyll

Membuat situs web statis dengan menggunakan Jekyll dan meng-hostingnya di GitHub Pages adalah pilihan yang baik untuk membuat situs web yang ringan dan mudah dikelola. Berikut langkah-langkah umumnya:

Instalasi Jekyll:
Pastikan Anda memiliki Ruby dan RubyGems diinstal. Kemudian, instal Jekyll dengan perintah:

              gem install jekyll bundler

Buat Proyek Baru Jekyll:
Buat situs web Jekyll baru dengan perintah:

             jekyll new namaprojek

Ganti "namaprojek" dengan nama yang Anda inginkan untuk proyek Anda.

Pindah ke Direktori Proyek:

Masuk ke direktori proyek yang baru dibuat:


            cd namaprojek

Jalankan Server Lokal:

Jalankan server lokal untuk melihat situs Anda:


            bundle exec jekyll serve

Buka browser dan kunjungi http://localhost:4000 untuk melihat situs Anda.

Sunting Konten:

Sesuaikan konten Anda di dalam direktori _posts untuk posting blog, _layouts untuk layout, dan _includes untuk komponen yang dapat digunakan kembali.

Konfigurasi _config.yml:

Sesuaikan konfigurasi situs Anda dengan mengedit file _config.yml.

Uji Situs secara Lokal:

Pastikan situs Anda terlihat dengan baik secara lokal sebelum meng-hostingnya.

Inisialisasi Repository GitHub:

Buat repository baru di GitHub dan ikuti petunjuk untuk menginisialisasi dengan README. Pastikan nama repositori sesuai dengan username.github.io jika Anda ingin menggunakan GitHub Pages.

Host di GitHub Pages:

Pada pengaturan repository di GitHub, pilih sumber untuk GitHub Pages. Pilih branch "main" atau "master" (atau branch yang Anda pilih) sebagai branch yang akan di-host.

Akses Situs Web:

Setelah beberapa saat, situs web Anda akan dapat diakses di https://username.github.io (gantilah "username" dengan nama pengguna GitHub Anda).

Situs web Jekyll Anda sekarang akan di-host di GitHub Pages. Jika Anda membuat perubahan di repositori GitHub, itu akan secara otomatis diterapkan di situs web publik Anda. Jangan lupa untuk memahami struktur direktori dan berbagai fitur yang ditawarkan oleh Jekyll untuk mengoptimalkan penggunaannya.





