# ICit

**ICit** — drop an IFC, OBJ, STL, PLY, or glTF file onto the page and your building model loads instantly, no install, no internet, no data leaving your machine.

Built for architects, designers, and QA assessors working on NZ residential construction — select elements by IFC class, export Psets and quantities to CSV for cost planning and compliance review, render shadow studies at up to 4K.

Single HTML file, runs offline from a USB stick or a locked-down government computer via `file://`. No server, no login, no subscription.

FOSS stack: three.js (MIT) + web-ifc (MPL-2.0). Built and maintained by Empiricus Design, Christchurch, Aotearoa New Zealand.

---

## Download and use

1. Go to [`dist/icit_v0.9.html`](dist/icit_v0.9.html)
2. Click **Download raw file** (the download icon, top right of the file view)
3. Double-click the downloaded file — it opens in your browser
4. Drop an IFC file onto the page

That's it. Nothing to install.

---

## Supported formats

| Format | Notes |
|---|---|
| IFC | IFC2x3, IFC4, IFC4X3 (partial) |
| OBJ | Wavefront |
| STL | Binary and ASCII |
| PLY | With vertex colours |
| glTF / glb | Binary and text |

---

## Keyboard shortcuts

| Key | Action |
|---|---|
| `R` | Toggle shadow mode (1024px live preview) |
| `R` *(in shadow mode)* | High-quality render → clipboard |
| `Alt+Z` | X-ray mode — see through model |
| `A` | Select all visible / deselect all |
| `L` | Select all of same IFC class |
| `Ctrl+I` | Invert selection |
| `H` | Hide selected |
| `Shift+H` | Isolate selected |
| `Alt+H` | Unhide all |
| `Ctrl+F` | Focus search |
| `Escape` | Clear search |

---

## Platform support

| Platform | Status |
|---|---|
| Windows | ✓ Full support |
| macOS | ✓ Full support |
| Chromebook | ✓ Full support |
| Android | ✓ Chrome for Android |
| iOS / iPadOS | ✗ Apple blocks local file access |

---

## For contributors

If you want to modify the source and rebuild:

```bash
# Prerequisites: Node.js 18+
npm install

# Build
node build.js
# Output: dist/icit_v0.9.html
```

Source is in `src/app.js`. The build script assembles three.js, web-ifc WASM, and the app JS into a single self-contained HTML file.

---

## Licence

GPL-3.0 — see [LICENSE](LICENSE)

Empiricus Design — [empiricus.co.nz](https://empiricus.co.nz) — github.com/4nigel
