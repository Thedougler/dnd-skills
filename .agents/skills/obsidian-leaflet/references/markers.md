# Markers

Source: `javalent/obsidian-leaflet` README.

## Seven fields

```
marker: <type>,<lat>,<long>,<link>,<description>,<minZoom>,<maxZoom>
```

`type`, `lat`, `long` are required. The rest are optional but
positional. Keep the empty slot if you skip `description` and still
want zoom bounds: `marker: default, 40, 90, [[location.x]], , 3, 8`.

A four-field tail (`type, lat, long, link`) builds, but the pin has
no pop-up text.

## Several pins — one key, list of strings

```leaflet
marker:
  - default, 40, 80, [[location.watchtower|Watchtower]], Abandoned watchtower
  - default, 41, 81, [[location.festival|Festival]], Festival grounds, 2, 6
```

Each entry is a bare CSV string. papaparse must receive a string.

Two shapes that look right and produce an empty dark container:

- Flow sequences (`- [default, 40, 80, [[Note]]]`) parse to arrays.
- Repeated `marker:` keys throw `YAMLParseError: Map keys must be unique`.

No comma inside a description. Fields split on commas; quoting does
not rescue a space-after-comma CSV.

## Markers from files

```leaflet
markerFile: [[location.harbor]]
markerFolder: world/
markerTag: harbor, active
filterTag: "#location"
linksTo: [[location.harbor]]
linksFrom:
  - [[location.market]]
```

Those notes supply position via their own frontmatter:

```yaml
location: [40, 89]
mapmarker: default
mapzoom: [2, 8]
```

## Custom types

Named only in Community plugins → Leaflet → marker types. Reference
the name in `marker:` / `mapmarker:`. There is no `markers.json` in
the vault.

In-app (mutable) markers persist in the plugin cache keyed on block
`id`. Code-block and frontmatter markers are what git sees.
