# Overlays, GeoJSON, GPX

Source: `javalent/obsidian-leaflet` README.

## Circle overlays

```
overlay: [<color>, [<lat>, <long>], <radius> <unit>, <description>]
```

```leaflet
overlay:
  - ['#FF0000', [32, 89], 25 km, 'Red zone']
  - ['rgb(0,255,0)', [40, 90], 500 ft, 'Green zone']
```

Quote hex colors and any value that contains a comma.

```leaflet
overlayTag: nearby
overlayColor: blue
```

## Image overlays

```leaflet
imageOverlay:
  - [[[assets/maps/ward.webp]], [800, 0], [0, 600]]
```

## GeoJSON and GPX

```leaflet
geojson: [[assets/maps/harbor.json]]
geojsonColor: "#3388ff"

gpx: [[assets/maps/coast.gpx]]
```

Put those files in `assets/` with the map image.
