# PRD Fitur Registrasi MAGIS (Mahasiswa)

## 1. Latar Belakang
Sesuai brief MAGIS, proses pendaftaran magang sebelumnya belum terintegrasi sehingga menyulitkan seleksi dan monitoring status peserta. Fitur registrasi diperlukan untuk menstandarkan proses onboarding mahasiswa melalui sistem web secara digital.

## 2. Tujuan Fitur
1. Menyediakan mekanisme registrasi mahasiswa yang terstruktur dan terdokumentasi.
2. Mendukung dua jalur registrasi: mandiri dan berbasis data instansi (admin-generated).
3. Memastikan data profil dan berkas pendaftaran lengkap sebelum proses validasi admin.
4. Menghasilkan status pendaftaran yang jelas: Pending, Diterima, Ditolak.

## 3. Ruang Lingkup
### In Scope
1. Registrasi mandiri mahasiswa.
2. Registrasi dari input admin (akun otomatis dibuat sistem).
3. Login mahasiswa setelah akun tersedia.
4. Pengisian profil magang.
5. Upload berkas persyaratan.
6. Submit pendaftaran dan perubahan status ke Pending.
7. Validasi admin dengan keputusan diterima/ditolak.

### Out of Scope
1. Presensi harian check-in/check-out.
2. Input logbook harian.
3. Penilaian akhir dan sertifikat.

## 4. Aktor
1. Mahasiswa Magang.
2. Admin Kominfo.

## 5. User Story
1. Sebagai mahasiswa, saya ingin membuat akun secara mandiri agar bisa mendaftar magang.
2. Sebagai admin, saya ingin membuat akun mahasiswa dari data instansi agar mahasiswa jalur khusus tetap terdaftar dalam sistem.
3. Sebagai mahasiswa, saya ingin mengisi profil dan upload berkas agar pendaftaran saya bisa diverifikasi.
4. Sebagai admin, saya ingin memvalidasi pendaftaran agar hanya peserta yang memenuhi syarat dapat diterima.

## 6. Alur Proses Singkat
1. Mahasiswa memilih jalur registrasi (mandiri atau akun dibuat admin).
2. Sistem membuat akun jika data valid.
3. Mahasiswa login.
4. Mahasiswa melengkapi profil dan upload berkas.
5. Mahasiswa submit pendaftaran.
6. Sistem set status Pending.
7. Admin validasi dan memberi keputusan Diterima/Ditolak.

## 7. Kebutuhan Fungsional
1. Sistem menyediakan form registrasi publik untuk mahasiswa.
2. Sistem memvalidasi data wajib: nama lengkap, email, NIM, universitas, password.
3. Sistem menolak registrasi jika format email tidak valid atau data wajib kosong.
4. Admin dapat input data mahasiswa dari panel admin.
5. Sistem dapat generate akun otomatis untuk jalur admin-generated.
6. Sistem mengizinkan mahasiswa login setelah akun aktif.
7. Sistem menyediakan form profil magang: universitas, program studi, nomor telepon, alamat, periode magang.
8. Sistem menyediakan upload berkas: CV, surat pengantar, transkrip, proposal (opsional).
9. Sistem mengubah status pendaftaran menjadi Pending saat mahasiswa submit.
10. Admin dapat menetapkan keputusan pendaftaran: Diterima atau Ditolak.
11. Jika ditolak, sistem menyimpan dan menampilkan alasan penolakan.
12. Jika diterima, sistem mengubah status mahasiswa menjadi Aktif.

## 8. Kebutuhan Non-Fungsional
1. Keamanan: password disimpan dalam bentuk hash, bukan plain text.
2. Otorisasi: akses fitur dibatasi berdasarkan role (admin/mahasiswa).
3. Usability: form registrasi dapat diakses di desktop dan mobile.
4. Reliabilitas: data registrasi dan berkas tidak hilang saat submit berhasil.
5. Validasi file: hanya format yang diizinkan (PDF/JPG/PNG) dan ukuran file dibatasi.

## 9. Aturan Bisnis
1. Mahasiswa tidak dapat lanjut ke tahap operasional magang jika status pendaftaran masih Pending atau Ditolak.
2. Keputusan validasi hanya dapat dilakukan oleh admin.
3. Mahasiswa wajib melengkapi data profil inti sebelum submit pendaftaran.
4. Satu pendaftaran terhubung dengan satu periode magang yang dipilih mahasiswa.

## 10. Data yang Dibutuhkan
1. Data akun user: id_user, nama_lengkap, username/email, password_hash, role.
2. Data mahasiswa: NIM, universitas, jurusan/prodi, nomor telepon, alamat, status_akun.
3. Data pendaftaran: id_pendaftaran, id_mahasiswa, id_periode, status, catatan_admin.
4. Data berkas: jenis_berkas, path_file, waktu_upload.

## 11. Acceptance Criteria
1. Mahasiswa dapat menyelesaikan registrasi mandiri jika semua data valid.
2. Sistem menampilkan error yang jelas jika ada data tidak valid atau belum lengkap.
3. Admin dapat membuat akun mahasiswa melalui jalur input manual.
4. Mahasiswa dapat login setelah akun berhasil dibuat.
5. Mahasiswa dapat submit pendaftaran setelah profil dan berkas minimum lengkap.
6. Status pendaftaran otomatis menjadi Pending setelah submit.
7. Admin dapat mengubah status pendaftaran menjadi Diterima atau Ditolak.
8. Jika Ditolak, alasan penolakan terlihat oleh mahasiswa.
9. Jika Diterima, status mahasiswa menjadi Aktif.

## 12. Dependensi
1. Modul autentikasi dan RBAC.
2. Modul manajemen periode magang.
3. Modul upload dan penyimpanan berkas.
4. Modul notifikasi (opsional untuk verifikasi email/kirim kredensial).

## 13. Risiko dan Mitigasi
1. Risiko data pendaftaran tidak lengkap.
	Mitigasi: validasi wajib pada sisi frontend dan backend.
2. Risiko duplikasi akun mahasiswa.
	Mitigasi: unique constraint pada email dan NIM.
3. Risiko kredensial awal bocor pada jalur admin-generated.
	Mitigasi: wajib ganti password pada login pertama.
