# AIT Internal Hub — Unofficial Edition

> ⚠️ **DISCLAIMER: Ini adalah halaman unofficial buatan Ancur Ini Tim. Bukan produk resmi Alpha Innovation Technology.**

One-page internal hub untuk tim AIT. Berisi link ke tools internal, profil tim, dan info singkat tentang AIT.

---

## 🚀 Live Site

Deploy via GitHub Pages:
`https://<username>.github.io/<repo-name>/`

---

## 📁 Struktur File

```
repo/
└── index.html   ← semua ada di sini (CSS, JS, SVG, animasi)
└── README.md
```

Satu file, no dependencies, no build step.

---

## 🛠️ Cara Deploy ke GitHub Pages

1. Upload `index.html` ke repo ini
2. Buka **Settings → Pages**
3. Source: **Deploy from a branch**
4. Branch: `main` → folder: `/ (root)`
5. Save → tunggu ~1 menit → live!

---

## ➕ Cara Tambah Tool Baru

Buka `index.html`, cari section `TOOLS`, copy salah satu blok `.tool-card` dan sesuaikan:

```html
<div class="tool-card reveal" data-url="https://link-tool-baru.com" onclick="launchTool(this)">
  <div class="tool-tag">AIT-xx</div>
  <div class="tool-name">Nama<br>Tool</div>
  <p class="tool-desc">Deskripsi singkat tool ini.</p>
  <div class="tool-features">
    <span class="tool-feature">Fitur 1</span>
    <span class="tool-feature">Fitur 2</span>
  </div>
  <div class="tool-cta">
    <span>Launch Tool</span>
    <div class="tool-cta-arrow">
      <svg width="14" height="14" viewBox="0 0 14 14" fill="none">
        <path d="M2 7h10M8 3l4 4-4 4" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </div>
  </div>
  <div class="tool-progress"></div>
</div>
```

---

## ➕ Cara Tambah Anggota Tim

Cari section `TEAM`, copy salah satu blok `.team-card`:

```html
<div class="team-card reveal" onclick="this.classList.toggle('flipped')">
  <div class="team-card-inner">
    <div class="team-front">
      <div class="team-avatar">XX</div>  <!-- inisial nama -->
      <div class="team-name">Nama</div>
      <div class="team-title-front">Role Keren</div>
    </div>
    <div class="team-back">
      <div class="team-role">Role<br>Keren</div>
      <p class="team-bio">Bio singkat orangnya.</p>
    </div>
  </div>
</div>
```

> Untuk perempuan, tambahkan class `female` pada `.team-avatar`:
> `<div class="team-avatar female">XX</div>`

---

## 🎨 Ganti Warna / Branding

Edit CSS variables di bagian `:root` dalam `index.html`:

```css
:root {
  --bg:          #080808;   /* background utama */
  --red:         #8B1A1A;   /* merah maroon */
  --red-bright:  #C0392B;   /* merah aksen */
  --white:       #F5F5F5;
}
```

---

## ✨ Fitur

- Logo SVG asli AIT dengan animasi assembly saat load
- Custom cursor segitiga merah
- Particle interaktif ngikutin mouse
- Hero title reveal per huruf
- Counter animasi stats
- Tool cards dengan launch animation
- Team cards flip on hover/tap
- Scroll reveal semua section
- Progress bar scroll
- Fully responsive (mobile & desktop)
- Noise texture overlay

---

## 👤 Built by

**Fadhil Ghifarion 法迪** — untuk Ancur Ini Tim 🔴

© 2026 Alpha Innovation Technology. Unofficial.
