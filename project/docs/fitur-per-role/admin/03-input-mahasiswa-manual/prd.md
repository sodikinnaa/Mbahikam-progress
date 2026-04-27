# PRD - Admin - Input Mahasiswa Manual

## Tujuan Fitur
Memungkinkan admin menambahkan mahasiswa langsung ke sistem tanpa registrasi mandiri.

## Ruang Lingkup
Hanya mencakup proses input data mahasiswa manual dan pembuatan akun awal.

## Pengguna
- Admin Kominfo

## Kebutuhan Fungsional
1. Admin dapat membuka form input mahasiswa manual.
2. Admin dapat mengisi data identitas mahasiswa.
3. Sistem memvalidasi data wajib sebelum akun dibuat.
4. Sistem membuat akun mahasiswa otomatis setelah data valid.
5. Sistem menetapkan status awal akun mahasiswa.
6. Sistem menampilkan kredensial awal setelah akun berhasil dibuat.

## Kebutuhan Non-Fungsional
1. Proses pembuatan akun manual harus selesai dalam satu alur tanpa pindah halaman.
2. Data mahasiswa baru harus langsung tersedia di daftar mahasiswa.

## Acceptance Criteria
1. Jika data input valid, akun mahasiswa berhasil dibuat dan tersimpan.
2. Jika data tidak valid, sistem menolak penyimpanan dan menampilkan field yang bermasalah.
3. Mahasiswa baru tampil pada daftar peserta dengan status awal yang ditetapkan.
4. Kredensial awal dapat dilihat admin setelah proses berhasil.
