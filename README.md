# Tugas PTI CI

## Informasi Mahasiswa
- **Nama:** Andrian Baros
- **NIM:** 10122003
- **Kelas:** IF1

## Deskripsi Proyek
Ini adalah proyek tugas PTI (Prinsip Teknologi Informasi) yang menggunakan framework CodeIgniter. Proyek ini berfokus pada pengelolaan data item dengan fitur CRUD (Create, Read, Update, Delete) serta pagination untuk tampilan data.

## Fitur
- **Autentikasi User:** Membatasi akses ke halaman tertentu berdasarkan status login.
- **Pengelolaan Data Item:**
  - **Tambah Item** (Create)
  - **Lihat Daftar Item** (Read) dengan pagination.
  - **Edit Item** (Update)
  - **Hapus Item** (Delete)
  - **Pencarian Item** berdasarkan kode model.
- **Pagination:** Menampilkan data item secara bertahap (10 per halaman).

## Struktur Direktori
- `controllers/Newitem.php`: Controller utama yang menangani logika aplikasi.
- `models/Item_model.php`: Model untuk berinteraksi dengan database, khususnya tabel `items`.
- `views/t-new-item.php` dan `new-item.php`: Menampilkan data item dalam bentuk tabel.
- `config/`: Pengaturan dasar CodeIgniter, termasuk konfigurasi database.

## Konfigurasi
1. **Persiapan Database**:
   - Buat database baru di MySQL/MariaDB.
   - Buat tabel `items` atau sesuaikan dengan skema yang ada di `models/Item_model.php`.
   
2. **Pengaturan Database di CodeIgniter**:
   - Buka file `application/config/database.php`.
   - Masukkan konfigurasi database (hostname, username, password, dan nama database).

3. **Jalankan Proyek**:
   - Letakkan folder proyek ini di dalam folder `htdocs` (untuk XAMPP) atau `www` (untuk WAMP).
   - Akses proyek melalui `http://localhost/nama-folder-proyek`.

## Endpoints Penting
- **`/newitem/index`**: Menampilkan daftar item dengan sidebar dan autentikasi.
- **`/newitem/lihat_item_paging`**: Menampilkan item dengan pagination.
- **`/newitem/proses_item`**: Menambah atau mengedit item.
- **`/newitem/delete_item/{kd_model}`**: Menghapus item berdasarkan kode model.
- **`/newitem/proses_cari_item`**: Melakukan pencarian item berdasarkan kode model.

## Catatan Tambahan
- Pastikan `jml_produk` di-set saat menambah atau mengedit item untuk menghindari error.
- Gunakan versi PHP dan MySQL yang kompatibel dengan CodeIgniter 3.x (versi framework ini).

## Lisensi
Proyek ini diselesaikan untuk keperluan akademik dan merupakan bagian dari tugas PTI di Universitas Komputer Indonesia.

