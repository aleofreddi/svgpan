# svgpan
Tiny Javascript to add pan, zoom &amp; drag capabilities to SVG.

Some time ago I had a need to display some vectorial drawings on the web so I've found out that SVG is decently supported by modern browsers (I won’t say anything about Internet Explorer – it’s just unsupported there). The language itself is great, but the interactivity provided by the browsers is definitely low: can display your SVG file on a browser and that's it - you can't navigate it, zoom it or pan :(

Since I couldn't find anything around, I've decided to write a minimalistic javascript library to provide such interactions, so SVGPan was born!

Features:

- Panning (pan à la Google maps) (click on the white background and pan)
- Zooming (using the mouse wheel)
- Element dragging (click on a drawing element and drag it somewhere else)
- Combinations of the above like zooming while dragging

The library itself is very small and easy to use; and it’s licensed under the BSD license. You can try a [demo](http://www.vleo.net/docs/projects/SVGPan/tiger.svg).

## Quickstart
You can install svgpan via [bower](http://bower.io):

```
bower install svgpan
```

Alternatively just download svgpan.js into your application.

The library requires a root group to be identified by the id `viewport`, which is where the svg/pan/zoom will be applied. Below an example:

```html
<script xlink:href="svgpan.js"/>

<g id="viewport" transform="translate(200,200)">...
```
