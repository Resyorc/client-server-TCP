# Laporan: Sistem Klien-Server dengan Socket TCP

## Pendahuluan
Dokumen ini akan menjelaskan tentang sistem klien-server yang menggunakan socket TCP untuk komunikasi. Terdiri dari dua bagian utama, yaitu sisi server dan sisi klien. Tujuan utamanya adalah memungkinkan klien untuk berkomunikasi dengan server dan berinteraksi dengan sistem file server.

## Sisi Server
Server bertugas menerima perintah dari klien, menjalankan perintah tersebut, dan memberikan respons kepada klien. Berikut adalah fitur dan cara penggunaan Server:

### Fitur:
- Menerima perintah seperti `ls`, `rm`, `size`, `download`, `upload`, dan `byebye`.
- Melakukan operasi seperti menampilkan daftar file, menghapus file, mendapatkan ukuran file, mengunduh file, dan mengunggah file.
- Menangani berbagai jenis kesalahan seperti file tidak ditemukan atau kesalahan saat membaca/menulis file.

### Cara Penggunaan:
1. Jalankan Server dengan mengeksekusi file `server.py`.
2. Program akan menunggu koneksi dari klien. (Menunggu client mengirimkan perintah `conme`)
3. Setelah koneksi terbentuk, server akan menerima perintah dari klien.
4. Klien dapat mengirim perintah seperti `ls`, `rm`, `size`, `download`, `upload`, dan `byebye`.
5. Server akan menanggapi perintah tersebut dan menjalankan operasi yang sesuai pada sistem file server.
6. Klien dapat terus berinteraksi dengan server sampai mengirim perintah `byebye` untuk menutup koneksi.

## Sisi Klien
Klien bertugas berkomunikasi dengan server dengan mengirimkan perintah dan menerima respons. Berikut adalah fitur dan cara penggunaan klien:

### Fitur:
- Mengirim perintah seperti `ls`, `rm`, `size`, `download`, `upload`, dan `byebye` ke server.
- Menerima respons dari server dan menampilkannya kepada pengguna.
- Mengunggah file ke server dan mengunduh file dari server.

### Cara Penggunaan:
1. Jalankan klien dengan mengeksekusi file `client.py`.
2. Program akan berjalan dan menampilkan pesan bahwa klien sedang aktif.
3. Gunakan perintah `connme` untuk menghubungkan klien ke server.
4. Masukkan perintah yang diinginkan, seperti `ls`, `rm`, `size`, `download`, `upload`, dan `byebye`.
5. Klien akan mengirim perintah tersebut ke server dan menampilkan respons yang diterima dari server.
6. Pengguna dapat terus berinteraksi dengan server sampai mengirim perintah `byebye` untuk menutup koneksi.

## Kesimpulan
 Sistem klien-server ini menyediakan antarmuka sederhana untuk berkomunikasi dengan sistem file server menggunakan socket TCP. Pengguna dapat mengirim perintah ke server dan melakukan operasi seperti menampilkan daftar file, menghapus file, mengunggah file, dan mengunduh file. Tentunya, penggunaan sistem ini dapat ditingkatkan dengan peningkatan fitur keamanan dan penanganan kesalahan yang lebih baik.
