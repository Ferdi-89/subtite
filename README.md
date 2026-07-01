# 💬 Percakapan Presenter

Website untuk menampilkan percakapan dalam format presentasi. Upload file Excel, TXT, atau JSON — langsung tampil sebagai chat bubble dengan fitur navigasi dan auto-play.

![Preview](preview.png)

## ✨ Fitur

- **Upload 3 format:** Excel (.xlsx/.xls), TXT, JSON
- **Drag & drop** file langsung
- **Tampilan chat bubble** dengan avatar warna-warni per speaker
- **Navigasi:** ⏮ ◀ ▶ ⏭ maju/mundur per pesan
- **Auto-play** dengan kecepatan bisa diatur (1-10 detik)
- **Mode fullscreen** untuk presentasi layar penuh
- **Shortcut keyboard** (← → navigasi, Spasi/Enter play, F fullscreen, Esc keluar)
- **Responsive** — desktop & mobile

## 📁 Format File

### JSON
```json
[
  { "speaker": "Andi", "text": "Halo Budi!" },
  { "speaker": "Budi", "text": "Hai Andi!" }
]
```

### TXT
```
Nama: Teks percakapan per baris
```

### Excel (.xlsx/.xls)
| Kolom A | Kolom B |
|---------|---------|
| Speaker | Teks |

> File contoh: `contoh-percakapan.json` dan `contoh-percakapan.txt`

## 🚀 Deploy ke Vercel

### Via GitHub (otomatis)

1. **Push ke GitHub:**
   ```bash
   git remote add origin https://github.com/username/nama-repo.git
   git add .
   git commit -m "Initial commit"
   git push -u origin main
   ```

2. **Deploy di Vercel:**
   - Buka [vercel.com](https://vercel.com) → Import Repository
   - Pilih repo ini → **Deploy**
   - Selesai! Vercel auto-detect ini static site

### Via Vercel CLI (manual)

```bash
npm i -g vercel
vercel login
vercel
```

## 🎯 Cara Pakai

1. Buka website
2. Upload file JSON/TXT/Excel, atau klik ganda area contoh untuk muat percakapan sampel
3. Navigasi manual atau tekan ▶ untuk auto-play
4. Tekan **F** atau klik ⛶ untuk mode fullscreen presentasi

## 🎹 Shortcut Keyboard

| Tombol | Aksi |
|--------|------|
| `→` / `Spasi` | Pesan berikutnya (atau stop auto-play) |
| `←` | Pesan sebelumnya |
| `Home` | Ke awal |
| `End` | Ke akhir |
| `Enter` | Play / Stop |
| `F` | Toggle fullscreen |
| `Esc` | Keluar fullscreen / stop play |

## 🛠 Teknologi

- HTML + CSS + JavaScript murni (single file)
- [SheetJS](https://sheetjs.com/) — parsing Excel
- Tidak perlu framework / build step
