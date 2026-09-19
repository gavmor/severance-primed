# Severance Primed

A *Cortex Prime* tabletop roleplaying game of Lumon Industries and the severed
floor — built from the Nine Principles. Corporate dystopia, paranoid
espionage thriller, religious cult drama.

## Contents

| File | What it is |
|---|---|
| `severance-primed-basis.html` | The 10-page basis document (setting, trait sets, mods, sample PCs, Session One) |
| `charsheet.html` | Blank 2-page character sheet (the Lumon file / what's hidden) |
| `pregens.html` | Pregenerated characters (Sol W., Ana R.) with trait-halo portraits |
| `portraits/` | Painted retro-corporate portraits + generation metadata |
| `fonts/` | CortexSymbology die-glyph font (community Cortex Prime font) |

## Building the PDFs

Rendered with [WeasyPrint](https://weasyprint.org/) (v70):

```bash
pip install weasyprint
python3 -c "from weasyprint import HTML; HTML(filename='severance-primed-basis.html').write_pdf('severance-primed-basis.pdf')"
python3 -c "from weasyprint import HTML; HTML(filename='charsheet.html').write_pdf('severance-primed-charsheet.pdf')"
python3 -c "from weasyprint import HTML; HTML(filename='pregens.html').write_pdf('severance-primed-pregens.pdf')"
```

All pages are US Letter. The trait halos follow Miriam Robern's canonical
geometry: a painted portrait ringed by one thin continuous circle studded with
die glyphs, trait labels to the side of each die, name as caption below.

## Design notes

- The Nine Principles are the Values prime set (d4–d12) with challengeable
  statements. Upholding one at real cost steps it up for the scene;
  challenging one grants 1 PP and steps up the Doom Pool.
- Opposition is always a Doom Pool (**The Nine**), a Crisis Pool (a File like
  Cold Harbor), or a named GMC (Cobel, Milchick) — never a contest against a
  faction. Pools are rolled and kept, never added.
- Stress is Woe, Frolic, Dread, Malice. Past d12: Break Room Compunction.
