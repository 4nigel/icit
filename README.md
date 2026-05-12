# ICit - a browser viewer-extractor for Ifc
ICit (i see it!) — drop an IFC, OBJ, STL, PLY, or glTF file onto the page and your building model loads instantly, no install, no internet, no data leaving your machine.

Built for building professinals working on small to medium sized projects — select elements by IFC class, export Psets and data/quantities to CSV for cost planning and compliance review, render shadow studies at up to 4K.

Single HTML file, runs offline from a USB stick or a locked-down government computer via file://. No server, no login, no subscription.

FOSS stack: three.js (MIT) + web-ifc (MPL-2.0). Built and maintained by Nigel with enormous help from Claude!

**ICit — Keyboard Shortcuts**

it is not by accident that many of these will look familiar to Blender Users

**Navigation**
| Key | Action |
|---|---|
| `F` | Fit model to screen |
| `Alt+Z` | X-ray mode — see through model |

**Shadows**
| Key | Action |
|---|---|
| `R` | Enter shadow mode (1024px live preview) |
| `R` *(in shadow mode)* | High-quality render at selected resolution → clipboard |

**Selection**
| Key | Action |
|---|---|
| `Click` | Select single element |
| `Ctrl+Click` | Add or remove element from selection |
| `Shift+Click` | Range select within same IFC class in tree |
| `A` | Select all visible — press again to deselect all |
| `Ctrl+I` | Invert selection |
| `L` | Select all elements of same IFC class as current selection |

**Visibility**
| Key | Action |
|---|---|
| `H` | Hide selected elements |
| `Shift+H` | Isolate selected — hide everything else |
| `Alt+H` | Unhide all — restore full model visibility |

**Search**
| Key | Action |
|---|---|
| `Ctrl+F` | Focus search box |
| `Escape` | Clear search and restore tree |
