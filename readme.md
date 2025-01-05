Keuangan Harian dan Pengelola Data Mahasiswa
Repositori ini berisi dua aplikasi sederhana yang dibuat untuk memenuhi tugas mata kuliah Algoritma dan Pemrograman I. Berikut deskripsi dari masing-masing aplikasi:

1. Aplikasi Keuangan Harian
Deskripsi
Aplikasi Keuangan Harian adalah aplikasi berbasis konsol yang membantu pengguna mencatat pengeluaran harian mereka. Aplikasi ini memungkinkan pengguna untuk:
- Menambahkan pengeluaran dengan kategori tertentu.
- Menampilkan total pengeluaran yang telah dicatat.
- Menampilkan sisa saldo setelah pengeluaran.

Fitur Utama
1. Tambah Pengeluaran
   - Pengguna dapat memasukkan nama kategori pengeluaran dan jumlahnya.
   - Jumlah pengeluaran akan ditambahkan ke total pengeluaran dan dikurangkan dari saldo.

2. Tampilkan Total Pengeluaran
   - Menampilkan total pengeluaran yang telah tercatat sejauh ini.

3. Tampilkan Sisa Saldo
   - Menampilkan sisa saldo setelah dikurangi oleh pengeluaran yang tercatat.

4. Keluar dari Aplikasi
   - Menutup aplikasi dengan menampilkan pesan perpisahan.

Teknologi yang Digunakan
- Bahasa Pemrograman: C++

---

2. Aplikasi Pengelola Data Mahasiswa

Deskripsi
Aplikasi ini membantu mengelola data mahasiswa seperti NIM, nama, dan nilai akhir. Aplikasi ini dilengkapi dengan fitur pencarian, pengurutan, dan penyimpanan data ke dalam berkas.

Fitur Utama
1. Tambah Data Mahasiswa
   - Pengguna dapat memasukkan data mahasiswa seperti NIM, nama, dan nilai akhir.

2. Tampilkan Semua Data
   - Menampilkan seluruh data mahasiswa yang tersimpan.

3. Cari Data Mahasiswa
   - Mencari data mahasiswa berdasarkan NIM menggunakan algoritma pencarian linear.

4. Urutkan Data
   - Mengurutkan data mahasiswa berdasarkan nilai akhir dalam urutan menurun menggunakan algoritma Bubble Sort.

5. Simpan Data ke Berkas
   - Menyimpan data mahasiswa ke dalam file teks untuk keperluan penyimpanan permanen.

6. Baca Data dari Berkas
   - Membaca data mahasiswa dari file teks dan memuatnya kembali ke dalam aplikasi.

7. Keluar dari Aplikasi
   - Menutup aplikasi.

Teknologi yang Digunakan
- Bahasa Pemrograman: C++
- File Handling untuk penyimpanan dan pembacaan data.

---

Cara Penggunaan
1. Clone repositori ini ke komputer Anda.
   ```bash
   git clone <repository_url>
   ```
2. Compile dan jalankan masing-masing file source code menggunakan compiler C++ seperti `g++`.
   ```bash
   g++ keuangan_harian.cpp -o keuangan_harian
   ./keuangan_harian

   g++ pengelola_mahasiswa.cpp -o pengelola_mahasiswa
   ./pengelola_mahasiswa
   ```
3. Ikuti petunjuk di layar untuk menggunakan aplikasi.


