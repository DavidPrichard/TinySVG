# TinySVG
A set of hand-optimized SVG icons.

## Use

It's pretty simple. `icon-set.svg` contains all the icons declared as symbols; in most cases you'd want to include this inline with your HTML. Symbols support 'title' and 'desc' attributes if you need them for accessibility.

The rest of the icons are included as individual .svg files for convenience, if you have some other use in mind.

## Rationale

There are a lot of free SVG icon sets out there, and some of them look pretty good. But even though nearly every icon is composed of simple geometric shapes, every set I've found defines their shape with bezier curves, making them much larger than necessary.

I suspect the issue is that the designers are using the automatic optimization features of Illustrator or Inkscape, which work by attmepting to approximate shapes as closely as possible using as few bezier curves as possible. For simple shapes that can be drawn with just straight lines and circles.

This may not matter much given the small size of even bloated SVGs, but for now animating them properly nearly requires that they be included inline in the HTML, which means they aren't cached by browsers, so when using many of them it may make a difference. The small size also makes them much less disruptive when reading through an HTML document, and if you want to create complex animations for your icon, it is easier to do so when you can independently address each shape in the composition.

As a bonus, each SVG in the set has it's color or stroke-color set to "currentColor", so they will take on whatever color they are assigned or inherit through CSS, just like a font.

### Contributing

Open an issue if you'd like to see a particular symbol; keep in mind that TinySVG is for symbols that can be mostly, or entirely, drawn without bezier curves (i.e. with straight lines and circles)

If you'd like to contribute a symbol, please submit a pull request!

### Credit

* Many thanks to [SVGO](https://github.com/svg/svgo) and Jake Archibald's [SVGOMG](https://jakearchibald.github.io/svgomg/), which make it possible to reduce bloated, illegible SVGs down to smaller sizes that a human can then edit by hand.
