# Debloat

A personal Android TV / Google TV debloat setup over ADB, built on top of the open-source [cleanyourtv](https://github.com/Gathin23/cleanyourtv) project, with personal tweaks for the author's own TV. "Debloat" here means disabling the preinstalled apps and launcher noise that come with most smart TVs (tracking widgets, ad tiles, apps the owner never uses) without rooting the device or voiding its warranty.

[Baca dalam Bahasa Indonesia di bawah](#bahasa-indonesia)

## What's inside

This repository is the author's working copy of cleanyourtv, not a fork maintained for others: the `cleanyourtv/` folder holds the full upstream project (its launcher, `tools/` scripts, documentation and agent instructions), and the changes used on the author's own TV day to day are committed on top of it here.

- `cleanyourtv/` — the full cleanyourtv source: launcher, scripts, docs and agent prompts, unmodified except where noted below.
- `cleanyourtv/AGENT_DEBLOAT_ANDROID_TV.md` — short, safe ADB debloat instructions written for an AI agent to follow.
- `cleanyourtv/launcher/app/src/main/res/values/config.xml` — the author's personal TV configuration (which apps appear, in what order).
- `screenshots/` — documentation screenshots of the personal setup.

## Personal changes on top of cleanyourtv

- Dock apps rearranged for the author's own device (YouTube TV, Disney+, Hotstar).
- Custom tile labels for Disney+ and Hotstar.
- Extra agent instructions describing a safe, reversible debloat workflow, so an AI agent helping with ADB commands on this specific TV does not disable something that cannot be turned back on.

## Safety

The scripts only disable packages per user (`pm disable-user --user 0`), which Android treats as reversible: a disabled app can always be re-enabled from Settings or another `pm` command. Nothing here uninstalls system packages, roots the device, or flashes firmware. Even so, back up your current package list before applying any change, in case a particular TV's firmware behaves differently from the ones cleanyourtv was tested on.

## Credits

Based on [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) (MIT License, Copyright (c) 2026 Gathin). See `cleanyourtv/LICENSE` for the original license text. The author's own modifications on top of it are released under the same terms.

---

## Bahasa Indonesia

Setelan debloat Android TV / Google TV pribadi lewat ADB, dibangun di atas proyek open-source [cleanyourtv](https://github.com/Gathin23/cleanyourtv), dengan penyesuaian pribadi untuk TV milik penulis sendiri. "Debloat" di sini berarti mematikan aplikasi bawaan dan kebisingan launcher yang datang bersama kebanyakan smart TV (widget pelacak, tile iklan, aplikasi yang tidak pernah dipakai pemiliknya) tanpa melakukan root pada perangkat atau membatalkan garansinya.

### Isi

Repositori ini adalah salinan kerja penulis dari cleanyourtv, bukan fork yang dirawat untuk orang lain: folder `cleanyourtv/` menyimpan seluruh proyek upstream (launcher, skrip `tools/`, dokumentasi, dan instruksi agen), dan perubahan yang dipakai sehari-hari di TV penulis sendiri di-commit di atasnya di sini.

- `cleanyourtv/` — seluruh source cleanyourtv: launcher, skrip, dokumen, dan prompt agen, tidak diubah kecuali disebutkan di bawah.
- `cleanyourtv/AGENT_DEBLOAT_ANDROID_TV.md` — instruksi debloat ADB yang singkat dan aman, ditulis untuk diikuti agen AI.
- `cleanyourtv/launcher/app/src/main/res/values/config.xml` — konfigurasi TV pribadi penulis (aplikasi apa yang tampil, dalam urutan apa).
- `screenshots/` — tangkapan layar dokumentasi dari setelan pribadi ini.

### Perubahan pribadi di atas cleanyourtv

- Susunan aplikasi dock diatur ulang untuk perangkat penulis sendiri (YouTube TV, Disney+, Hotstar).
- Label tile khusus untuk Disney+ dan Hotstar.
- Instruksi tambahan untuk agen yang menjelaskan alur debloat yang aman dan bisa dibalik, sehingga agen AI yang membantu perintah ADB di TV ini tidak mematikan sesuatu yang tidak bisa dinyalakan lagi.

### Keamanan

Skrip hanya mematikan paket per pengguna (`pm disable-user --user 0`), yang oleh Android dianggap bisa dibalik: aplikasi yang dimatikan selalu bisa dinyalakan ulang dari Settings atau perintah `pm` lain. Tidak ada yang menghapus paket sistem, melakukan root perangkat, atau mem-flash firmware. Meski begitu, cadangkan daftar paket saat ini sebelum menerapkan perubahan apa pun, untuk jaga-jaga kalau firmware TV tertentu berperilaku berbeda dari yang sudah diuji cleanyourtv.

### Kredit

Berdasarkan [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) (Lisensi MIT, Hak Cipta (c) 2026 Gathin). Lihat `cleanyourtv/LICENSE` untuk teks lisensi aslinya. Modifikasi pribadi penulis di atasnya dirilis dengan ketentuan yang sama.
