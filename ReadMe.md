# Ruangan Interaktif — Full Features

Aplikasi visualisasi 3D interaktif berbasis browser untuk menjelajahi ruangan 3D dengan kontrol FPS, animasi, dan efek pencahayaan menggunakan Three.js.

## File

- index.html - File utama aplikasi
- NCC_ROOMS2.glb - Model 3D (~27MB)
- ReadMe.md - Dokumentasi ini
- libs/ - Library Three.js (mode offline)

## Library (libs/)
- three/three.module.js — Core Three.js
- three/addons/loaders/GLTFLoader.js — Loader model GLB
- three/addons/libs/lil-gui.module.min.js — Panel kontrol GUI

## Cara Pakai

### Manual dengan Three JS
npm install
npm install three 
npm run dev

# Buka browser: http://localhost:8080

### VS Code
Gunakan Live Server extension.

## Kontrol

| Tombol | Fungsi |
|--------|--------|
| LMB (tahan) | Putar kamera |
| W | Maju |
| S | Mundur |
| A | Kiri |
| D | Kanan |
| Space | Naik |
| Shift | Turun |
| P | Play/Pause animasi kursi |
| R | Reset animasi kursi |
| F | Senter on/off |

## Fitur GUI
Panel di kiri atas bisa diatur:
- Lingkungan — cahaya ambient, matahari
- Physics & Gerak — kecepatan, gravitasi, tinggi badan
- Head Bob — goyangan langkah saat berjalan
- Senter (Flashlight) — kekuatan, warna, sudut
- Lampu Ruangan — intensitas dan warna lampu
- Animasi Kursi — play/pause dan reset

## Mode Offline

Library Three.js sudah ada di folder libs/. Tidak perlu internet.

Catatan: Masih butuh HTTP server lokal (bukan file://) karena browser memblokir ES modules.

## Kustomisasi

Ganti model 3D: ganti file NCC_ROOMS2.glb
Ubah pengaturan: edit bagian settings di index.html

## Teknologi
- Three.js v0.160.0
- GLTFLoader
- lil-gui
- WebGL

---
*Dikembangkan untuk visualisasi 3D ruangan NCC_ROOMS.*
