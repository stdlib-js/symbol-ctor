<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

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

# Symbol

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] [![dependencies][dependencies-image]][dependencies-url]

> [Symbol][mdn-symbol] factory.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->

<section class="installation">

## Installation

```bash
npm install @stdlib/symbol-ctor
```

</section>

<section class="usage">

## Usage

```javascript
var Symbol = require( '@stdlib/symbol-ctor' );
```

#### Symbol( \[description] )

Returns a [`Symbol`][mdn-symbol] primitive.

<!-- run-disable -->

<!-- eslint-disable symbol-description -->

```javascript
var s = Symbol();
// returns <symbol>
```

To aid debugging, provide a [symbol][mdn-symbol] `description`.

<!-- run-disable -->

```javascript
var s = Symbol( 'beep' );
// returns <symbol>
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

## Notes

-   Unlike conventional constructors, the function does **not** support the `new` keyword.
-   The function is only supported in environments which support [symbols][mdn-symbol]. In non-supporting environments, the value is `undefined`.

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var hasSymbolSupport = require( '@stdlib/assert-has-symbol-support' );
var Symbol = require( '@stdlib/symbol-ctor' );

var s;

if ( hasSymbolSupport() ) {
    s = Symbol( 'beep' );

    // Print the value type:
    console.log( typeof s );
    // => 'symbol'

    // Serialize the symbol as a string:
    console.log( s.toString() );
    // => 'Symbol(beep)'

    // Test symbol equality:
    console.log( s === Symbol( 'beep' ) );
    // => false
} else {
    console.log( 'Environment does not support symbols.' );
}
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

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

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/symbol-ctor.svg
[npm-url]: https://npmjs.org/package/@stdlib/symbol-ctor

[test-image]: https://github.com/stdlib-js/symbol-ctor/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/symbol-ctor/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/symbol-ctor/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/symbol-ctor?branch=main

[dependencies-image]: https://img.shields.io/david/stdlib-js/symbol-ctor.svg
[dependencies-url]: https://david-dm.org/stdlib-js/symbol-ctor/main

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/symbol-ctor/main/LICENSE

[mdn-symbol]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol

</section>

<!-- /.links -->
