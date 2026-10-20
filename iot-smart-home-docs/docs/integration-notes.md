# Catatan Integrasi

Dokumen ini merangkum hal-hal teknis yang sering ditanyakan saat integrasi perangkat dengan platform kami.

## 1. Protokol yang Didukung

| Protokol | Digunakan untuk | Status | Catatan |
|----------|-----------------|:------:|---------|
| ONVIF | Discovery & kontrol kamera | TBD | Profil yang didukung: `TBD (S/T/G/M)` |
| RTSP | Streaming video | TBD | |
| HTTP/HTTPS API | Integrasi aplikasi | TBD | |
| P2P / Cloud | Pairing cepat | TBD | |
| SDK vendor | Fitur lanjutan | TBD | Vendor: `TBD` |

## 2. Kebutuhan Jaringan

| Item | Rekomendasi | Catatan |
|------|-------------|---------|
| Bandwidth per kamera | `TBD` | Tergantung resolusi/bitrate |
| Port yang perlu dibuka | `TBD` | |
| DHCP vs static IP | `TBD` | |
| NAT / firewall | `TBD` | |

## 3. Langkah Integrasi Umum (Eazy Gateway)

1. `TBD` — contoh: hubungkan gateway ke jaringan yang sama dengan kamera.
2. `TBD` — tambahkan kamera via ONVIF/RTSP.
3. `TBD` — verifikasi live view & playback.

## 4. Kompatibilitas Brand

| Brand | Metode integrasi | Status | Catatan |
|-------|------------------|:------:|---------|
| `[Brand A]` | ONVIF | TBD | |
| `[Brand B]` | RTSP | TBD | |
| `...` | | | |

## 5. Troubleshooting Cepat

| Gejala | Kemungkinan penyebab | Solusi |
|--------|----------------------|--------|
| Kamera tidak terdeteksi | Beda subnet / ONVIF off | `TBD` |
| Video putus-putus | Bandwidth kurang | `TBD` |
| Tanpa audio | Codec tidak didukung | `TBD` |
| `...` | | |
