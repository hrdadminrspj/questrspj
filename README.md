# 🎮 Premier Jatinegara Memory Quest

Game Memory Card untuk menemukan Supervisor kita!

![Game Preview](https://img.shields.io/badge/Game-Memory%20Quest-blueviolet)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🎯 Tentang Game

Game memory card interaktif dengan tema Premier Jatinegara. Cocokkan foto-foto untuk menang!

### ✨ Fitur:
- 🎮 3 Tingkat Kesulitan (Mudah, Sedang, Sulit)
- 🏆 Sistem Scoring dengan Combo Bonus
- ⏱️ Timer dan Counter Gerakan
- 🎨 Animasi dan Efek Visual Menarik
- 🔊 Sound Effects
- 📱 Responsive (Desktop & Mobile)

## 🚀 Cara Setup di GitHub Pages

### Langkah 1: Upload ke GitHub

1. **Buat Repository Baru** di GitHub:
   - Klik tombol `New Repository`
   - Beri nama, misalnya: `premier-memory-quest`
   - Pilih `Public`
   - Centang `Add a README file`
   - Klik `Create repository`

2. **Upload File:**
   - Klik tombol `Add file` → `Upload files`
   - Upload file-file berikut:
     - `index.html` (rename dari `premier-jatinegara-memory-quest.html`)
     - `Poto1.jpg` sampai `Poto18.jpg`
   - Klik `Commit changes`

### Langkah 2: Struktur Repository

Repository Anda harus terlihat seperti ini:

```
📁 premier-memory-quest/
  ├── index.html          ← File game (wajib nama index.html)
  ├── Poto1.jpg
  ├── Poto2.jpg
  ├── Poto3.jpg
  ├── Poto4.jpg
  ├── Poto5.jpg
  ├── Poto6.jpg
  ├── Poto7.jpg
  ├── Poto8.jpg
  ├── Poto9.jpg
  ├── Poto10.jpg
  ├── Poto11.jpg
  ├── Poto12.jpg
  ├── Poto13.jpg
  ├── Poto14.jpg
  ├── Poto15.jpg
  ├── Poto16.jpg
  ├── Poto17.jpg
  ├── Poto18.jpg
  └── README.md
```

### Langkah 3: Aktifkan GitHub Pages

1. Di repository, klik tab `Settings`
2. Scroll ke bawah, cari menu `Pages` di sidebar kiri
3. Di bagian `Source`, pilih `main` branch
4. Klik `Save`
5. Tunggu beberapa menit
6. URL game Anda akan muncul, contoh:
   ```
   https://[username].github.io/premier-memory-quest/
   ```

## ⚠️ TROUBLESHOOTING - Foto Tidak Muncul di GitHub Pages

### Problem 1: Nama File Tidak Persis (Case Sensitive)

GitHub Pages **sangat sensitif** terhadap huruf besar/kecil!

❌ **SALAH:**
- `poto1.jpg` (huruf p kecil)
- `Poto1.JPG` (ekstensi JPG kapital)
- `Photo1.jpg` (kata berbeda)
- `Poto 1.jpg` (ada spasi)

✅ **BENAR:**
- `Poto1.jpg` (P besar, o kecil, .jpg kecil)
- `Poto2.jpg`
- ... dst

### Problem 2: Format File Foto

Pastikan foto Anda:
- ✅ Format: `.jpg` (lowercase)
- ✅ Ukuran: Maksimal 1MB per foto (untuk loading cepat)
- ✅ Dimensi: Idealnya 500x500px atau 800x800px (persegi)

### Problem 3: Lokasi File

Semua foto harus di **root folder** (folder utama) yang sama dengan `index.html`

### Cara Cek Apakah Foto Sudah Benar:

1. Buka repository GitHub Anda
2. Klik salah satu foto, misal `Poto1.jpg`
3. Klik tombol `Raw`
4. Jika foto muncul, berarti nama dan lokasi sudah benar
5. Copy URL-nya, contoh:
   ```
   https://raw.githubusercontent.com/username/repo/main/Poto1.jpg
   ```

## 🔧 Solusi Jika Foto Tetap Tidak Muncul

### Solusi 1: Gunakan Subfolder `images/`

Ubah struktur menjadi:

```
📁 premier-memory-quest/
  ├── index.html
  ├── images/
  │   ├── Poto1.jpg
  │   ├── Poto2.jpg
  │   └── ... (semua foto di sini)
  └── README.md
```

Lalu edit file `index.html`, cari bagian ini:

```javascript
const photoSets = {
    easy: [
        'Poto1.jpg', 'Poto2.jpg', // dst...
```

Ubah menjadi:

```javascript
const photoSets = {
    easy: [
        'images/Poto1.jpg', 'images/Poto2.jpg', // dst...
```

### Solusi 2: Rename File HTML

File HTML **HARUS** bernama `index.html` (bukan nama lain) agar GitHub Pages bisa mendeteksi.

### Solusi 3: Gunakan Developer Tools untuk Debug

1. Buka game di browser
2. Tekan `F12` atau klik kanan → `Inspect`
3. Buka tab `Console`
4. Lihat error message, biasanya menunjukkan file mana yang tidak ditemukan
5. Periksa apakah nama file di error sama persis dengan file di GitHub

### Solusi 4: Hard Refresh

Setelah upload/update file:
- Windows: `Ctrl + Shift + R`
- Mac: `Cmd + Shift + R`

Atau buka mode Incognito/Private untuk memastikan tidak ada cache.

## 📝 Checklist Upload ke GitHub

- [ ] File HTML sudah di-rename menjadi `index.html`
- [ ] Semua 18 foto sudah di-upload
- [ ] Nama foto persis: `Poto1.jpg` - `Poto18.jpg` (P besar, .jpg kecil)
- [ ] Semua file di root folder (atau semua foto di subfolder `images/`)
- [ ] GitHub Pages sudah diaktifkan di Settings
- [ ] Sudah tunggu 2-5 menit setelah upload
- [ ] Sudah coba hard refresh browser (Ctrl+Shift+R)

## 🎮 Cara Bermain

1. Pilih tingkat kesulitan:
   - **Mudah (4x4)** = 16 kartu
   - **Sedang (6x6)** = 36 kartu  
   - **Sulit (8x4)** = 32 kartu

2. Klik **Mulai Game**
3. Klik kartu untuk membuka
4. Cocokkan pasangan foto yang sama
5. Selesaikan semua pasangan untuk menang!

## 🏆 Sistem Scoring

- Match berhasil = **+100 poin**
- Bonus Kombo = **+50 poin** per kombo
- Bonus Waktu = Semakin cepat, semakin banyak poin

## 🛠️ Teknologi

- HTML5
- CSS3 (Animations & Transitions)
- Vanilla JavaScript
- Web Audio API (Sound Effects)

## 📱 Browser Support

- ✅ Chrome
- ✅ Firefox
- ✅ Edge
- ✅ Safari
- ✅ Opera

## 📄 License

© 2026 Premier Jatinegara. All rights reserved.

---

## 🆘 Butuh Bantuan?

Jika masih ada masalah:

1. **Periksa Console di Browser** (tekan F12)
2. **Cek nama file di GitHub** - harus persis sama
3. **Tunggu beberapa menit** setelah upload
4. **Clear cache browser** atau gunakan Incognito mode

---

**Dibuat dengan ❤️ untuk Premier Jatinegara**
