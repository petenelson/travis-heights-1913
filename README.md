# Travis Heights, 1913 vs. Today

An interactive overlay of the original 1913 "Map of Travis Heights" (Austin, Texas) on today's street map and aerial imagery, with notes on what changed.

**Live page:** https://petenelson.github.io/travis-heights-1913/ (once GitHub Pages is enabled)

## Files

- `index.html`: the page (Leaflet, OpenStreetMap tiles, Esri aerial imagery)
- `img/travis-heights-1913-georeferenced.webp`: the plat warped north-up to line up with the modern map (transparent outside the map frame)
- `img/travis-heights-1913-photo.jpg`: photo of the original paper map, rotated upright
- `data/georeference.json`: the control points and transform used

## How it was lined up

Thirteen street intersections that appear on both the 1913 plat and current OpenStreetMap data were matched by hand (for example, Travis Heights Blvd at Woodland, Fairmount and Avondale; Alta Vista at Algarita; Alameda at Riverside). A perspective (homography) transform was fit to those points and used to warp the photo. Typical error is 10–40 m. The largest error is near Mariposa Drive, and comes from the photo, the paper folds and the 1913 drafting.

## Publishing

Settings → Pages → Build and deployment → Deploy from a branch → `trunk` / root.

Map data © OpenStreetMap contributors. Aerial imagery © Esri.
