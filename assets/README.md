# 📁 ChirpDev — Asset Folder Guide

Taruh semua foto dan video kamu di sini sesuai folder-nya.

---

## 📂 Struktur Folder

```
assets/
├── images/
│   ├── projects/       ← Foto screenshot / thumbnail tiap project
│   │   ├── ara-space.jpg
│   │   ├── gold-ai-pro.jpg
│   │   ├── warungku.jpg
│   │   └── torai-cha-haus.jpg
│   │
│   ├── about/          ← Foto profil / foto kamu sendiri
│   │   └── profile.jpg
│   │
│   └── gallery/        ← Foto untuk accordion gallery section
│       ├── gallery-01.jpg
│       ├── gallery-02.jpg
│       ├── gallery-03.jpg
│       ├── gallery-04.jpg
│       └── gallery-05.jpg
│
└── videos/
    ├── projects/       ← Video demo tiap project (MP4)
    │   ├── ara-space-demo.mp4       ← Video Slot 1
    │   ├── gold-ai-pro-demo.mp4     ← Video Slot 2
    │   ├── warungku-demo.mp4        ← Video Slot 3
    │   └── torai-demo.mp4           ← Video Slot 4
    │
    └── hero/           ← (Opsional) Video background hero
        └── hero-bg.mp4
```

---

## 🔗 Cara Pasang ke HTML

### Pasang VIDEO project (ganti placeholder):
Cari `data-slot="video-1"` di HTML, lalu tambahkan video di dalamnya:

```html
<div class="frame__media" data-slot="video-1">
  <video src="assets/videos/projects/ara-space-demo.mp4" autoplay muted loop playsinline></video>
</div>
```

Lakukan hal yang sama untuk `video-2`, `video-3`, `video-4`.

### Pasang FOTO About:
Cari section `id="about"`, lalu di dalam `.frame__media`:

```html
<div class="frame__media">
  <img src="assets/images/about/profile.jpg" alt="ChirpDev" />
</div>
```

### Pasang FOTO Gallery (Accordion):
Cari `.acc__item` di HTML, lalu tambahkan img tag di dalam tiap item:

```html
<div class="acc__item">
  <img src="assets/images/gallery/gallery-01.jpg" alt="Project 01" />
  ...
</div>
```

---

## 📌 Tips Format File

| Jenis   | Format | Ukuran Ideal |
|---------|--------|--------------|
| Foto    | .jpg / .webp | Maks 500KB per file |
| Video   | .mp4 (H.264) | Maks 10MB per file |
| Profil  | .jpg / .webp | 800×1000px (portrait) |
| Gallery | .jpg / .webp | 900×600px (landscape) |

