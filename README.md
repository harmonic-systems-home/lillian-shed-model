# Lillian Drive Shed — interactive model

An interactive 3D model of a backyard storage shed. Rotate it, zoom, switch framing
layers on and off, and tap the photo markers to see the photograph taken at each spot.

**Live:** https://harmonic-systems-home.github.io/lillian-shed-model/

## This repository is generated

`index.html` and `assets/` are **built output**. The source lives in the private
`lillian-shed-design` repository, alongside the written record the model is drawn from —
measurements, condition notes, and the work plan.

**Don't edit `index.html` here.** Edit `model/shed-model.html` upstream and run
`scripts/publish-model.sh`, which rebuilds and pushes to this repo. Anything edited here
directly will be overwritten on the next publish.

## What the model shows

The shed is an older site-built gable structure: concrete block piers, two 4x girders with
4x4 joists laid across them, a ¾" plywood deck, 2x4 stud walls sheathed in plywood inside,
48" panel siding, and asphalt shingles over plywood.

Reading the colours:

| Drawn as | Means |
|---|---|
| Solid material | Existing, as built |
| Translucent teal with drawn edges | Proposed — not built |
| Red overlay | Damage, high severity |
| Amber overlay | Damage, medium severity |
| Amber arrows | Suspected movement, unconfirmed |

**Deviation is annotated, never modelled.** The geometry stays nominal even where the real
shed has moved — bending the model to match a guess would destroy the reference you measure
deviation against. Roof spread is drawn as arrows and candidate rafter ties; the roof
itself stays straight.

Several dimensions are still estimates rather than measurements, and the page says so on
its face. That caveat stays until the numbers are real.

## Photos

The images in `assets/` are stripped of all metadata except orientation. A CI check
refuses to publish if any of them carries GPS data.
