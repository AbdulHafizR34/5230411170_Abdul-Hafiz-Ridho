Aplikasi ini adalah sistem manajemen produk dan transaksi untuk sebuah usaha retail skala kecil. Dengan menggunakan aplikasi ini, admin dapat mengelola data produk, mencatat transaksi penjualan, mengatur stok produk, serta melihat riwayat transaksi. Aplikasi ini dirancang menggunakan bahasa pemrograman Python dengan paradigma Pemrograman Berorientasi Objek (OOP) dan antarmuka berbasis GUI (Graphical User Interface) menggunakan Tkinter. Data aplikasi disimpan dalam database MySQL untuk kemudahan pengelolaan dan skalabilitas.

Fitur Utama:

CRUD (Create, Read, Update, Delete) untuk data produk.
Pencatatan transaksi penjualan.
Manajemen stok produk.
Tampilan riwayat transaksi.
Validasi input untuk menghindari kesalahan data.
Cara Menjalankan Aplikasi
Persiapan Lingkungan:

Pastikan Python 3.x telah terinstal di komputer Anda.
Instal pustaka yang diperlukan dengan menjalankan perintah berikut:
bash
Salin kode
pip install mysql-connector-python
Pastikan MySQL Server telah terinstal dan berjalan di sistem Anda.
Konfigurasi Database:

Buka aplikasi MySQL seperti phpMyAdmin atau MySQL Workbench.
Jalankan file SQL yang telah disediakan (create_retail_db.sql) untuk membuat database dan tabel yang diperlukan.
Pastikan MySQL memiliki user dengan akses yang sesuai, dan catat kredensialnya (username, password).
Menjalankan Aplikasi:

Edit file Python aplikasi untuk memasukkan konfigurasi MySQL Anda di bagian berikut:
python
Salin kode
self.conn = mysql.connector.connect(
    host="localhost",
    user="your_username",  # Ganti dengan username MySQL Anda
    password="your_password",  # Ganti dengan password MySQL Anda
    database="retail_db"
)
Jalankan aplikasi dengan perintah berikut:
bash
Salin kode
python responsi.py
Aplikasi akan membuka jendela GUI untuk manajemen produk dan transaksi.
Menggunakan Aplikasi:

Kelola Produk: Tambahkan, edit, hapus, atau lihat daftar produk.
Kelola Transaksi: Pilih produk, masukkan jumlah, dan simpan transaksi.
Lihat Riwayat Transaksi: Klik tombol untuk melihat daftar transaksi yang telah dilakukan.
