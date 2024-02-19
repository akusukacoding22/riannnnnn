## Instalasi FreeRADIUS di Ubuntu:
1. ### Buka Terminal:
   Buka terminal pada sistem Linux Anda.

2. ### Perbarui Repositori:
  
   sudo apt update

4. ### Instalasi FreeRADIUS:

   sudo apt install freeradius
   
5. ### Konfigurasi FreeRADIUS:
   Konfigurasi utama FreeRADIUS terdapat dalam berkas-berkas di direktori /etc/freeradius/. Anda dapat mengonfigurasi parameter seperti otentikasi, otorisasi, dan akuntabilitas sesuai kebutuhan.

6. ### Restart FreeRADIUS:
   Setelah mengonfigurasi, restart FreeRADIUS untuk menerapkan perubahan:

   sudo service freeradius restart
   
## Verifikasi Instalasi:
1. ### Periksa Status FreeRADIUS:

   sudo service freeradius status
   
   Pastikan tidak ada kesalahan dan layanan berjalan dengan baik.

3. ### Uji Coba Koneksi:
   Gunakan perintah radtest untuk menguji koneksi ke server RADIUS:

   radtest username password localhost 0 testing123

   Pastikan untuk mengganti username dan password sesuai kebutuhan.

   Jika Anda menggunakan distribusi Linux lain atau sistem operasi yang berbeda, proses instalasi mungkin sedikit berbeda. Selalu rujuk dokumentasi resmi dan panduan pengguna untuk distribusi        atau sistem operasi yang Anda gunakan.

   Selain itu, jika Anda membutuhkan integrasi dengan layanan direktori seperti LDAP atau Active Directory, Anda perlu mengonfigurasi parameter tambahan sesuai kebutuhan Anda. Pastikan untuk         merujuk dokumentasi FreeRADIUS dan sumber daya online lainnya untuk informasi lebih lanjut dan dukungan.

## Pengertian Radius Server
      Server RADIUS (Remote Authentication Dial-In User Service) adalah jenis server yang digunakan untuk mengelola otentikasi, otorisasi, dan akuntabilitas (AAA) pada jaringan komputer. Fungsi       utamanya adalah untuk mengelola proses otentikasi pengguna yang mencoba terhubung ke jaringan, seperti pengguna yang ingin mengakses jaringan Wi-Fi atau jaringan yang melibatkan protokol 
    dial- up.

  ### Berikut adalah beberapa poin kunci mengenai Server RADIUS:

  1. ### Otentikasi (Authentication):
     Server RADIUS digunakan untuk memverifikasi identitas pengguna yang mencoba mengakses jaringan. Ini dapat melibatkan penggunaan username dan password atau metode 
     otentikasi lainnya, seperti sertifikat digital.

  2. ### Otorisasi (Authorization):
     Setelah otentikasi berhasil, Server RADIUS menentukan hak akses yang dimiliki pengguna ke dalam jaringan. Ini mencakup pengaturan hak akses, bandwidth, dan              parameter lainnya.

  3. ### Akuntabilitas (Accounting):
     Server RADIUS mencatat informasi terkait penggunaan layanan jaringan oleh pengguna. Ini termasuk informasi seperti lama sesi, volume data yang ditransfer, dan 
     lainnya. Informasi ini dapat digunakan untuk tujuan pemantauan dan penagihan.

  4. ### Protokol RADIUS:
     RADIUS bekerja menggunakan protokol RADIUS untuk komunikasi antara perangkat yang memerlukan otentikasi (seperti akses point atau server VPN) dan Server RADIUS. Protokol ini 
     membawa informasi otentikasi dan otorisasi antara klien dan server.

  5. ### Keamanan:
     Informasi yang dikirimkan antara perangkat klien dan Server RADIUS dapat dienkripsi untuk menjaga keamanan data selama proses otentikasi.

  Server RADIUS sangat umum digunakan dalam lingkungan jaringan yang memerlukan kontrol akses dan keamanan, terutama di lingkungan di mana banyak pengguna perlu terhubung secara aman ke jaringan, 
  seperti jaringan kantor, kampus, atau layanan Wi-Fi publik.















   
