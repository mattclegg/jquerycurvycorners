# jQuery Curvy Corners #

jQuery Curvy Corners is a jQuery plugin for adding rounded corners to HTML block elements i.e. DIVs. It Supports anti-aliasing, borders and background images. It is licensed under the LGPL.

It is based on, and contains code from, "[Curvy Corners](http://code.google.com/p/curvycorners/)" by Cameron Cooke. The end result is a jQuery optimised file thats much smaller in size that still works great. The official site for the original curvy corners script is http://www.curvycorners.net.

## Usage ##

To use this plugin just apply corners via CSS Rules and include this plugin - it will automatically detect styles and apply corners.

  * Opera and Chrome support rounded corners via `border-radius`
  * Safari and Mozilla support rounded borders via `-webkit-border-radius` and `-moz-border-radius`
  * IE (any version) does not support border-radius - this is all curvy corners need to support.

So to make curvycorners work with any major browser simply add the following CSS declarations:

> .round {
> > border-radius: 3px;
> > -webkit-border-radius: 3px;
> > -moz-border-radius: 3px;

> }

If you don't want to use the above method, you can still use the direct syntax if you want:

> $('.myBox').corner({
> > tl: { radius: 8 },
> > tr: { radius: 8 },
> > bl: { radius: 8 },
> > br: { radius: 8 },
> > antiAlias: true

> });

The script will still apply border-radius for those browsers which support it.