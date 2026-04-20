# Matriks Asesmen Generator

Aplikasi web untuk generate jadwal wawancara asesmen otomatis.

## Setup (wajib sebelum deploy)

1. Download library SheetJS dari browser:
   👉 https://cdn.jsdelivr.net/npm/xlsx@0.18.5/dist/xlsx.full.min.js
2. Simpan file tersebut sebagai `xlsx.full.min.js` di folder ini
3. Struktur folder harus jadi:
   ```
   matriks-asesmen/
   ├── index.html
   ├── xlsx.full.min.js   ← hasil download
   ├── vercel.json
   └── README.md
   ```

## Deploy ke Vercel

### Cara 1 — Via GitHub (recommended)
1. Upload folder ini ke GitHub repository
2. Buka vercel.com → New Project → Import repo GitHub
3. Klik Deploy — selesai!

### Cara 2 — Via Vercel CLI
```bash
npm i -g vercel
cd matriks-asesmen
vercel
```

### Cara 3 — Drag & Drop
1. Buka vercel.com → Add New Project
2. Drag & drop folder `matriks-asesmen` ke halaman tersebut

## Fitur
- Upload data peserta, asesor, jadwal dari Excel
- Pengelompokan LGD otomatis (Statistisi/Pranata Komputer/Lainnya)
- Aturan slot mulai per range kelompok
- Assign asesor wawancara & partner otomatis
- Download hasil sebagai Excel (3 sheet: Matriks, Asesor, Peserta)
