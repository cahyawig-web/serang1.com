# BotolPro — Website Admin Penjualan

## Cara menjalankan
1. Ekstrak ZIP.
2. Buka `index.html` di browser, atau unggah seluruh isi folder ke repository GitHub.
3. Aktifkan GitHub Pages dari **Settings → Pages → Deploy from a branch**, pilih branch `main` dan folder `/ (root)`.
4. Buka alamat GitHub Pages yang diberikan.

## Aturan perhitungan
- Penjualan 0–17 botol per sales per hari: uang penjualan Rp0.
- Penjualan 18–24 botol per sales per hari: Rp15.000.
- Penjualan minimal 25 botol per sales per hari: Rp40.000.
- Uang absen Rp10.000 untuk setiap hari yang memiliki catatan penjualan lebih dari 0 botol.
- Syarat uang absen: total penjualan sales selama Senin–Minggu minimal 25 botol. Jika kurang dari 25 botol, uang absen seluruh hari pada minggu tersebut menjadi Rp0.
- Jika sales tidak memiliki catatan pada suatu hari, hari tersebut tidak dihitung sebagai hari absen berbayar.

## Fitur
- Tambah, lihat, edit, hapus catatan penjualan.
- Mencegah dua catatan untuk nama sales yang sama pada tanggal yang sama.
- Ringkasan harian, rekap absensi mingguan, peringkat dan ekspor CSV.
- Data tersimpan di `localStorage` browser.

## Catatan penting tentang GitHub Pages
GitHub Pages hanya meng-host file statis. Data tersimpan pada browser/perangkat yang digunakan, bukan otomatis tersinkron ke semua perangkat atau admin lain. Jika ingin beberapa admin mengakses dan mengubah database yang sama dari HP/laptop berbeda, aplikasi perlu dihubungkan ke backend/database seperti Supabase atau Firebase. Jangan menghapus data browser sebelum membuat cadangan.
