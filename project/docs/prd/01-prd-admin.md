# PRD Role: Admin Kominfo

## Ringkasan
Admin bertugas mengelola siklus administrasi magang dari periode, pendaftaran, assignment mentor, monitoring, hingga pelaporan.

## Tujuan Produk (Admin)

1. Mempercepat validasi pendaftaran.
2. Memastikan distribusi mentor dan kuota periode terkontrol.
3. Menyediakan monitoring real-time aktivitas mahasiswa.
4. Menghasilkan laporan dan output akhir secara cepat.

## Fitur Utama

1. Login/logout admin
2. Manajemen periode magang
3. Validasi pendaftaran
4. Input mahasiswa manual
5. Assign mentor
6. Monitoring absensi
7. Monitoring logbook
8. Kelola data master
9. Export laporan/nilai
10. Generate sertifikat (opsional)

## Daftar Kebutuhan Fungsional

1. Admin dapat CRUD periode magang (tanggal, kuota).
2. Admin dapat melihat detail pendaftaran dan berkas.
3. Admin dapat menerima/menolak pendaftaran dengan alasan.
4. Admin dapat menambahkan akun mahasiswa manual.
5. Admin dapat menetapkan mentor untuk mahasiswa aktif.
6. Admin dapat melihat rekap absensi harian.
7. Admin dapat melihat status validasi logbook.
8. Admin dapat export laporan ke PDF/Excel.

## Kriteria Penerimaan (Acceptance Criteria)

1. Pendaftaran berubah status dalam < 5 detik setelah keputusan admin.
2. Mahasiswa yang diterima wajib memiliki mentor sebelum status aktif final.
3. Dashboard admin menampilkan total mahasiswa aktif, pending validasi logbook, dan absensi hari ini.
4. Export laporan menghasilkan file yang dapat diunduh dan terbaca.

## Data yang Dibutuhkan

1. Data user admin
2. Data mahasiswa
3. Data mentor
4. Data periode magang
5. Data pendaftaran dan berkas
6. Data presensi
7. Data logbook
8. Data penilaian
9. Data sertifikat

## KPI Admin

1. Waktu rata-rata validasi pendaftaran
2. Persentase pendaftaran selesai divalidasi
3. Persentase mahasiswa ter-assign mentor
4. Ketepatan waktu publikasi laporan
