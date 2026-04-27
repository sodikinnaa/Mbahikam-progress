# PRD - Admin - Validasi Pendaftaran

## Tujuan Fitur
Memastikan setiap pendaftaran mahasiswa divalidasi admin secara konsisten berdasarkan data dan berkas.

## Ruang Lingkup
Hanya mencakup proses review pendaftaran dan penetapan hasil validasi.

## Pengguna
- Admin Kominfo

## Kebutuhan Fungsional
1. Admin dapat melihat daftar pendaftaran masuk.
2. Admin dapat membuka detail data pendaftar.
3. Admin dapat melihat semua berkas syarat yang diunggah mahasiswa.
4. Admin dapat menetapkan keputusan diterima atau ditolak.
5. Sistem mewajibkan alasan penolakan saat status ditolak.
6. Sistem menyimpan riwayat keputusan validasi.

## Kebutuhan Non-Fungsional
1. Dokumen berkas harus dapat dibuka dengan cepat dari halaman validasi.
2. Data keputusan validasi harus tersimpan akurat tanpa duplikasi status.

## Acceptance Criteria
1. Saat admin memilih Diterima, status pendaftaran berubah menjadi Diterima.
2. Saat admin memilih Ditolak, sistem meminta alasan penolakan sebelum menyimpan.
3. Alasan penolakan tampil pada detail pendaftaran yang ditolak.
4. Riwayat waktu dan admin validator tercatat pada data pendaftaran.
