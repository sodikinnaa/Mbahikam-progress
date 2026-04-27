# PRD Cross-Role MAGIS

## Tujuan
Menetapkan kebutuhan lintas role agar alur antar Admin, Mentor, dan Mahasiswa berjalan sinkron.

## Ruang Lingkup
1. Status pendaftaran lintas Admin dan Mahasiswa.
2. Validasi logbook lintas Mentor dan Mahasiswa.
3. Monitoring lintas Admin terhadap data operasional.
4. Penilaian akhir lintas Mentor, Mahasiswa, dan Admin untuk pelaporan.

## Kebutuhan Fungsional
1. Sistem menyediakan status standar: pending, diterima, ditolak, disetujui, perlu revisi, selesai.
2. Setiap perubahan status harus terlihat oleh role terkait.
3. Data presensi, logbook, dan nilai dapat dipakai sebagai sumber laporan admin.
4. Sistem menerapkan kontrol akses berbasis role.

## Acceptance Criteria
1. Perubahan status dari satu role langsung terbaca pada dashboard role lain yang berhak.
2. Tidak ada konflik data antara modul pendaftaran, logbook, penilaian, dan laporan.
3. Laporan admin mencerminkan data terbaru dari seluruh role.
