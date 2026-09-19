# Severance Primed

A *Cortex Prime* tabletop roleplaying game of Lumon Industries and the severed
floor — built from the Nine Principles. Corporate dystopia, paranoid
espionage thriller, religious cult drama.

## Contents

| File | What it is |
|---|---|
| `severance-primed-basis.html` | The 19-page basis document, formatted as a diegetic Lumon Industries *Handbook for the Severed Employee* (setting, trait sets, mods, sample PCs, Session One) |
| `charsheet.html` | Blank 2-page character sheet (the Lumon file / what's hidden) |
| `pregens.html` | Pregenerated characters (Sol W., Ana R.) with trait-halo portraits |
| `portraits/` | Painted retro-corporate portraits + generation metadata |
| `fonts/` | CortexSymbology die-glyph font + the Lumon type system (Michroma, Archivo, Cinzel, IBM Plex Mono, Spectral, Caveat) |

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

## The handbook is the artifact

The basis document is formatted as a genuine Lumon Industries publication —
*Handbook for the Severed Employee*, Macrodata Refinement Division
(Doc. No. LUM-MDR-0047, Rev. 12). The design follows the show's own visual
system: stratified typography (Michroma for corporate authority, Archivo for
house style, Cinzel for scripture, IBM Plex Mono for terminals, Spectral for
body), the quarantined palette (Deep Blue `#294CA2`, Turf Green, Alabaster,
Slate — red reserved strictly for defiance), document-control apparatus,
an intake form, personnel files, and the full Compunction Statement on a
Break Room terminal.

Running through it in contraband red: marginalia from "P." — the innie who
stopped believing — including a torn-out Reintegration page taped back in.
