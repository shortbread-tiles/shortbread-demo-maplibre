# `shortbread-demo-maplibre`

A demo of using [Shortbread Vector Tiles](Shortbread Vector Tiles) styled with [MapLibre map rendering](https://maplibre.org/).

## Get some tiles

Consult the [Shortbread documentation](https://shortbread-tiles.org/) for how to get a shortbread mbtiles file.

## Running

### Serving vector tiles from a mbtiles file

Your browser needs the tiles in the mbtiles file to be accessible via HTTP. [Tilemaker](https://tilemaker.org/) contains a simple `tilemaker-server` tool which does this easily. Keep this command running while you use the map.

	tilemaker-server ./path/to/shortbread.mbtiles

### Local files

You need to access the `index.html` file via HTTP, not via a `file://` URL, which happens when you open the HTML file in your web browser. Use a static HTTP server like [`simple-http-server`](https://github.com/TheWaWaR/simple-http-server) to serve the files in this directory.


