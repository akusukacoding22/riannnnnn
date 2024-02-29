## Install freeradius

![Capture](https://github.com/akusukacoding22/riannnnnn/assets/156275570/0f0bd0af-ae89-4c8f-aa88-8701f36d023e)



## cara menginstal FreeRadius di ubuntu

Untuk menginstal FreeRADIUS di Ubuntu, berikut adalah langkah-langkah umumnya:

### 1. Update Repositori:
    Pastikan repositori paket Anda diperbarui sebelum menginstal paket baru.

    sudo apt update
### 2. Instal FreeRADIUS:
    Gunakan perintah berikut untuk menginstal FreeRADIUS pada sistem Ubuntu Anda.

    sudo apt install freeradius
    Ikuti petunjuk pada layar untuk menyelesaikan instalasi.

### 3. Konfigurasi:
    Buka atau buat berkas konfigurasi pengguna, misalnya /etc/freeradius/3.0/users:

    sudo nano /etc/freeradius/3.0/users.

### 4. Mulai Layanan FreeRADIUS:
    Setelah konfigurasi selesai, mulai layanan FreeRADIUS.

    sudo service freeradius start
    Atau menggunakan perintah berikut:

    sudo systemctl start freeradius
    Jika Anda ingin mengatur agar FreeRADIUS berjalan otomatis saat sistem boot:

    sudo systemctl enable freeradius
### 5. Uji Fungsionalitas:
    Uji fungsionalitas FreeRADIUS dengan menggunakan alat pengujian seperti radtest. Pastikan untuk menggantikan <username> dan <password> dengan informasi yang sesuai.

    radtest <username> <password> localhost 0 testing123
### 6. Dokumentasi dan Bantuan:
    Selalu merujuk pada dokumentasi resmi FreeRADIUS dan sumber daya komunitas untuk panduan lebih lanjut dan bantuan jika diperlukan.

    Penting untuk dicatat bahwa konfigurasi FreeRADIUS dapat menjadi tugas yang rumit tergantung pada kebutuhan spesifik Anda. Dokumentasi resmi FreeRADIUS akan memberikan panduan rinci dan dapat membantu Anda mengonfigurasi server Radius sesuai kebutuhan Anda.

## Untuk membuat pengguna dengan konfigurasi FreeRADIUS yang sangat minimal, Anda hanya perlu menambahkan entri pengguna dalam berkas konfigurasi yang digunakan oleh modul "files". Di bawah ini adalah contoh cara menambahkan pengguna secara minimal:

### Langkah 1: Buka Berkas Konfigurasi User
    Buka atau buat berkas konfigurasi pengguna, misalnya /etc/freeradius/3.0/users:

    sudo nano /etc/freeradius/3.0/users
### Langkah 2: Tambahkan Pengguna
    Tambahkan pengguna dengan memberikan nama pengguna dan kata sandi. Contoh:

    john  Cleartext-Password := "secret"
    Simpan dan keluar dari editor.

### Langkah 3: Uji Fungsionalitas
    Restart layanan FreeRADIUS:

    sudo systemctl restart freeradius
    Uji fungsionalitas dengan menggunakan alat pengujian bawaan seperti radtest. Misalnya, untuk menguji pengguna dengan nama pengguna "john" dan kata sandi "secret":

    radtest john secret localhost 0 testing123
    Pastikan untuk menggantikan "john" dan "secret" dengan nilai sesuai.

    Dengan langkah-langkah ini, Anda telah membuat pengguna dengan konfigurasi FreeRADIUS yang sangat minimal. Pastikan untuk menyesuaikan konfigurasi lebih lanjut sesuai kebutuhan Anda. Jika Anda hanya membutuhkan otentikasi pengguna yang sangat sederhana, langkah-langkah di atas sudah mencakup kebutuhan tersebut.
