# Tiles and metadata for [CivMap](https://civmap.github.io/)

Tiles are stored in the format `tiles/<world name>/z<zoom>/<x>,<z>.png` where `x` and `z` are the coordinates of that region, and `zoom` is 0 for one pixel per block and decreases by 1 every time the viewport width is doubled.

#### Files in `meta/`:
Coordinates are in `z,x` order, because Leaflet uses the `lat,long` standard. Bounds are a two-element array of two opposite corner points, usually `[[north, west], [south, east]]`.

- `maps.json`: map overlay images, `src` is optional and unused
- `portals.json`: portal positions and sizes
- `shard-ids.json`: convert (short) shard name to world id
- `tiles.json`: which shards to show and which tiles can be loaded
- `world-borders.json`: radii of the circular world borders

Some are not in use yet but all will be in the future.

Thank you [@Waffle-Stomper](https://github.com/waffle-stomper) for providing the world borders and portal coordinates in [a programmer-friendly form](https://github.com/waffle-stomper/WorldBorderViewer/blob/c9314a31a1657723abb787d1d5018ba8d8d06596/forge/src/main/java/wafflestomper/worldborderviewer/WBConfigManager.java#L84)!

## Map data contributors
A big *Thank You* to everyone who sent me their VoxelMap cache to fill the empty spots on the maps:
[ASomb](https://reddit.com/user/AddictiveSombrero),
[BritishBean](https://reddit.com/user/BritishBean),
[CalgarPascal](https://reddit.com/user/CalgarPascal),
[ChezireNeko](https://reddit.com/user/ChezireNeko),
[gantAR1](https://reddit.com/user/gantAR1),
[JhillOne](https://reddit.com/user/JhillOne),
[jQjx](https://reddit.com/user/jQjx),
[Kwikxilver](https://reddit.com/user/Kwikxilver),
[MattThePapa](https://reddit.com/user/MattThePapa),
[raceman95](https://reddit.com/user/raceman95),
[RibaT111](https://reddit.com/user/RibaT111),
[RonnySpears](https://reddit.com/user/RonnySpears),
[Searedoriginal](https://reddit.com/user/Searedoriginal),
[v3n0m95](https://reddit.com/user/v3n0m95),
[VIDE0HEAD](https://reddit.com/user/VIDE0HEAD),
[walkersgaming](https://reddit.com/user/walkersgaming),
[wuphonsreach](https://reddit.com/user/wuphonsreach)
