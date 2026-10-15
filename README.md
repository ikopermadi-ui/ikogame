# YorisGame

Satu halaman, dua game belajar pemrograman untuk anak SD. Halaman awal memilih:
- **Robo Labirin** (20 level): susun blok perintah, antar robot ke bendera. Dari urutan perintah, perulangan, kondisi, "selama", sampai labirin raksasa.
- **Arena Kode** (24 misi): game ala MOBA, tulis kode untuk hero. Blok lalu kode teks sungguhan, dengan kartu JPG pencapaian untuk dibagikan ke WhatsApp.

## Deploy ke GitHub Pages
1. Upload SEMUA isi folder `situs/` (index.html, sw.js, manifest.webmanifest, icon-*.png, folder fonts/) ke root repo.
2. Settings → Pages → Branch `main`, folder `/ (root)`.
3. Buka `https://USERNAME.github.io/NAMA-REPO/` di HP. Chrome Android: ⋮ → Tambahkan ke layar utama (bisa dipakai tanpa internet).

Tombol bagikan ke WhatsApp hanya jalan di alamat https. Semua kemajuan tersimpan di HP (localStorage).

## Mengubah game
Sumber ada di `sumber/`. `node build.js` membuat ulang `dist/` (isinya sama dengan `situs/`).
- Arena Kode: `src/` (`missions.js` berisi 24 misi; `node test/solutions.js` mengujinya).
- Robo Labirin: `robo/` (`logic.js` berisi 20 level; `node robo/test.js` mengujinya).
