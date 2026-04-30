<div align="center">

<img src="oDoc_icon_logo.jpeg" alt="oDoc Logo" width="120" height="120" style="border-radius: 22px;" />

# oDoc

**A clean, fast, single-file document reader & editor.**  
No install. No account. No cloud. Just open and read.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![HTML](https://img.shields.io/badge/Built%20with-HTML%2FJS-f7df1e?logo=javascript)](oDoc.html)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/oDoc/oDoc/pulls)
[![No dependencies](https://img.shields.io/badge/dependencies-0-success)](oDoc.html)

[**→ Open oDoc**](https://odoc.github.io/oDoc) · [Report Bug](https://github.com/oDoc/oDoc/issues) · [Request Feature](https://github.com/oDoc/oDoc/issues)

</div>

---

## What is oDoc?

oDoc is a **single HTML file** that lets you open, read, and edit documents — right in your browser. No server required, no sign-up, no data ever leaves your device. Download the file once and use it forever, even offline.

---

## ✨ Features

- **Multi-format support** — Open `.md`, `.txt`, `.html`, `.pdf`, and `.epub` files
- **Live Markdown preview** — Renders headings, code blocks, tables, blockquotes, and more
- **Edit mode** — Switch to a raw text editor at any time; edits update the preview in real time
- **Drag & drop** — Drop files anywhere on the window to open them instantly
- **Download** — Save edited files back to your device
- **Dark theme** — Easy on the eyes, always
- **Zero dependencies at runtime** — Ships with PDF.js and JSZip via CDN; works offline with a local copy
- **Single file** — The entire app is one `.html` file you can bookmark, share, or self-host

---

## 🚀 Getting Started

### Option 1 — Just open it

Download [`oDoc.html`](oDoc.html) and open it in any modern browser. That's it.

```bash
# Clone the repo
git clone https://github.com/oDoc/oDoc.git

# Open in your browser
open oDoc/oDoc.html
```

### Option 2 — Self-host

Drop `oDoc.html` on any static host (GitHub Pages, Netlify, Vercel, your own server):

```bash
# GitHub Pages example
git clone https://github.com/oDoc/oDoc.git
cd oDoc
# Push to a gh-pages branch or configure Pages to serve from main
```

### Option 3 — Use the live demo

Visit **(ODoc](https://odoc.oddsifylabs.com/))** — no download needed.

---

## 📄 Supported Formats

| Format | Extension | Notes |
|--------|-----------|-------|
| Markdown | `.md`, `.markdown` | Full preview with GFM-style rendering |
| Plain text | `.txt` | Displayed in a monospace editor |
| HTML | `.html`, `.htm` | Sanitized preview (scripts stripped) |
| PDF | `.pdf` | Text extraction via PDF.js |
| EPUB | `.epub` | Text extraction via JSZip |

> Unsupported formats (`.docx`, `.csv`, `.psd`, `.zip`, etc.) are intentionally excluded to keep the app focused and secure.

---

## 🖥 Interface

```
┌─────────────────┬──────────────────────────────────────┐
│  Sidebar        │  Header (filename · type · size)     │
│  ─────────────  │  ─────────────────────────────────── │
│  + Add Files    │  [ Preview ]  [ Edit ]               │
│                 │                                      │
│  📝 readme.md   │  Rendered document content           │
│  📕 report.pdf  │  or raw text editor                  │
│  📖 book.epub   │                                      │
│                 │                                      │
└─────────────────┴──────────────────────────────────────┘
```

- **Sidebar** — file list with icons, sizes, and one-click remove
- **Preview tab** — rendered output (Markdown, HTML) or plain text
- **Edit tab** — raw text editor; changes sync to preview instantly
- **Download button** — saves the current (possibly edited) file
- **Drag & drop** — drop files anywhere to add them

---

## 🔒 Privacy

oDoc processes everything locally in your browser.

- No files are uploaded to any server
- No analytics or tracking
- No cookies or local storage used
- Works fully offline once the page is loaded

---

## 🛠 Development

The entire app lives in a single file — `oDoc.html`. There is no build step.

```bash
git clone https://github.com/oDoc/oDoc.git
cd oDoc

# Edit the file
code oDoc.html

# Test in browser
open oDoc.html
```

**External libraries loaded via CDN** (swap for local copies if you need offline-first):

| Library | Version | Purpose |
|---------|---------|---------|
| [PDF.js](https://mozilla.github.io/pdf.js/) | 3.11.174 | PDF text extraction |
| [JSZip](https://stuk.github.io/jszip/) | 3.10.1 | EPUB parsing |

---

## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m 'Add my feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

For bugs or ideas, [open an issue](https://github.com/oDoc/oDoc/issues).

---

## 📜 License

Released under the [MIT License](LICENSE). Free to use, modify, and distribute.

---

<div align="center">

Made with ☕ · [oDoc](https://github.com/oDoc/oDoc)

</div>
