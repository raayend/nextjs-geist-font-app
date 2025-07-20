# Survey Application - Setup Guide

## 📥 Cara Import ke VS Code Anda

### Metode 1: Download ZIP (Recommended)
1. **Download file**: `survey-app.zip` (sudah dibuat di folder project)
2. **Extract file** di laptop Anda
3. **Buka VS Code**
4. **File → Open Folder** → Pilih folder hasil extract

### Metode 2: Copy Paste Manual
1. **Buat folder baru** di laptop Anda: `survey-app`
2. **Copy semua file** dari project ini
3. **Paste ke folder baru**
4. **Buka folder** dengan VS Code

## 🚀 Setup di Laptop Anda

### Prerequisites (Pastikan sudah terinstall):
- **Node.js** (versi 18 atau lebih baru)
- **VS Code** (text editor)
- **Git** (optional, untuk version control)

### Langkah Setup:

1. **Buka Terminal di VS Code**
   - Tekan `Ctrl + ~` atau
   - View → Terminal

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Jalankan Development Server**
   ```bash
   npm run dev
   ```

4. **Buka di Browser**
   - Akses: `http://localhost:3000`

## 📋 Login Credentials

- **Admin Login**: 
  - Username: `admin`
  - Password: `admin123`

## 🎯 Fitur Aplikasi

1. **Survey Kepuasan** - Untuk publik mengisi survey
2. **Admin Dashboard** - Untuk melihat hasil survey
3. **Export Data** - Export ke Excel/PDF
4. **Reset Data** - Hapus semua data survey

## 🔧 Troubleshooting

### Jika ada error:
1. **Delete folder `node_modules`**
2. **Delete file `package-lock.json`**
3. **Run ulang**: `npm install`
4. **Run**: `npm run dev`

### Port 3000 sudah digunakan:
```bash
npm run dev -- -p 3001
```

## 📁 Struktur Folder

```
survey-app/
├── src/
│   ├── app/
│   │   ├── page.tsx          # Halaman utama
│   │   ├── survey/page.tsx   # Halaman survey
│   │   ├── admin/
│   │   │   ├── page.tsx      # Dashboard admin
│   │   │   └── login/page.tsx # Login admin
│   │   └── api/survey/route.ts # API endpoints
├── public/                   # Assets
├── package.json             # Dependencies
└── README.md               # Dokumentasi
```

## 🎨 Customisasi

### Ubah Warna:
Edit file `tailwind.config.js` untuk mengubah tema warna

### Ubah Logo:
Ganti file di folder `public/` dengan logo Anda

### Ubah Text:
Edit file `.tsx` sesuai kebutuhan Anda

## 📞 Support

Jika ada masalah, cek:
1. Console log di browser (F12)
2. Terminal di VS Code untuk error messages
3. Pastikan semua dependencies terinstall dengan benar
