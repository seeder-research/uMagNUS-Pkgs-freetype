# uMagNUS-freetype
This is a port of the Freetype font rasterizer (www.freetype.org) to the Go
programming language (golang.org).

To download and install from source:
$ go get code.google.com/p/freetype-go/freetype

It is an incomplete port:
  * It only supports TrueType fonts, and not Type 1 fonts nor bitmap fonts.
  * It only supports the Unicode encoding.

There are also some implementation differences:
  * It uses a 24.8 fixed point co-ordinate system everywhere internally,
    as opposed to the original Freetype's mix of 26.6 (or 10.6 for 16-bit
	systems) in some places, and 24.8 in the "smooth" rasterizer.

Freetype-Go is derived from Freetype, which is written in C. Freetype is
copyright 1996-2010 David Turner, Robert Wilhelm, and Werner Lemberg.
Freetype-Go is copyright The Freetype-Go Authors, who are listed in the
AUTHORS file.

The Freetype-Go homepage is http://code.google.com/p/freetype-go/
