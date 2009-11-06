Compiles one or more JavaScript files/fragments with the [Google Closure
Compiler](http://code.google.com/closure/compiler/docs/overview.html). 

The default compilation level is _WHITESPACE\_ONLY_. Another level can be
specified with the `--level` option. _SIMPLE\_OPTIMIZATIONS_ can be
abbreviated as _simple_, _ADVANCED\_OPTIMIZATIONS_ as _advanced_, and
_WHITESPACE\_ONLY_ as _whitespace_.

The JavaScript to compress can be supplied on STDIN, or contained in files
named on the command line. The compressed JavaScript is printed to STDOUT.

For example, `js-compile some.js` performs whitespace-only compression on the
file named _some.js_. `js-compile --level=advanced <some.js >compressed.js`
performs advanced compression on the files it receives via STDIN, then writes
then concatenated result to _compressed.js_.
