---
layout: post
title:  "Welcome to Jekyll!"
date:   2024-01-23 13:49:42 +0800
categories: jekyll update

ntuk menginstal Jekyll melalui Command Prompt (CMD) di Windows, Anda dapat mengikuti langkah-langkah berikut:

Catatan: Pastikan Anda sudah menginstal Ruby dan RubyGems di komputer Anda sebelum memulai proses instalasi Jekyll.

Langkah-langkah Instalasi Jekyll di Windows:
Buka Command Prompt:

Buka Start menu, cari "Command Prompt," dan buka aplikasi Command Prompt.
Atau, tekan tombol Windows + R, ketik cmd, dan tekan Enter.
Instal Jekyll dan Bundler:
Jalankan perintah berikut untuk menginstal Jekyll dan Bundler menggunakan RubyGems:

bash
Copy code
gem install jekyll bundler
Buat Proyek Jekyll Baru:
Pilih atau buat direktori tempat Anda ingin membuat proyek Jekyll baru, lalu jalankan perintah:

bash
Copy code
jekyll new namaprojek
Gantilah "namaprojek" dengan nama yang Anda inginkan untuk proyek Anda.

Pindah ke Direktori Proyek:
Pindah ke direktori proyek yang baru dibuat:

bash
Copy code
cd namaprojek
Jalankan Server Pengembangan Jekyll:
Untuk melihat situs web Jekyll secara lokal, jalankan perintah berikut:

bash
Copy code
bundle exec jekyll serve
Jika Anda tidak menggunakan Bundler, gunakan perintah ini:

bash
Copy code
jekyll serve
Buka Browser:
Buka browser web Anda dan kunjungi http://localhost:4000 untuk melihat situs web Jekyll yang sedang dikembangkan.

Dengan langkah-langkah ini, Anda seharusnya dapat menginstal dan menjalankan Jekyll di Windows menggunakan Command Prompt. Jika Anda mengalami masalah atau memiliki pertanyaan lebih lanjut, beri tahu saya!






