# is-glob [![NPM version](https://badge.fury.io/js/is-glob.svg)](http://badge.fury.io/js/is-glob)  [![Build Status](https://travis-ci.org/jonschlinkert/is-glob.svg)](https://travis-ci.org/jonschlinkert/is-glob) 

> Returns `true` if the given string looks like a glob pattern.

## Install with [npm](npmjs.org)

```bash
npm i is-glob --save
```

## Usage

```js
var isGlob = require('is-glob');

isGlob('foo.js');
//=> 'false'
isGlob('!foo.js');
//=> 'true'
isGlob('*.js');
//=> 'true'
isGlob('**/abc.js');
//=> 'true'
isGlob('abc/*.js');
//=> 'true'
isGlob('abc/(aaa|bbb).js');
//=> 'true'
isGlob('abc/[a-z].js');
//=> 'true'
isGlob('abc/{a,b}.js');
//=> 'true'
isGlob('abc/?.js');
//=> 'true'
isGlob('abc.js');
//=> 'false'
isGlob('abc/def/ghi.js');
//=> 'false'
```

## Related
* [is-git-url](https://github.com/jonschlinkert/is-git-url): Regex to validate that a URL is a git url.
* [micromatch](https://github.com/jonschlinkert/micromatch): Glob matching for javascript/node.js. A drop-in replacement and faster alternative to minimatch and multimatch (10-45x faster on avg). Just use `minimatch.isMatch()` instead of `multimatch()` or `minimatch()`.
* [parse-glob](https://github.com/jonschlinkert/parse-glob): Parse a glob pattern into an object of tokens.

## Run tests
Install dev dependencies.

```bash
npm i -d && npm test
```

## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/is-glob/issues)

## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2015 Jon Schlinkert  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on March 14, 2015._