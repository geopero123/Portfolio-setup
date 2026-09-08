# Utility Tools

Five standalone, client-side web tools. Each lives in its own folder with its own
dependencies, its own build, and its own visual identity — they are siblings in
purpose, not in appearance.

Every tool runs entirely in the browser. No backend, no upload, no API keys.

| # | Tool | What it does | Status |
| --- | --- | --- | --- |
| 1 | [`01-file-converter`](./01-file-converter) | Images ↔ PNG/JPG/WEBP/GIF/PDF, DOCX → HTML/MD/TXT, CSV ↔ JSON | ✅ Built |
| 2 | `02-pdf-toolkit` | Merge, split, compress PDFs; images ↔ PDF pages | Planned |
| 3 | `03-image-compressor` | Bulk compress and resize with live preview | Planned |
| 4 | `04-qr-generator` | QR codes (URL, wifi, vCard) and barcodes | Planned |
| 5 | `05-markdown-to-pdf` | Live markdown editor with styled PDF export | Planned |

## Running any of them

```bash
cd 01-file-converter
npm install
npm run dev
```

Each folder has its own README covering libraries, limits, and deployment.

## Shared conventions

- **React 19 + Vite + Tailwind CSS v4**
- **`lucide-react`** for icons throughout — no emoji standing in for iconography
- **Self-hosted variable fonts** via `@fontsource-variable`, so type renders
  identically offline and on first paint
- **Static output** — `npm run build` produces a `dist/` folder that deploys to
  Vercel, Netlify, Cloudflare Pages, or any static host with no configuration
