# MAGIS Project - Urutan Pengerjaan

Dokumen ini berisi daftar urutan kerja yang disarankan agar penyusunan dokumen MAGIS berjalan rapi dan konsisten.

## Urutan Tahap Pengerjaan

1. Pahami brief utama project.
2. Tetapkan scope sistem dan role utama.
3. Susun flow global sistem.
4. Susun flow role-based tingkat tinggi.
5. Susun PRD level role (Admin, Mentor, Mahasiswa, Cross-role).
6. Breakdown fitur per role.
7. Buat flowchart per fitur (1 fitur 1 flowchart).
8. Buat PRD per fitur (1 fitur 1 PRD).
9. Sinkronkan istilah status lintas role.
10. Review akhir konsistensi dokumen.

## Daftar Dokumen Inti (Dikerjakan Lebih Dulu)

1. docs/flowchart/01-global-flow.md
2. docs/flowchart/02-role-based-flow.md
3. docs/prd/01-prd-admin.md
4. docs/prd/02-prd-mentor.md
5. docs/prd/03-prd-mahasiswa.md
6. docs/prd/04-prd-cross-role.md

## Daftar Fitur per Role (Dikerjakan Setelah Dokumen Inti)

1. docs/fitur-per-role/admin
2. docs/fitur-per-role/mentor
3. docs/fitur-per-role/mahasiswa

## Aturan Pengerjaan Dokumen

1. Satu folder fitur hanya untuk satu fitur.
2. Setiap folder fitur wajib memiliki:
- flowchart.md
- prd.md
3. Flowchart ditulis dengan format Mermaid agar mudah dipreview.
4. PRD minimal berisi:
- Tujuan Fitur.
- Ruang Lingkup.
- Pengguna.
- Kebutuhan Fungsional.
- Kebutuhan Non-Fungsional.
- Acceptance Criteria.

## Checklist Selesai

1. Semua flowchart per fitur sudah fokus dan tidak melebar.
2. Semua PRD per fitur sudah sesuai scope.
3. Istilah status konsisten pada semua dokumen.
4. Dokumen siap untuk sesi review tim.

## Kondisi Struktur Saat Ini

1. docs/flowchart sudah tersedia dan berisi dokumen inti alur sistem.
2. docs/prd sudah tersedia dan berisi dokumen inti kebutuhan per role.
3. docs/fitur-per-role berisi detail flowchart dan PRD per fitur untuk Admin, Mentor, dan Mahasiswa.

## Urutan Eksekusi Praktis Tim

1. Review dokumen inti di docs/flowchart dan docs/prd.
2. Lanjut review detail per role di docs/fitur-per-role/admin.
3. Lanjut review detail per role di docs/fitur-per-role/mentor.
4. Lanjut review detail per role di docs/fitur-per-role/mahasiswa.
5. Lakukan sinkronisasi istilah status antar semua dokumen.
6. Finalisasi dokumen untuk sesi review dan implementasi.
