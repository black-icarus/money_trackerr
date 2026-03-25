# 💸 Dompet — Panduan Deploy PWA (Pemula-Friendly)

## 📁 File yang Kamu Miliki
```
index.html      ← Aplikasi utama (semua UI + logika)
manifest.json   ← Konfigurasi PWA (nama, ikon, warna)
sw.js           ← Service Worker (supaya bisa offline)
icon-192.png    ← Ikon aplikasi kecil
icon-512.png    ← Ikon aplikasi besar
vercel.json     ← Konfigurasi deploy Vercel
```

---

## 🚀 CARA DEPLOY KE VERCEL (Gratis, ~5 Menit)

### Langkah 1 — Buat akun GitHub
1. Buka https://github.com dan klik **Sign Up**
2. Daftar dengan email kamu (gratis)

### Langkah 2 — Upload file ke GitHub
1. Setelah login, klik tombol **+** di pojok kanan atas → **New repository**
2. Nama repository: `dompet-app` (atau bebas)
3. Pilih **Public**, lalu klik **Create repository**
4. Di halaman repository yang baru dibuat, klik **uploading an existing file**
5. **Drag & drop** semua 6 file di atas ke halaman itu
6. Scroll ke bawah, klik **Commit changes**

### Langkah 3 — Deploy ke Vercel
1. Buka https://vercel.com dan klik **Sign Up**
2. Pilih **Continue with GitHub** → izinkan akses
3. Di dashboard Vercel, klik **Add New → Project**
4. Temukan repository `dompet-app` kamu, klik **Import**
5. Di halaman konfigurasi, **langsung klik Deploy** (tidak perlu ubah apapun)
6. Tunggu ~30 detik... ✅ **Selesai!**
7. Vercel akan memberimu URL seperti: `https://dompet-app.vercel.app`

---

## 📱 CARA INSTALL DI HP (Jadikan Ikon Aplikasi)

### Di iPhone/iPad (iOS 16.4+):
1. Buka Safari (HARUS Safari, bukan Chrome)
2. Ketuk URL dari Vercel kamu
3. Ketuk ikon **Share** (kotak dengan panah ke atas) di bagian bawah
4. Scroll dan pilih **"Add to Home Screen"** / "Tambahkan ke Layar Utama"
5. Ketuk **Add** / "Tambahkan"
6. Ikon 💸 Dompet akan muncul di Home Screen!

### Di Android:
1. Buka Chrome
2. Ketuk URL dari Vercel kamu
3. Akan muncul banner **"Add to Home Screen"** secara otomatis — ketuk **Install**
4. Atau: ketuk menu ⋮ (3 titik) di pojok kanan atas → **"Add to Home Screen"**
5. Ketuk **Add** / "Tambahkan"
6. Ikon 💸 Dompet akan muncul di Home Screen!

---

## 🔒 Tentang Data
- Semua data tersimpan di **LocalStorage browser HP kamu**
- Data **TIDAK dikirim ke server manapun** — 100% privat
- Data tetap ada selama kamu tidak hapus cache browser
- Untuk backup: di masa depan bisa ditambahkan fitur export CSV

---

## 🛠️ Cara Update Aplikasi
1. Edit file `index.html` di GitHub langsung (klik file → ikon pensil)
2. Vercel akan otomatis re-deploy dalam ~30 detik

---

## ❓ FAQ

**Q: Apakah bisa dipakai offline?**
A: Ya! Setelah pertama kali dibuka saat ada internet, aplikasi bisa dipakai offline sepenuhnya.

**Q: Data aman tidak jika HP diganti?**
A: Karena data di LocalStorage, perlu export dulu. Hubungi developer untuk fitur backup cloud.

**Q: Bisa tambah kategori baru?**
A: Edit bagian `BUDGET` dan `CATNAME` di `index.html`.

---

Dibuat dengan ❤️ — Tech Stack: Vanilla HTML/CSS/JS + PWA (Service Worker + Web Manifest)
