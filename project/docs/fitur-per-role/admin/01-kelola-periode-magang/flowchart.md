# Flowchart - Admin - Kelola Periode Magang

Fokus fitur ini hanya pada pengelolaan data periode magang oleh admin.

```mermaid
flowchart TD
	A([Start]) --> B[Admin login]
	B --> C[Buka menu kelola periode magang]
	C --> D{Pilih aksi}
	D -->|Tambah| E[Isi nama periode, tanggal mulai, tanggal selesai, kuota]
	D -->|Ubah| F[Pilih periode yang akan diubah]
	F --> G[Perbarui data periode]
	D -->|Hapus| H[Pilih periode yang akan dihapus]
	H --> I[Konfirmasi penghapusan]
	E --> J[Sistem validasi data periode]
	G --> J
	I --> J
	J --> K{Valid?}
	K -->|Tidak| L[Tampilkan pesan error]
	L --> D
	K -->|Ya| M[Sistem simpan perubahan]
	M --> N([End])
```

## Narasi Singkat

1. Admin mengelola periode magang melalui aksi tambah, ubah, atau hapus.
2. Sistem memvalidasi data sebelum perubahan disimpan.
3. Alur selesai saat data periode berhasil diperbarui.
