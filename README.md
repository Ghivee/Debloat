# Debloat

Personal **Android TV / Google TV debloat setup** over ADB, built on top of the open-source
[cleanyourtv](https://github.com/Gathin23/cleanyourtv) project, with personal tweaks for my own TV.

This repository is my working copy: the `cleanyourtv/` folder contains the launcher, scripts, and
agent instructions, while the changes I use daily are committed here.

## What's inside

- `cleanyourtv/` — the full cleanyourtv source (launcher, `tools/` scripts, docs, and agent prompts).
- `cleanyourtv/AGENT_DEBLOAT_ANDROID_TV.md` — short, safe ADB debloat instructions for an AI agent.
- `cleanyourtv/launcher/app/src/main/res/values/config.xml` — my personal TV configuration.
- `screenshots/` — documentation screenshots.

## Personal changes

- Dock apps rearranged for my device (YouTube TV, Disney+, Hotstar).
- Custom tile labels for Disney+ and Hotstar.
- Extra agent instructions for a safe, reversible debloat workflow.

## Safety

The scripts only disable packages per user (`pm disable-user --user 0`); they do not uninstall,
root, or flash anything. Back up your package list before applying changes.

## Credits

Based on [Gathin23/cleanyourtv](https://github.com/Gathin23/cleanyourtv) (MIT License, Copyright (c) 2026 Gathin).
See `cleanyourtv/LICENSE` for the original license. My own modifications are released under the same terms.
