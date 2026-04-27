# PRD - Admin - Kelola Periode Magang

## Tujuan Fitur
Memungkinkan admin mengelola periode magang agar jadwal dan kuota peserta terkontrol.

## Ruang Lingkup
Hanya mencakup pengelolaan data periode magang (tambah, ubah, hapus).

## Pengguna
- Admin Kominfo

## Kebutuhan Fungsional
1. Admin dapat menambah periode magang baru.
2. Admin dapat mengubah data periode magang.
3. Admin dapat menghapus periode magang.
4. Sistem menyimpan tanggal mulai, tanggal selesai, dan kuota pada setiap periode.
5. Sistem menampilkan daftar periode beserta status aktif atau nonaktif.

## Kebutuhan Non-Fungsional
1. Form validasi wajib berjalan sebelum data disimpan.
2. Perubahan data periode harus tercatat pada log aktivitas admin.

## Acceptance Criteria
1. Ketika admin menambah periode dengan data valid, periode baru muncul di daftar.
2. Ketika admin mengubah periode, data terbaru langsung tampil pada daftar periode.
3. Ketika admin menghapus periode, data periode tidak muncul lagi pada daftar.
4. Sistem menolak penyimpanan jika tanggal atau kuota tidak valid.
