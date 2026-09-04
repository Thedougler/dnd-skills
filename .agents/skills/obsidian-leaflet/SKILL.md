---
name: obsidian-leaflet
description: >-
  Leaflet map fence, marker, overlay, or GeoJSON/GPX on a spatial
  page. Use when authoring or editing a `leaflet` code block, adding
  a pin, shading a region, or layering an overlay. Player-facing maps
  are renderer output (static image), not this fence.
---

# Obsidian Leaflet

The Leaflet plugin (`javalent/obsidian-leaflet`) renders a `leaflet`
fence as a pannable map. In this vault the fence lives on a spatial
page (`location`, `settlement`, `region`, `dungeon`). The image file
lives in `assets/`. Geography fields (`within`, `adjacent_to`,
`near`, cardinals, `geo_anchor`) stay the spatial source of truth.

Player-facing maps are renderer output — a static image. The live
fence is DM runtime chrome. There is no `kind: player-handout`.

## Quick syntax

```leaflet
id: kalowe-harbor
image: [[assets/maps/kalowe-harbor.webp]]
bounds:
  - [0, 0]
  - [800, 600]
lat: 400
long: 300
height: 900px
width: 95%
defaultZoom: -1
minZoom: -2
maxZoom: 1
unit: feet
scale: 5
marker:
  - default, 200, 150, [[location.widow-hollow|Widow's Hollow]], Abandoned watchtower
```

`marker:` is seven positional fields —
`type,lat,long,link,description,minZoom,maxZoom`. Detail:
`references/markers.md`.

## What you need

| Need | Read |
|------|------|
| `id` / `image` / `bounds` / zoom / scale / tiles | `references/map-params.md` |
| Pins, frontmatter markers, custom types | `references/markers.md` |
| Overlays, GeoJSON, GPX, image overlays | `references/overlays.md` |

## Workflow

### 1. Place the fence

Put it on the spatial page the map depicts. Put the image in `assets/`.
Give the block a stable `id`.

**Complete when** the page is a spatial kind, the image path is under
`assets/`, and `id` is unique.

### 2. Set the coordinate space

Image maps need `bounds:` (usually the image pixel box) and a center
(`lat` / `long` at half height, half width). `lat` counts up from the
bottom; convert from an image editor's top-down pixels:
`lat = height - pixelsFromTop`.

**Complete when** a test marker lands on the intended feature.

### 3. Add markers and overlays

One `marker:` key. A list of CSV strings. Description in field 5 so
the pop-up has text. Overlays and GeoJSON per `references/overlays.md`.

**Complete when** every pin has a type, coordinate, link, and
description, and the map builds in Obsidian.

## Out of scope

Player-facing map handouts (renderer output). Geography field authorship (the location schema).
Custom marker *types* are named in the plugin Settings tab, then
referenced here — this skill does not invent a `markers.json`.
