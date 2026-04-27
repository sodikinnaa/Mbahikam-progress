# PRD - Admin - Monitoring Logbook

## Tujuan Fitur
Menyediakan pemantauan logbook mahasiswa agar admin dapat melihat progres pelaporan kegiatan harian.

## Ruang Lingkup
Hanya mencakup dashboard status logbook, filter data, dan akses detail logbook.

## Pengguna
- Admin Kominfo

## Kebutuhan Fungsional
1. Admin dapat melihat dashboard status logbook seluruh mahasiswa.
2. Admin dapat memfilter logbook berdasarkan periode, mahasiswa, dan status validasi.
3. Sistem menampilkan status logbook: pending, disetujui, atau ditolak.
4. Admin dapat membuka detail logbook per mahasiswa.
5. Sistem menampilkan indikator logbook yang belum diisi atau menumpuk.

## Kebutuhan Non-Fungsional
1. Dashboard logbook harus menampilkan data secara konsisten sesuai filter.
2. Perubahan status logbook dari proses validasi harus tercermin pada dashboard.

## Acceptance Criteria
1. Dashboard menampilkan status logbook sesuai filter yang dipilih admin.
2. Admin dapat membuka detail logbook dari daftar monitoring.
3. Logbook yang belum diisi atau masih pending dapat diidentifikasi dengan jelas.
4. Data status yang tampil sama dengan status terakhir pada sistem.
