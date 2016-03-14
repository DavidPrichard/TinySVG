# TinySVG
A set of hand-optimized SVG icons.

There are a lot of free SVG icon sets out there, and some of them look pretty good. But even though nearly every icon is composed of simple geometric shapes, every set I've found defines their shape with bezier curves, making them much larger than necessary.

I suspect the issue is that the designers are using the automatic optimization features of Illustrator or Inkscape, which work by attmepting to approximate shapes as closely as possible using as few bezier curves as possible. For simple shapes that can be drawn with straight lines and circles, this doesn't make much sense.

This may not matter much given the small size of even bloated SVGs, but for now animating them properly nearly requires that they be included inline in the HTML, which means they aren't cached by browsers, so the difference may add up to something. The small size also makes them much less disruptive when reading through an HTML document, and if you want to create complex animations for your icon, it is easier to do so when you can independently address each shape it is composed of.

As a bonus, each SVG in the set has it's color or stroke-color set to "currentColor", so that they will act like a font and take on whatever color they are assigned or inherit through CSS.
