# Kelas-PakAR-DasarAlgoritmaDanPemograman
Nama : Elsa Anggita Rachmawati
NIM : 24110310019

Penjelasan Program
1. Pengembangan aplikasi
   1.1 Struktur Data
Menggunakan list of dictionaries untuk menyimpan data inventori
Setiap barang memiliki 4 atribut:
a. id (identifier unik)
b. nama (nama barang)
c. stok (jumlah stok)
d. harga (harga satuan)
2. Fitur Utama:
Tambah Barang:
1.Generate ID otomatis
a) Input data baru melalui keyboard
b) Validasi tipe data numerik
2. Tampilkan Semua Barang:
a)Menampilkan dalam format tabel
b)Penanganan kasus inventori kosong
3. Edit Barang:
a)Cari barang berdasarkan ID
b) Ubah data parsial (field tertentu saja)
c) Validasi input numerik
4. Hapus Barang:
a) Konfirmasi sebelum penghapusan
b) Pencarian berdasarkan ID
5. Cari Barang:
a)Pencarian berdasarkan nama (case-insensitive)
b)Tampilkan hasil dalam format tabel
6. Export ke CSV:
a. Simpan data ke file CSV
a)Format standar dengan header
b)Otomatis dijalankan saat keluar program
7. Laporan Inventori:
a)Total jenis barang
b)Total nilai inventori (stok x harga)
c)Rata-rata harga barang

3. Manajemen File:
Format File: CSV (Comma-Separated Values)
Nama File Default: inventori.csv
Auto-load: Memuat data saat program dijalankan
Auto-save: Menyimpan data saat keluar program
4. Keamanan Data:
Validasi tipe data input
Penanganan error file tidak ditemukan
Konfirmasi untuk operasi penghapusan

Pencarian berdasarkan ID untuk modifikasi data

5. Antarmuka Pengguna:
Menu interaktif berbasis teks
Format tabel untuk tampilan data
Input dengan petunjuk jelas
Pesan error informatif
          2. Dokumentasi Teknis 
➤ Struktur File/Kode
inventori.db – file database SQLite

Program utama langsung berisi:

Pembuatan tabel

Fungsi: tambah, edit, hapus, tampil

Contoh eksekusi fungsi
➤ Library yang Digunakan
sqlite3: menyimpan dan mengelola data barang
Tidak menggunakan library eksternal

Diagram Alur aplikasi 
[Mulai]
   ↓
[Input User: Tambah/Edit/Hapus]
   ↓
[Akses Database SQLite]
   ↓
[Update/Tampilkan Data]
   ↓
[Selesai]

    3. Panduan Pengguna Menu
1. Tambah Barang : 	Memasukkan nama dan jumlah stok barang baru
2. Tampilkan:  Barang	Menampilkan semua barang yang tersimpan
3. Edit Barang	:Mengubah jumlah stok berdasarkan ID barang
4. Hapus Barang	: Menghapus barang berdasarkan ID
5. Keluar: 	Menghentikan aplikasi

Cara Menjalankan Aplikasi
a. Simpan file Python dengan nama: inventori.py
b. Jalankan melalui terminal atau command prompt:
python inventori.py
c. Akan muncul menu utama yang menampilkan 5 pilihan:
=== MENU INVENTORI ===
1. Tambah Barang
2. Tampilkan Barang
3. Edit Barang
4. Hapus Barang
5. Keluar
Contoh Input dan Fungsi Menu
   1. Tambah Barang
Pilih menu 1 untuk menambahkan barang baru.
Masukkan nama dan jumlah stok barang.
Pilih menu (1-5): 1
Nama barang: Pulpen
Jumlah stok: 50
Hasilnya: Barang bernama Pulpen dengan stok 50 disimpan di database
2. Tampilkan Barang
Pilih menu 2 untuk melihat semua data barang yang tersimpan.
Contoh Output:
Daftar Barang:
ID: 1, Nama: Pulpen, Stok: 50
ID: 2, Nama: Buku Tulis, Stok: 30
3. Edit Data Barang
Pilih menu 3 untuk mengubah jumlah stok barang.
Diperlukan ID barang yang ingin diedit.
Masukkan jumlah stok baru.
Pilih menu (1-5): 3
Masukkan ID barang yang ingin diedit: 1
Masukkan jumlah stok baru: 100
Hasilnya: Barang dengan ID 1 (Pulpen) stoknya diubah menjadi 100.
4. Hapus Data Barang
Pilih menu 4 untuk menghapus data barang dari sistem.
Diperlukan ID barang yang ingin dihapus.
Pilih menu (1-5): 4
Masukkan ID barang yang ingin dihapus: 2
Hasilnya: Barang dengan ID 2 (Buku Tulis) dihapus dari daftar.
5. Keluar dari Aplikasi
Pilih menu 5 untuk keluar dari aplikasi.
