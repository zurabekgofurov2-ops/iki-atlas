# Atlas by Iki — Windows installer

Atlas is an offline decision engine for companies: it reads your own data and the world around it — and tells you what to do while you still have time to choose. Everything runs on your computer; your data stays there.

**Website and demo video:** https://iki-atlas.vercel.app

## Download

The installer is published on the [Releases](https://github.com/zurabekgofurov2-ops/iki-atlas/releases) page:

- **Atlas-Setup.exe** — one file, ~0.7 GB: the app, an embedded Python and a local language model.
- **Atlas-Setup.torrent** — the same file via BitTorrent. It downloads even with no peers online: the file itself is the web seed.
- **SHA256SUMS.txt** — checksum. In PowerShell: `Get-FileHash .\Atlas-Setup.exe` must print the same value.

## Install

1. Run `Atlas-Setup.exe` and follow the wizard.
2. Windows SmartScreen may say "Windows protected your PC": the installer is not signed with a commercial certificate. Click **More info → Run anyway**.
3. Atlas appears on the desktop and in the Start menu; it is removed like any other program.

The first launch takes up to a minute (the engine warms up its screens).

**System:** Windows 10 or newer; .NET Framework 4 and WebView2 are already part of Windows.
**Local model:** a CPU with AVX2 (Core i3–i9, Ryzen) and 8 GB of RAM. Without them Atlas runs without the model and says so.

## Trial

This public build is a **trial: it works until 26 October 2026**. For a licence or a pilot on your own data — [Telegram](https://t.me/+998950213404) or zurabekgofurov2@gmail.com.

## Licences

- Atlas — © 2026 Iki. All rights reserved. The trial build may be installed and evaluated free of charge.
- Bundled local model **Qwen2.5-0.5B-Instruct** (GGUF, q4_k_m) — © 2024 Alibaba Cloud, Apache License 2.0: see [LICENSE-Qwen2.5.txt](LICENSE-Qwen2.5.txt).
- The embedded Python and its packages ship with their own licence files inside the installation folder (`.venv\Lib\site-packages\*.dist-info`).

---

**По-русски.** Атлас — офлайн-платформа решений для компаний: читает ваши данные и мир вокруг и говорит, что делать, пока есть время выбирать. Установщик — на странице [Releases](https://github.com/zurabekgofurov2-ops/iki-atlas/releases) (`Atlas-Setup.exe`, ~0,7 ГБ, или торрент). Если Windows покажет «Система Windows защитила ваш компьютер» — «Подробнее → Выполнить в любом случае». Пробная версия работает до 26 октября 2026 года.
