# Wax

Tools for improving web maps. The centerpiece of the code is a client implementation of the [MBTiles interaction specification](https://github.com/mapbox/mbtiles-spec).

For full documentation of supported mapping APIs and how to use Wax see http://mapbox.github.com/wax.

## Versions

There are three current development branches of Wax:

* `master`, this branch, supports **Modest Maps 1.x**, the latest version of Modest Maps _only_
* 4.x supports **Modest Maps 0.x**, older versions of Modest Maps
* 6.x is **unstable** and will introduce new **event-based interaction APIs**

To find more detail of what has changed in each version, consult `CHANGELOG.md`.

## Compatibility

* Google Maps API v3
* Leaflet 0.x.x
* Modest Maps 1.x.x
* OpenLayers 2.11

## Building Wax

For end users, a minified library is already provided in `dist/`.

But for developers you can rebuild a minified library by running:

    npm install --dev
    make

## Includes

Wax currently includes three externals:

* [reqwest](https://github.com/ded/reqwest) (MIT)
* [mustache.js](https://github.com/janl/mustache.js) (MIT)
* [html-sanitizer from Google Caja](http://code.google.com/p/google-caja/source/browse/trunk/src/com/google/caja/plugin/html-sanitizer.js) (Apache)

## Authors

- Tom MacWright (tmcw)
- Young Hahn (yhahn)
- Will White (willwhite)
