# gps-hiking-maps-releases

**Public download server for offline hiking map packages** of the
HikingLife app.

- Pipeline source (private): `DapDeveloper/gps-hiking-maps`
- Packages are published here as **GitHub Release assets** (tag `v<version>`)
- `releases/manifest.json` is the machine-readable package index (region,
  version, size, sha256) the app uses to discover downloads

## For the app

Download URL pattern:

```
https://github.com/DapDeveloper/gps-hiking-maps-releases/releases/download/v<version>/<region>-v<version>.mbtiles
```

Every package is a standard **MBTiles (vector)** file rendered with
`hiking-style.json` (paths, footways, tracks, bridleways, streams, peaks,
refuges, viewpoints, shelters, water sources, parking).

## Data license

Map data © OpenStreetMap contributors — [ODbL 1.0](https://opendatacommons.org/licenses/odbl/).
The HikingLife app must display this attribution when rendering the maps.

## For maintainers

Build requests / region suggestions → open an issue on the private repo or
contact the maintainers.
