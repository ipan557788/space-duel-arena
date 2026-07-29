# 🚀 Space Duel Arena

Game 2D pertempuran luar angkasa, dibuat dengan **HTML5 Canvas + JavaScript murni** (tanpa library, tanpa build tools). Cukup 1 file `index.html` — langsung bisa dibuka di browser atau dihosting gratis lewat **GitHub Pages**.

## ✨ Fitur

- ⏱️ **Waktu** — tiap level punya batas waktu 45 detik.
- 📈 **Level** — 5 level dengan musuh yang makin cepat & makin sering menembak.
- 🔔 **Notifikasi** — pop-up di layar saat naik level, mulai game, dll.
- 🔊 **Suara** — efek suara tembak, kena hit, ledakan, naik level, menang/kalah (dibuat langsung lewat Web Audio API, jadi tidak perlu file audio eksternal).
- 🤖 **Musuh Komputer (AI)** — mode 1 pemain melawan CPU yang bisa mengejar & menghindar.
- 🎮 **Mode 2 Pemain** — main berdua di satu keyboard.
- 🌌 **Latar belakang animasi** — starfield berlapis (parallax) + nebula bergerak untuk kesan luar angkasa yang realistis.

## 🕹️ Kontrol

| Aksi | Player 1 | Player 2 |
|---|---|---|
| Gerak | W A S D | ↑ ↓ ← → |
| Tembak | Spasi | Enter |
| Kembali ke menu | Esc | Esc |

## ▶️ Cara Menjalankan

### Lokal
Cukup buka `index.html` langsung di browser (double click), atau jalankan server sederhana:
```bash
python3 -m http.server 8000
```
lalu buka `http://localhost:8000`.

### Deploy ke GitHub Pages
1. Buat repository baru di GitHub, upload file `index.html` (dan `README.md`) ke root repo.
2. Masuk ke **Settings → Pages**.
3. Pada **Source**, pilih branch `main` dan folder `/ (root)`.
4. Simpan — GitHub akan memberi URL seperti `https://username.github.io/nama-repo/`.
5. Game langsung bisa dimainkan online, tidak perlu server tambahan.

## 🧩 Struktur

```
├── index.html   # seluruh game (HTML + CSS + JS) dalam satu file
└── README.md
```

## 🛠️ Ide Pengembangan Lanjutan

- Tambah power-up (shield, tembakan ganda, heal).
- Simpan skor tertinggi di `localStorage`.
- Tambah lebih banyak jenis musuh / boss di level akhir.
- Ganti sprite ship dengan gambar/animasi sprite sheet untuk tampilan lebih detail.
- Versi mobile dengan tombol virtual (touch controls).
