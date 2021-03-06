# SFL -- Standard Function Library

SFL is the iMatix Standard Function Library, which is:
(a) a portability layer for C, across Unix, Windows, etc; and

(b) a library of base functions useful for building real software

It was developed stand alone throughout the 1990s, and then later 
incorporated directly into iMatix products such as the Xitami
webserver.   It became a key part of the iMatix "base" in the early
2000s and was not released separately after that.

The original license for SFL is in [src/license.txt](src/license.txt).
Briefly it allows usage under the GNU General Public License, the
Perl Artistic License, or with a advertising clause.  See
[src/license.txt](src/license.txt) for details.

On [2016-04-29 it was also released under the
MPLv2](https://github.com/imatix-legacy/license) ([license
text](https://imatix-legacy.github.io/license/MPLv2.html)), so `SFL` can
be used under either GPLv2, the Perl Artistic license, a license
with an advertising clause or the MPLv2.

This repository contains the last SFL source, binaries,and documentation
released in a stand alone version, retrieved from:

*  http://legacy.imatix.com/pub/sfl

*  http://legacy.imatix.com/html/sfl

on 2016-04-27.

See the [documentation](https://imatix-legacy.github.io/sfl/) for 
more information.

## `pub`

The `pub` directory contains the released artefacts (binaries, source
archives, etc) which are still retrievable; if older releases artefacts
are found they may be added later.  Due to their small size (well under
1MB each), and the fact that development ceased many years ago (so there
will not be growth in the archive), these are added directly into the
git repository.

## `src`

The `src` directory was created from the unpacked contents of
`pub/src/sflsrc21.tgz`, for ease of reference.  To this the `sfldoc*.txt`
files and `*.def` files were added from an early 2000 build directory, with
approximately the equivalent documentation version.

The build scripts were built with
[otto](https://github.com/imatix-legacy/otto) from
[src/buildsfl.txt](src/buildsfl.txt).  Building the documentation requires
[srcdoc](https://github.com/imatix-legacy/srcdoc) and 
[htmlpp](https://github.com/imatix-legacy/htmlpp).

## `website`

The `website` directory contains the *rendered* documentation.  This
is approximately equivalent to the contents of `pub/doc/sfldoc21.tgz`, but
was taken directly from http://legacy.imatix.com/html/sfl.

The documentation was built (with `htmlpp`) from a marked up text file.
`src/sfldoc.txt`, `src/sfldoc1.txt` and `src/sfldoc2.txt` contain
*approximately* equivalent source for the documentation, taken from 
an early 2000 build directory.  These should rebuild to *similiar* 
documentaton but it may not be exactly identical.
