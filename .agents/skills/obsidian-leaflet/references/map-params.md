# Map parameters

Source: `javalent/obsidian-leaflet` README.

## Core

| Parameter | Purpose | Example |
|-----------|---------|---------|
| `id` | Required. Mutable in-app markers persist per `id` in the plugin cache | `id: kalowe-harbor` |
| `image` | Image layer, as a wikilink | `image: [[assets/maps/kalowe-harbor.webp]]` |
| `lat` / `long` | Initial view center | `lat: 400` / `long: 300` |
| `height` / `width` | Container size | `height: 900px` / `width: 95%` |

Multiple images:

```leaflet
image:
  - [[assets/maps/harbor-day.webp]]
  - [[assets/maps/harbor-night.webp]]
```

## Bounds

```leaflet
bounds:
  - [<top-left-lat>, <top-left-long>]
  - [<bottom-right-lat>, <bottom-right-long>]
```

Maps `[lat, long]` onto that box — typically the image's pixel
dimensions. Omit `bounds:` and the plugin uses CRS.Simple percentage
space (fractional coords like `[-2.09, 1.28]`), not pixels.

`lat` counts **up from the image bottom**. Image-editor pixels count
down from the top: `lat = <image height> - <pixels from top>`.

With `bounds:` set, an omitted `lat`/`long` falls back to `[50, 50]`
— a corner of a pixel-scale map. Set them to the image center.

## Zoom

```leaflet
minZoom: -2
maxZoom: 1
defaultZoom: -1
zoomDelta: 1
```

Pixel-scale bounds (hundreds/thousands wide) need a **negative** zoom
range. `defaultZoom: 1` on a 1600px image is ~2× native and crops the
map. Plugin discussion: `javalent/obsidian-leaflet-plugin` #130.

## Distance

```leaflet
unit: feet
scale: 5
```

`unit` is what a scale bar / overlay radius measures (`feet`, `meters`,
`miles`, `km`). `scale` is how many of that unit one map unit is.

## Real-world tiles

For a real-world map (`lat`/`long`, no `image:`):

```leaflet
tileServer: https://{s}.basemaps.cartocdn.com/dark_all/{z}/{x}/{y}{r}.png|Dark
tileOverlay: https://tiles.wmflabs.org/hillshading/{z}/{x}/{y}.png|Hills|on
osmLayer: false
```
