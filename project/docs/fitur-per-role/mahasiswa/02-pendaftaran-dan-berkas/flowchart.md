# Flowchart - Mahasiswa - Pendaftaran dan Berkas

Fokus fitur ini hanya pada pengajuan pendaftaran dan kelengkapan berkas.

```mermaid
flowchart TD
	A([Start]) --> B[Mahasiswa buka menu pendaftaran]
	B --> C[Pilih periode magang]
	C --> D[Upload berkas: CV, surat pengantar, transkrip, proposal opsional]
	D --> E[Sistem validasi tipe dan ukuran file]
	E --> F{Valid?}
	F -->|Tidak| G[Tampilkan pesan error per berkas]
	G --> D
	F -->|Ya| H[Simpan berkas pendaftaran]
	H --> I[Mahasiswa submit pendaftaran]
	I --> J[Sistem set status pendaftaran: Pending]
	J --> K([End: Menunggu validasi admin])
```

## Narasi Singkat

1. Mahasiswa memilih periode dan mengunggah berkas syarat.
2. Sistem memvalidasi berkas sebelum pendaftaran bisa dikirim.
3. Setelah submit, status pendaftaran menjadi Pending.
