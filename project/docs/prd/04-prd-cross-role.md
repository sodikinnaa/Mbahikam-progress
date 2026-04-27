# PRD Cross-Role dan Integrasi Fitur

## Ringkasan
Dokumen ini menjelaskan fitur lintas role yang melibatkan lebih dari satu aktor.

## Fitur Cross-Role

1. Registrasi dan autentikasi berbasis role (RBAC)
2. Workflow validasi pendaftaran (Mahasiswa-Admin)
3. Workflow logbook harian (Mahasiswa-Mentor)
4. Monitoring operasional (Admin-Mentor)
5. Penilaian akhir (Mentor-Mahasiswa-Admin)
6. Pelaporan dan export (Admin)

## Dependensi Antar Role

1. Mahasiswa tidak dapat aktivitas harian sebelum status diterima admin.
2. Mentor tidak dapat menilai sebelum mahasiswa berada di bawah bimbingannya.
3. Nilai akhir dipublikasikan setelah validasi akhir selesai.

## Aturan Bisnis Kunci

1. Satu mahasiswa aktif terhubung ke satu mentor pada satu periode.
2. Satu logbook harian memiliki satu status validasi aktif.
3. Penilaian akhir terdiri dari empat aspek dan nilai akhir otomatis.
4. Sertifikat hanya terbit untuk mahasiswa dengan status selesai dan nilai final.

## Non-Fungsional Utama

1. Keamanan autentikasi dan otorisasi role.
2. Ketersediaan sistem pada jam kerja operasional.
3. Integritas data presensi, logbook, dan nilai.
4. Audit trail untuk perubahan status kritis.

## Risiko dan Mitigasi

1. Risiko: upload file besar gagal.
   Mitigasi: batas ukuran, validasi format, retry upload.
2. Risiko: keterlambatan validasi mentor.
   Mitigasi: dashboard antrean dan notifikasi.
3. Risiko: akun awal tidak aman.
   Mitigasi: wajib ganti password saat login pertama.
