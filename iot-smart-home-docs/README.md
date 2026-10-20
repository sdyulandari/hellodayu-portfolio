# Dokumentasi Kapabilitas Platform — Squad IoT Smart Home

> **Tujuan:** Sumber tunggal (*single source of truth*) yang menjelaskan **apa yang sudah bisa** dan **apa yang belum bisa** dilakukan oleh setiap platform kami terhadap produk/perangkat yang dijual.
>
> **Audiens:** Sales, Pre-Sales, Product, Support, dan tim teknis internal.
>
> **Status dokumen:** `TEMPLATE — data belum diisi`. Semua baris bertanda `TBD` wajib dikonfirmasi sebelum dipakai untuk presentasi ke customer.

---

## 1. Platform yang Dicakup

| # | Platform | Tipe | Fungsi Utama | Dokumen Detail |
|---|----------|------|--------------|----------------|
| 1 | Mobile Apps | Touch point customer | Kontrol & monitoring harian end-user | [platforms/mobile-app.md](docs/platforms/mobile-app.md) |
| 2 | Web Monitoring | Touch point customer | Monitoring kamera dengan tampilan lebih luas | [platforms/web-monitoring.md](docs/platforms/web-monitoring.md) |
| 3 | VMS Heklix | Command center (on-prem/desktop) | Manajemen multi-kamera skala besar | [platforms/vms-heklix.md](docs/platforms/vms-heklix.md) |
| 4 | VMS Cloud | Command center (cloud) | Manajemen terpusat berbasis cloud | [platforms/vms-cloud.md](docs/platforms/vms-cloud.md) |
| 5 | Eazy Gateway | Integrasi | Menghubungkan kamera existing/third-party | [platforms/eazy-gateway.md](docs/platforms/eazy-gateway.md) |

---

## 2. Struktur Repo

```
iot-smart-home-docs/
├── README.md                       # Halaman ini — entry point
├── docs/
│   ├── capability-matrix.md        # Matriks utama (device×platform & fitur×platform)
│   ├── platforms/                  # Detail per platform
│   │   ├── mobile-app.md
│   │   ├── web-monitoring.md
│   │   ├── vms-heklix.md
│   │   ├── vms-cloud.md
│   │   └── eazy-gateway.md
│   ├── integration-notes.md        # Protokol, ONVIF/RTSP, pairing, dsb.
│   ├── roadmap.md                  # Fitur yang "belum" + target versi
│   ├── glossary.md                 # Daftar istilah
│   ├── changelog.md                # Riwayat perubahan dokumen
│   └── contributing.md             # Cara update + review process
└── slides/
    └── sales-capability-deck.md    # Slide deck untuk tim Sales (Marp)
```

---

## 3. Legenda Status Dukungan

| Ikon | Status | Arti | Dipakai saat |
|------|--------|------|--------------|
| ✅ | **Full** | Didukung penuh & sudah diuji | Siap dijual tanpa catatan |
| 🟡 | **Partial** | Didukung dengan batasan | Siap dijual, wajib sebutkan limitasi |
| 🔴 | **Not Supported** | Belum didukung | Jangan janjikan ke customer |
| 🔵 | **Roadmap** | Dalam rencana / development | Boleh disebut sebagai "akan datang" |
| ⚪ | **N/A** | Tidak berlaku untuk platform tsb. | Netral |

> Konsisten gunakan ikon ini di seluruh dokumen & slide. Jangan menulis status dengan kata lain.

---

## 4. Cara Pakai per Tim

| Tim | Mulai dari | Untuk apa |
|-----|-----------|-----------|
| **Sales** | [slides/sales-capability-deck.md](slides/sales-capability-deck.md) | Presentasi cepat ke customer |
| **Pre-Sales / Teknis** | [docs/capability-matrix.md](docs/capability-matrix.md) → detail platform | Menjawab pertanyaan "bisa tidak?" |
| **Support** | Detail platform + [integration-notes.md](docs/integration-notes.md) | Troubleshooting & batasan |
| **Product** | [roadmap.md](docs/roadmap.md) | Perencanaan fitur |

---

## 5. Aturan Update

1. **Setiap fitur baru / perubahan** → update `capability-matrix.md`, file platform terkait, dan `changelog.md`.
2. **Jangan** mengubah status tanpa bukti uji → lampirkan versi build / hasil QA di kolom "Catatan".
3. Gunakan **Pull Request** ke GitLab (lihat [docs/contributing.md](docs/contributing.md)).
4. Setiap platform punya **owner** (lihat file platform masing-masing); owner wajib approve PR yang menyentuh platformnya.

---

## 6. Versi & Pemeliharaan

| Field | Nilai |
|-------|-------|
| Versi dokumen | `0.1.0 (template)` |
| Terakhir diperbarui | `YYYY-MM-DD` |
| Pemilik dokumen | `TBD — Squad IoT Smart Home` |
| Jadwal review | `Per rilis / kuartalan` |
