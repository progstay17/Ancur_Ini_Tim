<div align="center">

<img src="assets/ghifarion/repo-banner.svg" alt="AIT INTERNAL HUB — A focused home for tools, team links, and shared context." width="100%">

</div>

# AIT Internal Hub — Unofficial Edition

> ⚠️ **DISCLAIMER: Ini adalah halaman unofficial buatan Ancur Ini Tim. Bukan produk resmi Alpha Innovation Technology.**

One-page internal hub untuk tim AIT. Berisi link ke tools internal, profil tim, dan info singkat tentang AIT.

> **Ghifarion** · Engineering Intelligence. Building Legacy.

## On this page

- [Live site](#live-site)
- [File structure](#struktur-file)
- [Deploy](#cara-deploy-ke-github-pages)
- [Add tools](#cara-tambah-tool-baru)
- [Add team members](#cara-tambah-anggota-tim)
- [Branding](#ganti-warna--branding)
- [Features](#fitur)

---

## Live Site

Jika GitHub Pages diaktifkan untuk repository ini, alamat proyek biasanya:
`https://progstay17.github.io/Ancur_Ini_Tim/`

URL tersebut belum dianggap live sampai deployment dan pengaturan Pages diverifikasi.

## Struktur File

```
repo/
├── index.html   # Semua HTML, CSS, JS, SVG, dan animasi
└── README.md
```

Satu file, tanpa dependencies atau build step.

## Cara Deploy ke GitHub Pages

1. Upload `index.html` ke repo ini.
2. Buka **Settings → Pages**.
3. Source: **Deploy from a branch**.
4. Branch: `main` → folder: `/ (root)`.
5. Save, lalu tunggu deployment selesai dan verifikasi URL Pages.

## Cara Tambah Tool Baru

Buka `index.html`, cari section `TOOLS`, lalu salin salah satu blok `.tool-card` dan sesuaikan URL, nama, deskripsi, dan fiturnya.

Contoh struktur:

```html
<div class="tool-card reveal" data-url="https://link-tool-baru.com" onclick="launchTool(this)">
  <div class="tool-tag">AIT-xx</div>
  <div class="tool-name">Nama Tool</div>
  <p class="tool-desc">Deskripsi singkat tool ini.</p>
  <div class="tool-features">
    <span class="tool-feature">Fitur 1</span>
    <span class="tool-feature">Fitur 2</span>
  </div>
</div>
```

Pastikan URL yang ditambahkan benar dan memang boleh dibagikan kepada anggota tim.

## Cara Tambah Anggota Tim

Cari section `TEAM`, salin salah satu blok `.team-card`, lalu sesuaikan inisial, nama, role, dan bio. Untuk kartu dengan styling khusus, ikuti class yang sudah digunakan di `index.html`.

## Ganti Warna / Branding

Edit CSS variables di bagian `:root` dalam `index.html`. Variabel tema saat ini menggunakan warna gelap, maroon, merah aksen, dan putih. Ubah nilainya secara konsisten agar kontras teks tetap terbaca.

## Fitur

- Logo SVG dengan animasi saat halaman dimuat.
- Custom cursor dan particle interaktif.
- Hero title reveal per huruf.
- Animated stats counter.
- Tool cards dengan launch animation.
- Team cards yang dapat flip saat hover/tap.
- Scroll reveal, progress bar, dan noise texture.
- Layout responsif untuk mobile dan desktop.

## Built by

**Fadhil Ghifarion 法迪** — untuk Ancur Ini Tim.

© 2026 Alpha Innovation Technology. Unofficial.
