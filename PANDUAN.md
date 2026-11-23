# Kelana Jakarta di iPhone: panduan unggah

Isi folder ini (`web-iphone`) sudah siap diunggah apa adanya:
`index.html` (game v86), `manifest.webmanifest`, `sw.js`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`.
`PANDUAN.md` ini boleh ikut terunggah, tidak mengganggu.

## Pilihan A: Netlify (paling gampang)
1. Buka https://app.netlify.com/drop lalu daftar/masuk (bisa pakai akun GitHub atau email).
2. Seret folder `web-iphone` dari File Explorer ke kotak "Drag and drop your site output folder here".
3. Tunggu sampai muncul alamat seperti `https://nama-acak-123.netlify.app`. Itu link game-nya.
4. (Opsional) Site configuration > Change site name, misalnya `kelana-jakarta` → `https://kelana-jakarta.netlify.app`.
5. Update nanti: buka situsnya di Netlify > tab Deploys > seret lagi folder `web-iphone` ke kotak di bawah.

## Pilihan B: GitHub Pages
1. Masuk ke https://github.com, klik **New repository**, nama misalnya `kelana-jakarta`, pilih **Public**, klik Create.
2. Di halaman repo kosong, klik **uploading an existing file**, seret semua isi folder `web-iphone` (berkasnya, bukan foldernya), klik **Commit changes**.
   (Berkas `index.html` sekitar 5,5 MB, masih di bawah batas unggah 25 MB.)
3. Settings > Pages > Source: **Deploy from a branch**, Branch: `main`, folder `/ (root)`, klik Save.
4. Tunggu 1–2 menit, alamatnya muncul di atas halaman itu: `https://<username>.github.io/kelana-jakarta/`.

## Pasang di iPhone
1. Buka link tadi di **Safari** (harus Safari; di iOS lama, Chrome tidak bisa menambah ke layar utama).
2. Tunggu game terbuka sampai layar judul sekali (biar tersimpan untuk offline).
3. Ketuk tombol **Bagikan** (kotak dengan panah ke atas) > **Tambahkan ke Layar Utama** > **Tambah**.
4. Buka dari ikon Kelana Jakarta di layar utama, putar HP ke lanskap. Game tampil layar penuh tanpa bilah Safari dan tetap jalan tanpa internet.

## Catatan
- Suara baru bunyi setelah ketukan pertama, dan tidak bunyi kalau sakelar senyap (silent) iPhone sedang aktif.
- Simpanan game di layar utama **terpisah** dari simpanan di tab Safari. Mainnya dari ikon layar utama saja.
- Kalau ikon layar utama dihapus, simpanannya ikut hilang.
- Saat memperbarui game: ganti `index.html`, lalu naikkan nomor di baris `const VERSION = 'kelana-v86-1'` di `sw.js` (misalnya jadi `kelana-v87-1`), lalu unggah ulang. HP mengambil versi baru saat game dibuka dengan internet; kadang perlu ditutup dan dibuka sekali lagi.
