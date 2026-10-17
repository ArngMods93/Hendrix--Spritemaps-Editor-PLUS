<div align="center">

<img src="icon-512.png" alt="Hendrix's Spritemaps Editor PLUS" width="128">

# Hendrix's Spritemaps Editor PLUS

**A web-based Spritemaps editor made specifically for Friday Night Funkin' (FNF).**
Edit, repack and manage your Spritemaps straight from the browser, no install needed.

![HTML](https://img.shields.io/badge/HTML-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![PWA](https://img.shields.io/badge/PWA-installable-5A0FC8?logo=pwa&logoColor=white)
![Fork](https://img.shields.io/badge/fork%20of-Hendrix--Spritemaps--editor--%20-7c2c44)

</div>

---

## About

**Hendrix's Spritemaps Editor PLUS** is an improved fork of [Hendrix's Spritemaps Editor](https://github.com/hendrixfunker053/Hendrix-Spritemaps-editor-). It is a tool for FNF modders who work with Spritemaps exported from **V-Slice** and **Better TA**, letting you open, visualize, rename and repack them without any extra software.

It runs entirely in your browser: your files are processed locally and never uploaded anywhere.

## Features

- **Repack Spritemaps** made with Adobe Animate / Better TA, either as frames or as `.XML`
- **Create Spritemaps** by importing your own frames
- **Visualize** your Spritemaps right in the editor
- **Select and rename** sprites
- **Export packed results as a ZIP** (powered by JSZip)
- **Installable as an app (PWA)**: works in standalone mode and can be used offline once installed
- Dark, FNF-styled interface with the *VCR* font, plus built-in music

## Getting started

### Use it online

Open the hosted page in any modern browser (Chrome, Edge, Firefox, Safari). You can also install it as an app from your browser's menu.

### Run it locally

The editor is a static site, so there is nothing to build. Clone the repo and serve it with any static server:

```bash
git clone https://github.com/ArngMods93/Hendrix--Spritemaps-Editor-PLUS.git
cd Hendrix--Spritemaps-Editor-PLUS

# any static server works, for example:
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

> **Note:** opening `index.html` directly with `file://` works for the editor itself, but the service worker (offline mode / PWA install) only runs over `http://localhost` or `https://`.

## Project structure

| File | Description |
| --- | --- |
| `index.html` | The whole editor: UI, styles and logic |
| `manifest.json` | PWA manifest (name, icons, theme colors) |
| `sw.js` | Service worker for offline support |
| `icon-192.png`, `icon-512.png`, `icon-original.png` | App icons |
| `*.mp3`, `*.ogg` | Audio files used by the app |

## Built with

- HTML
- JavaScript
- [JSZip](https://stuk.github.io/jszip/) for ZIP packing and unpacking

## Credits

- Original project: [hendrixfunker053/Hendrix-Spritemaps-editor-](https://github.com/hendrixfunker053/Hendrix-Spritemaps-editor-)
- PLUS version: [ArngMods93](https://github.com/ArngMods93)

## Contributing

Found a bug or have an idea? Feel free to open an [issue](https://github.com/ArngMods93/Hendrix--Spritemaps-Editor-PLUS/issues) or send a pull request.
