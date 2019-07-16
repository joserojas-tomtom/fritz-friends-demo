# Maps SDK for Web 5.21.4

## Documentation

Please refer to the [Maps SDK section](https://developer.tomtom.com/maps-sdk-web-js) in TomTom's Developer Portal for detailed documentation with examples.

Also, the latest version of this SDK can be found there.

## Package content

The package contains the following files:

- `maps-web.min.js` - Library prepared to be included direcly in your HTML file.
- `maps-web.min.js.map` - Source map for the SDK build file.
- `maps.min.js` - Library in [UMD format](https://github.com/umdjs/umd). The code is minified and does not need any external dependencies.
- `maps.min.js.map` - Source map for the SDK build file.
- `maps.css` - Cascading Style Sheet needed by the library. It must be included in your webpage in order to render the expected map.
- `LICENSE.txt` - License file.
- `README.md` - This file.
- `glyphs/` - Glyphs files used by the vector tile layer.
- `sprites/` - Sprite images used by the vector tile layer to display the shields over the map.
- `css-styles/` - Cascading Style Sheets providing utility classes (e.g., poi icons and traffic incidents marker styles).
- `styles/` - Definitions of map styles.

## Getting started

Please check the examples for a better understanding of the common use cases. The minimal *HTML* page allowed to display
the TomTom map could look like this:

```html
<html>
    <head>
        <link rel="stylesheet" type="text/css" href="maps.css"/>
        <script src="maps.min.js"></script>
    </head>
    <body style="width: 100%; height: 100%; margin: 0; padding: 0;">
        <div id="map" style="width: 100%; height: 100%;"></div>
        <script>
            const map = tt.map({
                key: "${api.key}",
                container: "map"
            });
        </script>
    </body>
</html>
```

Please note that you need to have a valid **API Key** which can be obtained at [TomTom's Developer Portal](https://developer.tomtom.com).

## License

© 1992 – 2019 TomTom International B.V.
The library is licensed under Apache License Version 2.0, check LICENSE.txt for details.
