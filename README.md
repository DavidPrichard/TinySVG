# TinySVG
A set of hand-optimized SVG icons.

Even the most bloated SVG icon is pretty small, but sometimes you want it to be even smaller.

SVGs that have come out of Inkscape or Illustrator have a lot of editor-specific markup, redundant groups and other unused
fluff that can be largely eliminated with the smart use of a tool like SVGOMG, which I highly recommend.

What is often overlooked, however, is that when Inkscape and Illustrator 'optimize' an SVG, they are actually attempting to
approximate its shape with as few bezier curves as possible- and they do a great job! For hand-drawn and complex shapes it is impressive stuff. But for the basic shapes most icons are composed of, it doesn't make much sense.

So, in the spirit of unnecessary, life-affirming optimization, I've spent a little time making generic SVG icons- like the three-bar menu icon- using hand-written SVG commands. It's a little hassle for a little bit of gain.

As a bonus, each SVG in the set has it's color or stroke-color set to "currentColor", so that they will act like a font and take on whatever color they are assigned or inherit through CSS.
