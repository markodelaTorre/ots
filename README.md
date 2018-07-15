[![Build Status](https://travis-ci.org/khaledhosny/ots.svg?branch=master)](https://travis-ci.org/khaledhosny/ots)
[![Build status](https://ci.appveyor.com/api/projects/status/0l9ms6g47corescm?svg=true)](https://ci.appveyor.com/project/khaledhosny/ots)

OpenType Sanitizer
==================

The OpenType Sanitizer (OTS) parses and serializes OpenType files (OTF, TTF)
and WOFF and WOFF2 font files, validating them and sanitizing them as it goes.

The C library is integrated into Chromium and Firefox, and also simple
command line tools to check files offline in a Terminal.

The CSS [font-face property][1] is great for web typography. Having to use images
in order to get the correct typeface is a great sadness; one should be able to
use vectors.

However, on many platforms the system-level TrueType font renderers have never
been part of the attack surface before, and putting them on the front line is
a scary proposition... Especially on platforms like Windows, where it's a
closed-source blob running with high privilege.

Building from source
--------------------

See [BUILDING](BUILDING.md)

Usage
-----

See [docs](docs)

* * *

Thanks to Alex Russell for the original idea.

[1]: http://www.w3.org/TR/CSS2/fonts.html#font-descriptions