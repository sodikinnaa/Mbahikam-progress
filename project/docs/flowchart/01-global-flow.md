# Flowchart Global MAGIS

## Tujuan
Mendefinisikan alur utama sistem dari pendaftaran hingga penilaian akhir dan sertifikat.

## Start-End Flow

1. Start
2. Mahasiswa registrasi (mandiri) atau akun dibuat admin
3. Mahasiswa login
4. Mahasiswa lengkapi profil dan upload berkas
5. Mahasiswa submit pendaftaran
6. Admin validasi pendaftaran
7. Keputusan pendaftaran:
   - Jika ditolak: status Ditolak, proses selesai
   - Jika diterima: status Aktif, lanjut assign mentor
8. Admin assign mentor
9. Mahasiswa menjalani aktivitas harian (loop per hari):
   - Check-in presensi (selfie, timestamp, opsional GPS)
   - Input logbook + upload bukti
   - Mentor validasi logbook
   - Jika ditolak mentor: mahasiswa revisi logbook
   - Jika disetujui mentor: lanjut check-out
   - Check-out presensi
10. Akhir periode:
    - Mahasiswa upload laporan akhir
    - Mentor input penilaian aspek
    - Sistem hitung nilai akhir otomatis
11. Admin generate laporan / export PDF
12. (Opsional) Sistem generate sertifikat + QR
13. End

## Keputusan Kritis

1. Validasi pendaftaran oleh admin
2. Validasi logbook oleh mentor
3. Kelengkapan laporan akhir sebelum penilaian final

## Data yang Terlibat

1. User dan role
2. Pendaftaran dan berkas
3. Periode magang
4. Presensi harian
5. Logbook harian
6. Penilaian akhir
7. Laporan akhir
8. Sertifikat
