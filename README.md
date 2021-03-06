# buffer-regexp-compiler-js
Compiles a string or RegExp instance to ecma-script for use with buffers.  
Supports ECMA5, ECMA2016, 2017 and PERL features as well as all popular flavors 
of regular expressions.

installations:
~~~~
> npm install buffer-regexp-compiler-js          # for node script project use
> npm install buffer-regexp-compiler-js -save    # for node cli and script project use
> npm install buffer-regexp-compiler-js -global  # for node cli and script global use
~~~~

cli use:
~~~~
regexp-compiler '(\\w+)' --flags=g
regexp-compiler --source='source.js'
~~~~

module use:
~~~~
const CRegExp = require( 'regexp-compiler.js' )
    .ClassFactory( { flavor: 'PERL', library: library } );
~~~~

   with
~~~~
cre = new RegExpCompiler.RegExp( /(\w+)/ );
~~~~

or
~~~~
cre = new RegExpCompiler.RegExp( '(\\w+)', 'g' );
~~~~

or
~~~~
cre = new RegExpCompiler.RegExp( ).compile( '(\\w+)'
    , { global: true } );
~~~~

or
~~~~
CRegExp = RegExpCompiler.classFactory( { flavor: 'PERL', library: library } );
cre = new CRegExp( /(\w+)/ );
~~~~

browser use:
~~~~
<script src="https://github.com/LaughingSun/buffer-regexp-compiler-js/build/regexp-compiler-min.js"></script>
~~~~

or
~~~~
<script src="https://github.com/LaughingSun/buffer-regexp-compiler-js/build/regexp-compiler.js"></script>
~~~~

or
~~~~
<script type="module" src="https://github.com/LaughingSun/buffer-regexp-compiler-js/build/regexp-compiler-min.js"></script>
~~~~

or
~~~~
<script type="module" src="https://github.com/LaughingSun/buffer-regexp-compiler-js/build/regexp-compiler.js"></script>
~~~~

with
~~~~
<script>
cre = new RegExpCompiler.RegExp( /(\w+)/ );
</script>
~~~~

or
~~~~
<script>
cre = new RegExpCompiler.RegExp( '(\\w+)', 'g' );
</script>
~~~~

or
~~~~
<script>
cre = new RegExpCompiler.RegExp( ).compile( '(\\w+)', { global: true } );
</script>
~~~~

or
~~~~
<script>
CRegExp = RegExpCompiler.ClassFactory( { flavor: 'PERL', library: library } );
cre = new CRegExp( /(\w+)/ );
</script>
~~~~
