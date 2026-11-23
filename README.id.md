# Debloat

Setup **debloat Android TV / Google TV** pribadi lewat ADB, dibangun di atas proyek open-source
[cleanyourtv](https://github.com/Gathin23/cleanyourtv), dengan penyesuaian untuk TV saya sendiri.

Repositori ini adalah working copy saya: folder `cleanyourtv/` berisi launcher, script, dan instruksi
agent, sementara perubahan yang saya pakai sehari-hari di-commit di sini.

## Isi repositori

- `cleanyourtv/` — source lengkap cleanyourtv (launcher, script di `tools/`, dokumentasi, dan prompt agent).
- `cleanyourtv/AGENT_DEBLOAT_ANDROID_TV.md` — instruksi debloat ADB yang singkat dan aman untuk agent AI.
- `cleanyourtv/launcher/app/src/main/res/values/config.xml` — konfigurasi TV pribadi saya.
- `screenshots/` — screenshot dokumentasi.

## Penyesuaian pribadi

- Urutan dock apps disesuaikan dengan perangkat saya (YouTube TV, Disney+, Hotstar).
- Label tile khusus untuk Disney+ dan Hotstar.
- Instruksi agent tambahan untuk alur debloat yang aman dan bisa dibatalkan.

## Keamanan

Script hanya menonaktifkan paket per user (`pm disable-user --user 0`); tidak melakukan uninstall,
root, atau flashing. Backup daftar paket sebelum menerapkan perubahan.

## Kredit

Berdasarkan [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) (MIT License, Copyright (c) 2026 Gathin).
Lihat `cleanyourtv/LICENSE` untuk lisensi asli. Modifikasi saya dirilis dengan ketentuan yang sama.
