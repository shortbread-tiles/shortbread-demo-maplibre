# `shortbread-demo-maplibre`

A demo of using [Shortbread Vector Tiles](https://shortbread-tiles.org/) styled with [MapLibre map rendering](https://maplibre.org/).

This is a very, very simple demo style, which doesn't show the range of what is possible with Shortbread.

## Get some tiles

Consult the [Shortbread documentation](https://shortbread-tiles.org/) for how to get a shortbread mbtiles file.

## Running

### Serving vector tiles from a mbtiles file

Your browser needs the tiles in the mbtiles file to be accessible via HTTP. [Tilemaker](https://tilemaker.org/) contains a simple `tilemaker-server` tool which does this easily. Keep this command running while you use the map.

    tilemaker-server ./path/to/shortbread.mbtiles

The map style presumes the tiles are served on `http://localhost:8080/`, which is the default for this command.

### Local files

You need to access the `index.html` file via HTTP, not via a `file://` URL, which happens when you open the HTML file in your web browser. Use a static HTTP server like [`simple-http-server`](https://github.com/TheWaWaR/simple-http-server) to serve the files in this directory. This tool

    simple-http-server --cors -i .

The map style & HTML & JS presume content is server on `http://localhost:8000/`, which is the default for this command.

### Website

View the simple map: [`http://localhost:8000/`](http://localhost:8000/)!
