# Alfamart P263 Database Viewer

Website statis untuk membaca database SQLite di browser. Mode baca-saja; file tidak dikirim ke server.

## Deploy lewat GitHub + Vercel dari HP
1. Ekstrak ZIP ini.
2. Buat repository baru di GitHub, misalnya `alfamart-p263-viewer`.
3. Upload `index.html` dan `README.md` ke root repository (bukan ke dalam folder tambahan).
4. Buka Vercel → Add New → Project → pilih repository tersebut → Deploy.
5. Karena ini website statis, tidak perlu Environment Variables atau database server.

## Cara menggunakan
Buka alamat Vercel, pilih file `.db`, lalu tekan **Buka Database**. Pilih tabel di daftar sebelah kiri/atas, gunakan pencarian, atau unduh hasil tabel sebagai CSV.

## Catatan penting untuk file yang diberikan
File `P263_2026-10-11_20121561_windows (2).db` yang diberikan tidak memiliki header SQLite standar (`SQLite format 3`). Karena itu, website ini mungkin tidak bisa membacanya jika file tersebut terenkripsi atau merupakan format khusus dari aplikasi sumber. Bila muncul pesan gagal membaca, ekspor database dari aplikasi asal sebagai SQLite standar yang tidak terenkripsi, lalu unggah hasil ekspor tersebut.
