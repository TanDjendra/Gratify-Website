# Gratify Website

Website pengenalan dan unduhan aplikasi musik [Gratify](https://github.com/TanDjendra/Gratify).
Dibuat dengan HTML, CSS, dan JavaScript tanpa langkah build.

## Isi website

- Logo Gratify hijau dan cuplikan asli aplikasi.
- Tampilan Now Playing sebagai fokus desktop, dengan galeri geser di ponsel.
- Fitur aplikasi, unduhan APK, panduan pemasangan, FAQ, dan dukungan.
- Halaman kebijakan privasi dan ketentuan penggunaan yang masih berstatus draf.

## Jalankan secara lokal

Dari folder repository:

```sh
python -m http.server 4173 --bind 127.0.0.1 --directory dist
```

Buka http://127.0.0.1:4173/. Seluruh file yang perlu dihosting ada di `dist/`.

## Struktur

```text
dist/
  index.html            Halaman utama
  styles.css            Gaya halaman utama
  showcase.css          Galeri cuplikan responsif
  app.js                Menu ponsel
  assets/               Logo dan cuplikan aplikasi
  privacy/index.html    Draf kebijakan privasi
  terms/index.html      Draf ketentuan penggunaan
```

## Pemeliharaan

Tautan APK di `dist/index.html` mengarah ke aset rilis resmi Gratify v2.1.5.
Perbarui tautannya saat rilis aplikasi berubah. Tautan catatan pembaruan
mengarah ke halaman rilis terbaru GitHub.

Untuk hosting statis, gunakan `dist` sebagai direktori publik; tidak diperlukan
instalasi dependensi atau perintah build. Domain yang direncanakan adalah
`gratify.web.id`. Konfigurasi akun hosting, DNS, dan kredensial tidak termasuk
repository ini.

Dokumen pada `/privacy/` dan `/terms/` tetap berstatus **draf untuk peninjauan**
hingga disetujui pemilik. Mengunggah source tidak mengubah status dokumen.

## Aset dan atribusi

Logo dan cuplikan layar berasal dari proyek Gratify. Desain mengambil referensi
visual Spotify; Gratify adalah proyek independen dan tidak berafiliasi dengan
Spotify, YouTube, atau Google. Karya pihak ketiga yang terlihat di cuplikan
aplikasi tetap merupakan milik pemegang hak masing-masing.

## Lisensi

GNU GPL v3, mengikuti lisensi repository aplikasi Gratify. Lihat [LICENSE](LICENSE).
