# svgpan
Tiny Javascript to add pan ,zoom &amp; drag capabilities to SVG.

Some time ago the need for a browser-compatible vectorial language pushed me to consider the SVG markup language (I won’t say anything about Internet Explorer – it’s just unsupported there). The language itself is great, but, as a beginner, I was so disappointed about the fact that on the Internet I couldn’t find ANY library ready to use for panning and zooming features that I had to write one from scratch.

The SVGPan library features:

Panning (pan à la Google maps) (click on the white background and pan)
Zooming (using the mouse wheel)
Element dragging (click on a drawing element and drag it somewhere else)
Combinations of the above like zooming while dragging
The resulting javascript library is published here, in the hope that someone can find it useful. The library itself is very small and easy to use; and it’s licensed under the BSD license. You can try a demo here

## How to use

You can also open [the demo at vleo.net](http://www.vleo.net/docs/projects/SVGPan/tiger.svg).

The library itself requires a root group to be identified by the id viewport, which confines the svgpan library effects, and the import of the javascript code as well. For example, to adapt the tiger drawing, it was necessary to add the following:

```html
<script xlink:href="SVGPan.js"/>

<g id="viewport" transform="translate(200,200)">...
```

If you found this code useful please consider donating!
