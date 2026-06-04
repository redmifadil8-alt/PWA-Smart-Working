# ✅ Smart Task Manager & Life Control

Aplikasi produktivitas pribadi berbasis PWA (Progressive Web App) yang berjalan **100% offline** tanpa memerlukan akun atau koneksi internet. Semua data tersimpan secara lokal di perangkat Anda menggunakan IndexedDB.

## 🚀 Live Demo

Akses aplikasi langsung di browser:  
**https://username.github.io/smart-task-manager/**

*(Ganti `username` dengan username GitHub Anda)*

## 📱 Fitur

| Modul | Deskripsi |
|-------|-----------|
| 📊 **Dashboard** | Ringkasan produktivitas, Productivity Score, tugas & habit hari ini |
| ✅ **Task Manager** | CRUD tugas, 4 prioritas, deadline, status tracking, filter & arsip |
| 🔥 **Habit Tracker** | Daily check, streak counter, icon picker |
| 📅 **Kalender** | Bulanan, navigasi, agenda harian dengan indikator event |
| ⏱️ **Pomodoro** | 3 mode timer (Focus 25m / Short 5m / Long 15m), statistik fokus |
| 🎯 **Goals** | Target harian/mingguan/bulanan/tahunan dengan progress bar |
| 💰 **Keuangan** | Catat pemasukan & pengeluaran, 9 kategori, saldo otomatis |
| 📝 **Catatan** | Quick Notes & Checklist |
| 📈 **Analitik** | Tasks per kategori, produktivitas mingguan, best/worst habits |
| 📋 **Review** | Evaluasi mingguan/bulanan, Export/Import JSON |

## 🛠️ Teknologi

- **Frontend:** HTML5, CSS3, JavaScript ES6+
- **Storage:** IndexedDB (lokal, tanpa server)
- **Offline:** Service Worker + Cache Storage API
- **Deploy:** GitHub Pages

## 📦 Struktur Folder

```
smart-task-manager/
├── index.html          # Aplikasi utama (SPA)
├── manifest.json       # Konfigurasi PWA
├── service-worker.js   # Offline caching
└── README.md           # Dokumentasi ini
```

## 🚀 Deploy ke GitHub Pages

### Langkah 1: Buat Repository
1. Login ke [GitHub](https://github.com)
2. Klik tombol **New Repository** (+
3. Isi nama repository: `smart-task-manager`
4. Pilih **Public**
5. Klik **Create repository**

### Langkah 2: Upload File

**Opsi A: Via GitHub Web (Cepat)**
1. Di halaman repository, klik **"Add file" → "Upload files"**
2. Upload ketiga file: `index.html`, `manifest.json`, `service-worker.js`
3. Klik **"Commit changes"**

**Opsi B: Via Git Command Line**
```bash
# Clone repository (ganti username)
git clone https://github.com/username/smart-task-manager.git
cd smart-task-manager

# Copy file ke folder ini, lalu:
git add .
git commit -m "Initial commit: Smart Task Manager PWA"
git push origin main
```

### Langkah 3: Aktifkan GitHub Pages
1. Di repository, klik tab **Settings**
2. Scroll ke bawah ke bagian **Pages**
3. Di "Source", pilih branch **`main`** (atau `master`)
4. Klik **Save**
5. Tunggu 1-2 menit, lalu akses: `https://username.github.io/smart-task-manager/`

### Langkah 4: Install PWA di HP
1. Buka URL di Chrome/Android Browser
2. Tap menu **⋮ → "Add to Home screen"** (atau **"Install app"**)
3. Aplikasi akan terinstall seperti app native!

## 🔄 Backup & Restore Data

- **Export:** Buka menu **Review → Export JSON** untuk backup data
- **Import:** Buka menu **Review → Import JSON** untuk restore/pindah perangkat

## 🎨 Custom Domain (Opsional)

Jika ingin pakai domain sendiri:
1. Di repository, buat file `CNAME` dengan isi: `nama-domain-anda.com`
2. Atur DNS di provider domain Anda (CNAME ke `username.github.io`)
3. Aktifkan HTTPS di Settings → Pages → Enforce HTTPS

## ⚠️ Catatan Penting GitHub Pages

| Perhatian | Penjelasan |
|-----------|------------|
| **Path Relatif** | Semua file menggunakan `./` (bukan `/`) agar kompatibel dengan subdirectory GitHub Pages |
| **HTTPS Wajib** | Service Worker hanya berjalan di HTTPS — GitHub Pages otomatis menyediakan ini |
| **Trailing Slash** | Akses URL dengan trailing slash `/` di akhir untuk memastikan Service Worker aktif |
| **Cache Update** | Jika ada update, ubah `CACHE_NAME` di `service-worker.js` (misal: `v2`) lalu push ulang |

## 📄 Lisensi

MIT License — Bebas digunakan, dimodifikasi, dan didistribusikan.

---

**Dibuat dengan ❤️ untuk produktivitas Indonesia**
