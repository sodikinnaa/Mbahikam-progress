# Flowchart - Admin - Input Mahasiswa Manual

Fokus fitur ini hanya pada input mahasiswa jalur manual oleh admin.

```mermaid
flowchart TD
	A([Start]) --> B[Admin buka menu input mahasiswa manual]
	B --> C[Isi data mahasiswa: identitas, kampus, prodi, kontak]
	C --> D[Sistem validasi kelengkapan data]
	D --> E{Data valid?}
	E -->|Tidak| F[Tampilkan error dan minta perbaikan]
	F --> C
	E -->|Ya| G[Sistem buat akun mahasiswa]
	G --> H[Sistem set status akun awal]
	H --> I[Sistem tampilkan atau kirim kredensial awal]
	I --> J([End])
```

## Narasi Singkat

1. Admin memasukkan data mahasiswa yang tidak melalui registrasi mandiri.
2. Sistem memvalidasi data lalu membuat akun mahasiswa.
3. Kredensial awal disediakan agar mahasiswa dapat login.
