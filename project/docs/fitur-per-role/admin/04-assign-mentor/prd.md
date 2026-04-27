# PRD - Admin - Assign Mentor

## Tujuan Fitur
Memastikan setiap mahasiswa aktif memiliki mentor yang ditetapkan oleh admin.

## Ruang Lingkup
Hanya mencakup proses pemilihan mahasiswa, pemilihan mentor, dan penyimpanan relasi pembimbing.

## Pengguna
- Admin Kominfo

## Kebutuhan Fungsional
1. Admin dapat melihat daftar mahasiswa yang membutuhkan mentor.
2. Admin dapat melihat daftar mentor yang tersedia.
3. Admin dapat memilih mentor untuk mahasiswa tertentu.
4. Sistem memvalidasi bahwa mentor dapat ditugaskan.
5. Sistem menyimpan relasi mentor-mahasiswa.
6. Sistem menampilkan hasil assignment yang berhasil.

## Kebutuhan Non-Fungsional
1. Proses assignment harus sederhana dan dapat dilakukan dalam satu halaman.
2. Data assignment harus langsung terlihat pada profil mahasiswa.

## Acceptance Criteria
1. Saat admin memilih mentor valid, relasi mentor-mahasiswa tersimpan.
2. Data mentor yang dipilih muncul pada detail mahasiswa.
3. Jika mentor tidak tersedia, sistem menolak penyimpanan dan menampilkan pesan.
4. Riwayat assignment tercatat dengan waktu dan admin pelaku.
