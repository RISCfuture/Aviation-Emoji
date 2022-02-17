# Aviation Emoji

This repository contains a collection of aviation-related emoji for Slack. The emoji are created using [Sketch](https://www.sketch.com). To generate the emoji, simply choose the "Export…" option from Sketch.

Generated emoji are available for download under Releases, in PNG and SVG format. Emoji have feathered alpha masks making them visible in light and dark themes.

Available emoji include:

* AIRMET/SIGMET symbols
* ForeFlight-esque flight condition symbols
* METAR precipitation and visibility symbols
* The Garmin "direct-to" symbol
* Prog chart symbols
* Flight instruments
* Glideslope indicators (PAPI and IFLOLS)
* Aviation organization logos

![preview](https://user-images.githubusercontent.com/15338/154589046-ec4e09dd-72b6-4165-9854-aabf5914b264.png)

## Releasing

After generating the images using Sketch…

* To optimize the SVGs: `svgo -r .`
* To crush the PNGs: `find . -name *.png -exec pngcrush -brute -reduce -ow {} \;`
* To generate the preview image using ImageMagick: `montage -tile 10x0 **/*.png preview.png`
