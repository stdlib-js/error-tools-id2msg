<!--

@license Apache-2.0

Copyright (c) 2022 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# id2msg

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Return an error message corresponding to a provided two-character error identifier.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

To use in Observable,

```javascript
id2msg = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/error-tools-id2msg@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var id2msg = require( 'path/to/vendor/umd/error-tools-id2msg/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/error-tools-id2msg@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
(function () {
    window.id2msg;
})();
})();
</script>
```

#### id2msg( id )

Returns an error message corresponding to a provided two-character error identifier.

```javascript
var v = id2msg( '8t' );
// e.g., returns 'invalid option. `%s` option must be an array. Option: `%s`.'
```

If provided an unrecognized error identifier, the function returns `null`.

```javascript
var v = id2msg( 'beep_boop' );
// returns null
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- TODO: better example -->

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/error-tools-id2msg@umd/browser.js"></script>
<script type="text/javascript">
(function () {
(function () {

var list;
var v;
var i;

list = [
    '01',
    '03',
    '8t',
    '0a',
    '9W'
];

for ( i = 0; i < list.length; i++ ) {
    v = list[ i ];
    console.log( 'id: "%s". msg: "%s".', v, id2msg( v ) );
}

})();
})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for describing a command-line interface. -->



<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- <license> -->

<!-- </license> -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/error-tools-id2msg.svg
[npm-url]: https://npmjs.org/package/@stdlib/error-tools-id2msg

[test-image]: https://github.com/stdlib-js/error-tools-id2msg/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/error-tools-id2msg/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/error-tools-id2msg/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/error-tools-id2msg?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/error-tools-id2msg.svg
[dependencies-url]: https://david-dm.org/stdlib-js/error-tools-id2msg/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/error-tools-id2msg/tree/deno
[umd-url]: https://github.com/stdlib-js/error-tools-id2msg/tree/umd
[esm-url]: https://github.com/stdlib-js/error-tools-id2msg/tree/esm
[branches-url]: https://github.com/stdlib-js/error-tools-id2msg/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/error-tools-id2msg/main/LICENSE

<!-- <related-links> -->

<!-- </related-links> -->

</section>

<!-- /.links -->
