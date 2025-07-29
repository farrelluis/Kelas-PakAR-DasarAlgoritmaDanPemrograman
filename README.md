# Kelas-PakAR-DasarAlgoritmaDanPemrograman
# FARREL LUIS REINALDO 24110310024
# USER MANUAL

1. Deskripsi Aplikasi
   
   Aplikasi ini dirancang untuk membantu pemilik toko kecil dalam mengelola barang dagangan mereka. Pengguna dapat menambah, melihat, memperbarui stok, dan menghapus data barang secara langsung dari terminal/command prompt.
   

2. Cara Instalasi
   
   Pastikan Python 3 telah terinstal di perangkat Anda. Cek dengan: python --version

   Simpan file program dengan nama inventory.py.

   Jalankan aplikasi dengan perintah berikut di terminal: python inventory.py


3. Navigasi Menu

   Tambah Barang	(Menambahkan data barang baru ke inventori)

   Tampilkan Inventori	(Menampilkan semua barang beserta stok dan harga)

   Update Stok	(Menambah/mengurangi jumlah stok berdasarkan kode barang)

   Hapus Barang	(Menghapus barang dari inventori berdasarkan kode)

   Keluar	(Menutup aplikasi)


# DOKUMENTASI TEKNIS

1. Informasi Umum
   
   Nama Aplikasi: Sistem Manajemen Inventori Toko Kecil

   Versi: 1.0

   Bahasa Pemrograman: Python 3.x

   Antarmuka: CLI (Command Line Interface)

   Tujuan: Mengelola data inventori seperti tambah barang, update stok, lihat daftar barang, dan hapus barang.


2. Struktur File
   
   Semua kode berada dalam satu file Python: inventory.py


3. Struktur Data
   
   python
   
   db_inventory =
   {'B01': {'nama': 'Teh Botol', 'stok': 20, 'harga': 3000},
   'B02': {'nama': 'Kopi Sachet', 'stok': 50, 'harga': 1500},}
   
   kode → kunci utama dictionary (string)

   nama → nama barang

   stok → jumlah unit barang (integer)

   harga → harga satuan dalam rupiah (integer)


4. Struktur Fungsi
   
   4.1. tambah_barang(kode, nama, stok, harga)
   
   Menambahkan barang baru ke dalam db_inventory

   Validasi: menolak jika kode sudah ada

   Output: konfirmasi berhasil atau peringatan duplikat

   4.2. tampilkan_inventory()
   
   Menampilkan semua barang dalam tabel ASCII

   Menangani kondisi inventori kosong

   4.3. update_stok(kode, jumlah)
   
   Menambah/mengurangi stok berdasarkan input positif/negatif

   Menampilkan stok terbaru

   Validasi jika kode tidak ditemukan

   4.4. hapus_barang(kode)
   
   Menghapus barang dari db_inventory

   Validasi: kode harus ada


5. Alur Program (Main Loop)
   
   mathematica

   [Start Program]
   
    ↓
   
   [Tampilkan Menu Utama]
   
    ↓
   
   [Pilih Opsi Menu]
   
    ↓
   
   ├─> Tambah Barang → Input Data → Simpan
   
   ├─> Tampilkan Inventori → Cetak Tabel
   
   ├─> Update Stok → Input Kode + Jumlah → Update
   
   ├─> Hapus Barang → Input Kode → Hapus
   
   └─> Keluar → Program Selesai


7. Kemungkinan Pengembangan Lanjutan
   
   Ekspor/Impor data ke/dari file CSV

   Backup otomatis

   Interface berbasis GUI (Tkinter)

   Otentikasi pengguna

   Koneksi ke database SQLite/MySQL


8. Kode Modular (Penulisan Fungsi)
   
   Semua fungsi ditulis modular untuk memudahkan:

   Reuse kode

   Testing per fungsi

   Refactor ke sistem yang lebih besar










