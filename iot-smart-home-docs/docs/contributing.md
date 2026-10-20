# Cara Berkontribusi / Update Dokumentasi

## Alur Kerja (GitLab)

1. Buat branch: `docs/<platform>-<ringkasan>` (contoh: `docs/vms-cloud-retensi`).
2. Edit file terkait:
   - `capability-matrix.md` (selalu, bila status berubah)
   - file platform di `docs/platforms/`
   - `roadmap.md` bila menyentuh fitur 🔵
   - `changelog.md` (wajib)
3. Buka **Merge Request** ke `main`.
4. Minta approval dari **owner platform** terkait.
5. Setelah merge, update slide (`slides/sales-capability-deck.md`) bila relevan untuk sales.

## Definition of Done

- [ ] Status di matriks & file platform **konsisten**.
- [ ] Setiap status 🟡/🔴 punya **catatan** yang jelas.
- [ ] `changelog.md` diperbarui.
- [ ] Ikon status memakai legenda standar (✅ 🟡 🔴 🔵 ⚪).
- [ ] Tidak ada `TBD` baru tanpa penjelasan.

## Aturan Penulisan

- Bahasa: Indonesia, istilah teknis boleh Inggris.
- Satu sel matriks = satu status, tanpa paragraf.
- Cantumkan **versi build / hasil uji** sebagai bukti status.
- Jangan hapus riwayat; cukup ubah status + catat di changelog.

## Owner Platform

| Platform | Owner |
|----------|-------|
| Mobile Apps | `TBD` |
| Web Monitoring | `TBD` |
| VMS Heklix | `TBD` |
| VMS Cloud | `TBD` |
| Eazy Gateway | `TBD` |
