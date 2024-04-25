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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Assert

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Assertion utilities.

<section class="installation">

## Installation

```bash
npm install @zibuthe7j11/provident-incidunt-ipsum
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var assert = require( '@zibuthe7j11/provident-incidunt-ipsum' );
```

#### assert

Namespace providing utilities for data type testing and feature detection.

```javascript
var o = assert;
// returns {...}
```

To validate the built-in JavaScript data types, the namespace includes the following assertion utilities:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array.</span>
-   <span class="signature">[`isBoolean( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-boolean]</span><span class="delimiter">: </span><span class="description">test if a value is a boolean.</span>
-   <span class="signature">[`isDateObject( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-date-object]</span><span class="delimiter">: </span><span class="description">test if a value is a Date object.</span>
-   <span class="signature">[`isFunction( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-function]</span><span class="delimiter">: </span><span class="description">test if a value is a function.</span>
-   <span class="signature">[`isnan( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nan]</span><span class="delimiter">: </span><span class="description">test if a value is NaN.</span>
-   <span class="signature">[`isNull( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-null]</span><span class="delimiter">: </span><span class="description">test if a value is null.</span>
-   <span class="signature">[`isNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number.</span>
-   <span class="signature">[`isObject( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-object]</span><span class="delimiter">: </span><span class="description">test if a value is an object.</span>
-   <span class="signature">[`isRegExp( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-regexp]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression.</span>
-   <span class="signature">[`isString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-string]</span><span class="delimiter">: </span><span class="description">test if a value is a string.</span>
-   <span class="signature">[`isSymbol( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-symbol]</span><span class="delimiter">: </span><span class="description">test if a value is a symbol.</span>
-   <span class="signature">[`isUndefined( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-undefined]</span><span class="delimiter">: </span><span class="description">test if a value is undefined.</span>

</div>

<!-- </toc> -->

For primitive types having corresponding object wrappers, assertion utilities provide `isObject` and `isPrimitive` methods to test for either objects or primitives, respectively.

<!-- eslint-disable no-new-wrappers -->

```javascript
var Boolean = require( '@stdlib/boolean/ctor' );
var isBoolean = require( '@zibuthe7j11/provident-incidunt-ipsum/is-boolean' );

var bool = isBoolean.isObject( new Boolean( false ) );
// returns true

bool = isBoolean.isObject( false );
// returns false

bool = isBoolean.isPrimitive( false );
// returns true
```

Many of the assertion utilities have corresponding packages that test whether array elements are of the given data type:

<!-- <toc pattern="is-+(array|boolean|date-object|function|string|nan|number|object|regexp|symbol|null|undefined)-array" > -->

<div class="namespace-toc">

-   <span class="signature">[`isArrayArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-array-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of arrays.</span>
-   <span class="signature">[`isBooleanArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-boolean-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of booleans.</span>
-   <span class="signature">[`isDateObjectArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-date-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only Date objects.</span>
-   <span class="signature">[`isFunctionArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-function-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only functions.</span>
-   <span class="signature">[`isNaNArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nan-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only NaN values.</span>
-   <span class="signature">[`isNullArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-null-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only null values.</span>
-   <span class="signature">[`isNumberArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object of numbers.</span>
-   <span class="signature">[`isObjectArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only objects.</span>
-   <span class="signature">[`isStringArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-string-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of strings.</span>
-   <span class="signature">[`isSymbolArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-symbol-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only symbols.</span>

</div>

<!-- </toc> -->

Where applicable, similar to the assertion utilities for built-in data types, array assertion utilities provides methods for testing for an array of primitives or objects.

<!-- eslint-disable no-new-wrappers -->

```javascript
var isStringArray = require( '@zibuthe7j11/provident-incidunt-ipsum/is-string-array' );

var bool = isStringArray( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.primitives( [ 'hello', 'world' ] );
// returns true

bool = isStringArray.objects( [ 'hello', 'world' ] );
// returns false

bool = isStringArray.objects( [ new String( 'hello' ), new String( 'world' ) ] );
// returns true
```

The namespace also contains utilities to test for numbers within a certain range or for numbers satisfying a particular "type":

<!-- <toc pattern="is-*+(number|integer)*" ignore="is-number-array" ignore="is-number" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCubeNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-cube-number]</span><span class="delimiter">: </span><span class="description">test if a value is a cube number.</span>
-   <span class="signature">[`isIntegerArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only integers.</span>
-   <span class="signature">[`isInteger( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having an integer value.</span>
-   <span class="signature">[`isNegativeIntegerArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-negative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative integers.</span>
-   <span class="signature">[`isNegativeInteger( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-negative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative integer value.</span>
-   <span class="signature">[`isNegativeNumberArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-negative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only negative numbers.</span>
-   <span class="signature">[`isNegativeNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-negative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a negative value.</span>
-   <span class="signature">[`isNonNegativeIntegerArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative integers.</span>
-   <span class="signature">[`isNonNegativeInteger( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative integer value.</span>
-   <span class="signature">[`isNonNegativeNumberArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonnegative numbers.</span>
-   <span class="signature">[`isNonNegativeNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative value.</span>
-   <span class="signature">[`isNonPositiveIntegerArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive integers.</span>
-   <span class="signature">[`isNonPositiveInteger( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive integer value.</span>
-   <span class="signature">[`isNonPositiveNumberArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only nonpositive numbers.</span>
-   <span class="signature">[`isNonPositiveNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonpositive value.</span>
-   <span class="signature">[`isPositiveIntegerArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-positive-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive integers.</span>
-   <span class="signature">[`isPositiveInteger( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-positive-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive integer value.</span>
-   <span class="signature">[`isPositiveNumberArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-positive-number-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only positive numbers.</span>
-   <span class="signature">[`isPositiveNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-positive-number]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a positive value.</span>
-   <span class="signature">[`isSafeIntegerArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-safe-integer-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only safe integers.</span>
-   <span class="signature">[`isSafeInteger( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-safe-integer]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a safe integer value.</span>
-   <span class="signature">[`isSquareNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-square-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square number.</span>
-   <span class="signature">[`isSquareTriangularNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-square-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a square triangular number.</span>
-   <span class="signature">[`isTriangularNumber( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-triangular-number]</span><span class="delimiter">: </span><span class="description">test if a value is a triangular number.</span>

</div>

<!-- </toc> -->

The namespace provides utilities for validating typed arrays:

<!-- <toc pattern="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array"> -->

<div class="namespace-toc">

-   <span class="signature">[`isFloat32Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float32Array.</span>
-   <span class="signature">[`isFloat64Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Float64Array.</span>
-   <span class="signature">[`isInt16Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-int16array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int16Array.</span>
-   <span class="signature">[`isInt32Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-int32array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int32Array.</span>
-   <span class="signature">[`isInt8Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-int8array]</span><span class="delimiter">: </span><span class="description">test if a value is an Int8Array.</span>
-   <span class="signature">[`isUint16Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-uint16array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint16Array.</span>
-   <span class="signature">[`isUint32Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-uint32array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint32Array.</span>
-   <span class="signature">[`isUint8Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-uint8array]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8Array.</span>
-   <span class="signature">[`isUint8ClampedArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-uint8clampedarray]</span><span class="delimiter">: </span><span class="description">test if a value is a Uint8ClampedArray.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating `ndarray`s (n-dimensional arrays).

<!-- <toc keywords="+ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isCentrosymmetricMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a centrosymmetric matrix.</span>
-   <span class="signature">[`isComplex128MatrixLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex128matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128ndarrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex128ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex128VectorLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex128vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64MatrixLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64ndarrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isComplex64VectorLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision complex floating-point numbers.</span>
-   <span class="signature">[`isFloat32MatrixLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float32matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32ndarrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float32ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat32VectorLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float32vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing single-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64MatrixLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float64matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64ndarrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float64ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is an ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isFloat64VectorLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-float64vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object containing double-precision floating-point numbers.</span>
-   <span class="signature">[`isMatrixLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-matrix-like]</span><span class="delimiter">: </span><span class="description">test if a value is 2-dimensional ndarray-like object.</span>
-   <span class="signature">[`isndarrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-ndarray-like]</span><span class="delimiter">: </span><span class="description">test if a value is ndarray-like.</span>
-   <span class="signature">[`isNonSymmetricMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonsymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a non-symmetric matrix.</span>
-   <span class="signature">[`isPersymmetricMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a persymmetric matrix.</span>
-   <span class="signature">[`isSkewCentrosymmetricMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-skew-centrosymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-centrosymmetric matrix.</span>
-   <span class="signature">[`isSkewPersymmetricMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-skew-persymmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-persymmetric matrix.</span>
-   <span class="signature">[`isSkewSymmetricMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-skew-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a skew-symmetric matrix.</span>
-   <span class="signature">[`isSquareMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-square-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a 2-dimensional ndarray-like object having equal dimensions.</span>
-   <span class="signature">[`isSymmetricMatrix( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-symmetric-matrix]</span><span class="delimiter">: </span><span class="description">test if a value is a symmetric matrix.</span>
-   <span class="signature">[`isVectorLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-vector-like]</span><span class="delimiter">: </span><span class="description">test if a value is a 1-dimensional ndarray-like object.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating complex numbers and arrays of complex numbers:

<!-- <toc pattern="is-complex*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isComplexLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex-like]</span><span class="delimiter">: </span><span class="description">test if a value is a complex number-like object.</span>
-   <span class="signature">[`isComplexTypedArrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is complex-typed-array-like.</span>
-   <span class="signature">[`isComplexTypedArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a complex typed array.</span>
-   <span class="signature">[`isComplex( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit or 128-bit complex number.</span>
-   <span class="signature">[`isComplex128( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex128]</span><span class="delimiter">: </span><span class="description">test if a value is a 128-bit complex number.</span>
-   <span class="signature">[`isComplex128Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex128array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex128Array.</span>
-   <span class="signature">[`isComplex64( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex64]</span><span class="delimiter">: </span><span class="description">test if a value is a 64-bit complex number.</span>
-   <span class="signature">[`isComplex64Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-complex64array]</span><span class="delimiter">: </span><span class="description">test if a value is a Complex64Array.</span>

</div>

<!-- </toc> -->

The namespace includes utilities for validating other special arrays or buffers:

<!-- <toc pattern="is-*array*" ignore="is-+(int8|int16|int32|uint8clamped|uint8|uint16|uint32|float32|float64)array" ignore="is-*+(number|integer)*" ignore="is-+(array|boolean|date-object|function|string|nan|number|object|primitive|regexp|symbol|null|undefined)-array" ignore="is-array" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`isAccessorArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-accessor-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object supporting the accessor (get/set) protocol.</span>
-   <span class="signature">[`isArrayLength( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid array length.</span>
-   <span class="signature">[`isArrayLikeObject( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object.</span>
-   <span class="signature">[`isArrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is array-like.</span>
-   <span class="signature">[`isArrayBufferView( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-arraybuffer-view]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer view.</span>
-   <span class="signature">[`isArrayBuffer( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-arraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is an ArrayBuffer.</span>
-   <span class="signature">[`isBetweenArray( value, a, b[, left, right] )`][@zibuthe7j11/provident-incidunt-ipsum/is-between-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object where every element is between two values.</span>
-   <span class="signature">[`isBigInt64Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-bigint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt64Array.</span>
-   <span class="signature">[`isBigUint64Array( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-biguint64array]</span><span class="delimiter">: </span><span class="description">test if a value is a BigUint64Array.</span>
-   <span class="signature">[`isCircularArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-circular-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array containing a circular reference.</span>
-   <span class="signature">[`isEmptyArrayLikeObject( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-empty-array-like-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array-like object.</span>
-   <span class="signature">[`isEmptyArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-empty-array]</span><span class="delimiter">: </span><span class="description">test if a value is an empty array.</span>
-   <span class="signature">[`isFalsyArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-falsy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only falsy values.</span>
-   <span class="signature">[`isFiniteArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-finite-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only finite numbers.</span>
-   <span class="signature">[`isNumericArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-numeric-array]</span><span class="delimiter">: </span><span class="description">test if a value is a numeric array.</span>
-   <span class="signature">[`isPlainObjectArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-plain-object-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only plain objects.</span>
-   <span class="signature">[`isProbabilityArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only probabilities.</span>
-   <span class="signature">[`isSameArray( v1, v2 )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both generic arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex128Array( v1, v2 )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-complex128array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex128Arrays and have the same values.</span>
-   <span class="signature">[`isSameComplex64Array( v1, v2 )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-complex64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Complex64Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat32Array( v1, v2 )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-float32array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float32Arrays and have the same values.</span>
-   <span class="signature">[`isSameFloat64Array( v1, v2 )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-float64array]</span><span class="delimiter">: </span><span class="description">test if two arguments are both Float64Arrays and have the same values.</span>
-   <span class="signature">[`isSharedArrayBuffer( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-sharedarraybuffer]</span><span class="delimiter">: </span><span class="description">test if a value is a SharedArrayBuffer.</span>
-   <span class="signature">[`isTruthyArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-truthy-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array-like object containing only truthy values.</span>
-   <span class="signature">[`isTypedArrayLength( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-typed-array-length]</span><span class="delimiter">: </span><span class="description">test if a value is a valid typed array length.</span>
-   <span class="signature">[`isTypedArrayLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-typed-array-like]</span><span class="delimiter">: </span><span class="description">test if a value is typed-array-like.</span>
-   <span class="signature">[`isTypedArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-typed-array]</span><span class="delimiter">: </span><span class="description">test if a value is a typed array.</span>
-   <span class="signature">[`isUnityProbabilityArray( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-unity-probability-array]</span><span class="delimiter">: </span><span class="description">test if a value is an array of probabilities that sum to one.</span>

</div>

<!-- </toc> -->

To test for error objects, the namespace includes the following utilities:

<!-- <toc pattern="is-*error*" > -->

<div class="namespace-toc">

-   <span class="signature">[`isError( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-error]</span><span class="delimiter">: </span><span class="description">test if a value is an Error object.</span>
-   <span class="signature">[`isEvalError( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-eval-error]</span><span class="delimiter">: </span><span class="description">test if a value is an EvalError object.</span>
-   <span class="signature">[`isRangeError( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-range-error]</span><span class="delimiter">: </span><span class="description">test if a value is a RangeError object.</span>
-   <span class="signature">[`isReferenceError( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-reference-error]</span><span class="delimiter">: </span><span class="description">test if a value is a ReferenceError object.</span>
-   <span class="signature">[`isSyntaxError( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-syntax-error]</span><span class="delimiter">: </span><span class="description">test if a value is a SyntaxError object.</span>
-   <span class="signature">[`isTypeError( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-type-error]</span><span class="delimiter">: </span><span class="description">test if a value is a TypeError object.</span>
-   <span class="signature">[`isURIError( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-uri-error]</span><span class="delimiter">: </span><span class="description">test if a value is a URIError object.</span>

</div>

<!-- </toc> -->

The namespace exposes the following constants concerning the current running process:

<!-- <toc pattern="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|big-endian|node|web-worker|windows|docker|mobile|touch-device)" > -->

<div class="namespace-toc">

-   <span class="signature">[`IS_BIG_ENDIAN`][@zibuthe7j11/provident-incidunt-ipsum/is-big-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is big endian.</span>
-   <span class="signature">[`IS_BROWSER`][@zibuthe7j11/provident-incidunt-ipsum/is-browser]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web browser.</span>
-   <span class="signature">[`IS_DARWIN`][@zibuthe7j11/provident-incidunt-ipsum/is-darwin]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Darwin.</span>
-   <span class="signature">[`IS_DOCKER`][@zibuthe7j11/provident-incidunt-ipsum/is-docker]</span><span class="delimiter">: </span><span class="description">check if the process is running in a Docker container.</span>
-   <span class="signature">[`IS_ELECTRON_MAIN`][@zibuthe7j11/provident-incidunt-ipsum/is-electron-main]</span><span class="delimiter">: </span><span class="description">check if the runtime is the main Electron process.</span>
-   <span class="signature">[`IS_ELECTRON_RENDERER`][@zibuthe7j11/provident-incidunt-ipsum/is-electron-renderer]</span><span class="delimiter">: </span><span class="description">check if the runtime is the Electron renderer process.</span>
-   <span class="signature">[`IS_ELECTRON`][@zibuthe7j11/provident-incidunt-ipsum/is-electron]</span><span class="delimiter">: </span><span class="description">check if the runtime is Electron.</span>
-   <span class="signature">[`IS_LITTLE_ENDIAN`][@zibuthe7j11/provident-incidunt-ipsum/is-little-endian]</span><span class="delimiter">: </span><span class="description">check if an environment is little endian.</span>
-   <span class="signature">[`IS_MOBILE`][@zibuthe7j11/provident-incidunt-ipsum/is-mobile]</span><span class="delimiter">: </span><span class="description">check if the current environment is a mobile device.</span>
-   <span class="signature">[`IS_NODE`][@zibuthe7j11/provident-incidunt-ipsum/is-node]</span><span class="delimiter">: </span><span class="description">check if the runtime is Node.js.</span>
-   <span class="signature">[`IS_TOUCH_DEVICE`][@zibuthe7j11/provident-incidunt-ipsum/is-touch-device]</span><span class="delimiter">: </span><span class="description">check if the current environment is a touch device.</span>
-   <span class="signature">[`IS_WEB_WORKER`][@zibuthe7j11/provident-incidunt-ipsum/is-web-worker]</span><span class="delimiter">: </span><span class="description">check if the runtime is a web worker.</span>
-   <span class="signature">[`IS_WINDOWS`][@zibuthe7j11/provident-incidunt-ipsum/is-windows]</span><span class="delimiter">: </span><span class="description">boolean indicating if the current process is running on Windows.</span>

</div>

<!-- </toc> -->

To test whether a runtime environment supports certain features, the namespace includes the following utilities:

<!-- <toc pattern="has-*-support" > -->

<div class="namespace-toc">

-   <span class="signature">[`hasArrayBufferSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-arraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `ArrayBuffer` support.</span>
-   <span class="signature">[`hasArrowFunctionSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-arrow-function-support]</span><span class="delimiter">: </span><span class="description">detect native `arrow function` support.</span>
-   <span class="signature">[`hasAsyncAwaitSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-async-await-support]</span><span class="delimiter">: </span><span class="description">detect native `async`/`await` support.</span>
-   <span class="signature">[`hasAsyncIteratorSymbolSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-async-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.asyncIterator` support.</span>
-   <span class="signature">[`hasBigIntSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-bigint-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt` support.</span>
-   <span class="signature">[`hasBigInt64ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-bigint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigInt64Array` support.</span>
-   <span class="signature">[`hasBigUint64ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-biguint64array-support]</span><span class="delimiter">: </span><span class="description">detect native `BigUint64Array` support.</span>
-   <span class="signature">[`hasClassSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-class-support]</span><span class="delimiter">: </span><span class="description">detect native `class` support.</span>
-   <span class="signature">[`hasDataViewSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-dataview-support]</span><span class="delimiter">: </span><span class="description">detect native `DataView` support.</span>
-   <span class="signature">[`hasDefinePropertiesSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-define-properties-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperties` support.</span>
-   <span class="signature">[`hasDefinePropertySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-define-property-support]</span><span class="delimiter">: </span><span class="description">detect `Object.defineProperty` support.</span>
-   <span class="signature">[`hasFloat32ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-float32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float32Array` support.</span>
-   <span class="signature">[`hasFloat64ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-float64array-support]</span><span class="delimiter">: </span><span class="description">detect native `Float64Array` support.</span>
-   <span class="signature">[`hasFunctionNameSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-function-name-support]</span><span class="delimiter">: </span><span class="description">detect native function `name` support.</span>
-   <span class="signature">[`hasGeneratorSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-generator-support]</span><span class="delimiter">: </span><span class="description">detect native `generator function` support.</span>
-   <span class="signature">[`hasGlobalThisSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-globalthis-support]</span><span class="delimiter">: </span><span class="description">detect `globalThis` support.</span>
-   <span class="signature">[`hasInt16ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-int16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int16Array` support.</span>
-   <span class="signature">[`hasInt32ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-int32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int32Array` support.</span>
-   <span class="signature">[`hasInt8ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-int8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Int8Array` support.</span>
-   <span class="signature">[`hasIteratorSymbolSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-iterator-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.iterator` support.</span>
-   <span class="signature">[`hasMapSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-map-support]</span><span class="delimiter">: </span><span class="description">detect native `Map` support.</span>
-   <span class="signature">[`hasNodeBufferSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-node-buffer-support]</span><span class="delimiter">: </span><span class="description">detect native `Buffer` support.</span>
-   <span class="signature">[`hasProxySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-proxy-support]</span><span class="delimiter">: </span><span class="description">detect native `Proxy` support.</span>
-   <span class="signature">[`hasSetSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-set-support]</span><span class="delimiter">: </span><span class="description">detect native `Set` support.</span>
-   <span class="signature">[`hasSharedArrayBufferSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-sharedarraybuffer-support]</span><span class="delimiter">: </span><span class="description">detect native `SharedArrayBuffer` support.</span>
-   <span class="signature">[`hasSymbolSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-symbol-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol` support.</span>
-   <span class="signature">[`hasToStringTagSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-tostringtag-support]</span><span class="delimiter">: </span><span class="description">detect native `Symbol.toStringTag` support.</span>
-   <span class="signature">[`hasUint16ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-uint16array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint16Array` support.</span>
-   <span class="signature">[`hasUint32ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-uint32array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint32Array` support.</span>
-   <span class="signature">[`hasUint8ArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-uint8array-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8Array` support.</span>
-   <span class="signature">[`hasUint8ClampedArraySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-uint8clampedarray-support]</span><span class="delimiter">: </span><span class="description">detect native `Uint8ClampedArray` support.</span>
-   <span class="signature">[`hasWebAssemblySupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-wasm-support]</span><span class="delimiter">: </span><span class="description">detect native WebAssembly support.</span>
-   <span class="signature">[`hasWeakMapSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-weakmap-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakMap` support.</span>
-   <span class="signature">[`hasWeakSetSupport()`][@zibuthe7j11/provident-incidunt-ipsum/has-weakset-support]</span><span class="delimiter">: </span><span class="description">detect native `WeakSet` support.</span>

</div>

<!-- </toc> -->

The remaining namespace utilities are as follows:

<!-- <toc ignore="is-+(array|boolean|date-object|function|string|symbol|nan|null|number|object|regexp|symbol|undefined)" ignore="is-*+(number|integer)*" ignore="is-*array*" ignore="is-*error*" ignore="is-+(browser|darwin|electron|electron-main|electron-renderer|little-endian|node|web-worker|windows)" ignore="has-*-support" keywords="-ndarray" > -->

<div class="namespace-toc">

-   <span class="signature">[`contains( val, searchValue[, position] )`][@zibuthe7j11/provident-incidunt-ipsum/contains]</span><span class="delimiter">: </span><span class="description">test if an array-like value contains a search value.</span>
-   <span class="signature">[`deepEqual( a, b )`][@zibuthe7j11/provident-incidunt-ipsum/deep-equal]</span><span class="delimiter">: </span><span class="description">test for deep equality between two values.</span>
-   <span class="signature">[`deepHasOwnProp( value, path[, options] )`][@zibuthe7j11/provident-incidunt-ipsum/deep-has-own-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path.</span>
-   <span class="signature">[`deepHasProp( value, path[, options] )`][@zibuthe7j11/provident-incidunt-ipsum/deep-has-property]</span><span class="delimiter">: </span><span class="description">test whether an object contains a nested key path, either own or inherited.</span>
-   <span class="signature">[`hasOwnProp( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/has-own-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property.</span>
-   <span class="signature">[`hasProp( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/has-property]</span><span class="delimiter">: </span><span class="description">test if an object has a specified property, either own or inherited.</span>
-   <span class="signature">[`hasUTF16SurrogatePairAt( string, position )`][@zibuthe7j11/provident-incidunt-ipsum/has-utf16-surrogate-pair-at]</span><span class="delimiter">: </span><span class="description">test if a position in a string marks the start of a UTF-16 surrogate pair.</span>
-   <span class="signature">[`instanceOf( value, constructor )`][@zibuthe7j11/provident-incidunt-ipsum/instance-of]</span><span class="delimiter">: </span><span class="description">test whether a value has in its prototype chain a specified constructor as a prototype property.</span>
-   <span class="signature">[`isAbsoluteHttpURI( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-absolute-http-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute HTTP(S) URI.</span>
-   <span class="signature">[`isAbsolutePath( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-absolute-path]</span><span class="delimiter">: </span><span class="description">test if a value is an absolute path.</span>
-   <span class="signature">[`isAbsoluteURI( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-absolute-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is an absolute URI.</span>
-   <span class="signature">[`isAccessorPropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-accessor-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has an accessor descriptor.</span>
-   <span class="signature">[`isAccessorProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-accessor-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has an accessor descriptor.</span>
-   <span class="signature">[`isAlphagram( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-alphagram]</span><span class="delimiter">: </span><span class="description">test if a value is an alphagram.</span>
-   <span class="signature">[`isAlphaNumeric( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-alphanumeric]</span><span class="delimiter">: </span><span class="description">test whether a string contains only alphanumeric characters.</span>
-   <span class="signature">[`isAnagram( str, value )`][@zibuthe7j11/provident-incidunt-ipsum/is-anagram]</span><span class="delimiter">: </span><span class="description">test if a value is an anagram.</span>
-   <span class="signature">[`isArguments( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-arguments]</span><span class="delimiter">: </span><span class="description">test if a value is an arguments object.</span>
-   <span class="signature">[`isArrowFunction( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-arrow-function]</span><span class="delimiter">: </span><span class="description">test if a value is an `arrow function`.</span>
-   <span class="signature">[`isASCII( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-ascii]</span><span class="delimiter">: </span><span class="description">test whether a character belongs to the ASCII character set and whether this is true for all characters in a provided string.</span>
-   <span class="signature">[`isBetween( value, a, b[, left, right] )`][@zibuthe7j11/provident-incidunt-ipsum/is-between]</span><span class="delimiter">: </span><span class="description">test if a value is between two values.</span>
-   <span class="signature">[`isBigInt( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-bigint]</span><span class="delimiter">: </span><span class="description">test if a value is a BigInt.</span>
-   <span class="signature">[`isBinaryString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-binary-string]</span><span class="delimiter">: </span><span class="description">test if a value is a binary string.</span>
-   <span class="signature">[`isBlankString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-blank-string]</span><span class="delimiter">: </span><span class="description">test if a value is a blank string.</span>
-   <span class="signature">[`isBoxedPrimitive( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-boxed-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript boxed primitive.</span>
-   <span class="signature">[`isBuffer( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a Buffer object.</span>
-   <span class="signature">[`isCamelcase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-camelcase]</span><span class="delimiter">: </span><span class="description">test if a value is a camelcase string.</span>
-   <span class="signature">[`isCapitalized( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-capitalized]</span><span class="delimiter">: </span><span class="description">test if a value is a string having an uppercase first character.</span>
-   <span class="signature">[`isCircular( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-circular]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object containing a circular reference.</span>
-   <span class="signature">[`isCircular( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-circular]</span><span class="delimiter">: </span><span class="description">test if an object-like value contains a circular reference.</span>
-   <span class="signature">[`isClass( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-class]</span><span class="delimiter">: </span><span class="description">test if a value is a class.</span>
-   <span class="signature">[`isCollection( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-collection]</span><span class="delimiter">: </span><span class="description">test if a value is a collection.</span>
-   <span class="signature">[`isComposite( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-composite]</span><span class="delimiter">: </span><span class="description">test if a value is a composite number.</span>
-   <span class="signature">[`isConfigurablePropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-configurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is configurable.</span>
-   <span class="signature">[`isConfigurableProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-configurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is configurable.</span>
-   <span class="signature">[`isConstantcase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-constantcase]</span><span class="delimiter">: </span><span class="description">test if a value is a constantcase string.</span>
-   <span class="signature">[`isCurrentYear( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-current-year]</span><span class="delimiter">: </span><span class="description">test if a value is the current year.</span>
-   <span class="signature">[`isDataPropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-data-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property has a data descriptor.</span>
-   <span class="signature">[`isDataProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-data-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property has a data descriptor.</span>
-   <span class="signature">[`isDataView( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-dataview]</span><span class="delimiter">: </span><span class="description">test if a value is a DataView.</span>
-   <span class="signature">[`isDigitString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-digit-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only numeric digits.</span>
-   <span class="signature">[`isDomainName( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-domain-name]</span><span class="delimiter">: </span><span class="description">test if a value is a domain name.</span>
-   <span class="signature">[`isDurationString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-duration-string]</span><span class="delimiter">: </span><span class="description">test if a value is a duration string.</span>
-   <span class="signature">[`isEmailAddress( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-email-address]</span><span class="delimiter">: </span><span class="description">test if a value is an email address.</span>
-   <span class="signature">[`isEmptyCollection( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-empty-collection]</span><span class="delimiter">: </span><span class="description">test if a value is an empty collection.</span>
-   <span class="signature">[`isEmptyObject( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-empty-object]</span><span class="delimiter">: </span><span class="description">test if a value is an empty object.</span>
-   <span class="signature">[`isEmptyString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-empty-string]</span><span class="delimiter">: </span><span class="description">test if a value is an empty string.</span>
-   <span class="signature">[`isEnumerablePropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-enumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is enumerable.</span>
-   <span class="signature">[`isEnumerableProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-enumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is enumerable.</span>
-   <span class="signature">[`isEven( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-even]</span><span class="delimiter">: </span><span class="description">test if a value is an even number.</span>
-   <span class="signature">[`isFalsy( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-falsy]</span><span class="delimiter">: </span><span class="description">test if a value is falsy.</span>
-   <span class="signature">[`isFinite( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a finite number.</span>
-   <span class="signature">[`isGeneratorObjectLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-generator-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is `generator` object-like.</span>
-   <span class="signature">[`isGeneratorObject( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-generator-object]</span><span class="delimiter">: </span><span class="description">test if a value is a `generator` object.</span>
-   <span class="signature">[`isgzipBuffer( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-gzip-buffer]</span><span class="delimiter">: </span><span class="description">test if a value is a gzip buffer.</span>
-   <span class="signature">[`isHexString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-hex-string]</span><span class="delimiter">: </span><span class="description">test whether a string contains only hexadecimal digits.</span>
-   <span class="signature">[`isInfinite( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-infinite]</span><span class="delimiter">: </span><span class="description">test if a value is an infinite number.</span>
-   <span class="signature">[`isInheritedProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-inherited-property]</span><span class="delimiter">: </span><span class="description">test if an object has an inherited property.</span>
-   <span class="signature">[`isIterableLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-iterable-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterable`-like.</span>
-   <span class="signature">[`isIteratorLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-iterator-like]</span><span class="delimiter">: </span><span class="description">test if a value is `iterator`-like.</span>
-   <span class="signature">[`isJSON( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-json]</span><span class="delimiter">: </span><span class="description">test if a value is a parseable JSON string.</span>
-   <span class="signature">[`isKebabcase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-kebabcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in kebab case.</span>
-   <span class="signature">[`isLeapYear( [value] )`][@zibuthe7j11/provident-incidunt-ipsum/is-leap-year]</span><span class="delimiter">: </span><span class="description">test if a value corresponds to a leap year in the Gregorian calendar.</span>
-   <span class="signature">[`isLocalhost( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-localhost]</span><span class="delimiter">: </span><span class="description">test whether a value is a localhost hostname.</span>
-   <span class="signature">[`isLowercase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-lowercase]</span><span class="delimiter">: </span><span class="description">test if a value is a lowercase string.</span>
-   <span class="signature">[`isMethodIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-method-in]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name, either own or inherited.</span>
-   <span class="signature">[`isMethod( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-method]</span><span class="delimiter">: </span><span class="description">test if an object has a specified method name.</span>
-   <span class="signature">[`isMultiSlice( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-multi-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `MultiSlice`.</span>
-   <span class="signature">[`isNamedTypedTupleLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-named-typed-tuple-like]</span><span class="delimiter">: </span><span class="description">test if a value is named typed tuple-like.</span>
-   <span class="signature">[`isNativeFunction( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-native-function]</span><span class="delimiter">: </span><span class="description">test if a value is a native function.</span>
-   <span class="signature">[`isNegativeZero( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-negative-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to negative zero.</span>
-   <span class="signature">[`isNodeBuiltin( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-node-builtin]</span><span class="delimiter">: </span><span class="description">test whether a string matches a Node.js built-in module name.</span>
-   <span class="signature">[`isNodeDuplexStreamLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-node-duplex-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node duplex stream-like.</span>
-   <span class="signature">[`isNodeReadableStreamLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-node-readable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node readable stream-like.</span>
-   <span class="signature">[`isNodeREPL()`][@zibuthe7j11/provident-incidunt-ipsum/is-node-repl]</span><span class="delimiter">: </span><span class="description">check if running in a Node.js REPL environment.</span>
-   <span class="signature">[`isNodeStreamLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-node-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node stream-like.</span>
-   <span class="signature">[`isNodeTransformStreamLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-node-transform-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node transform stream-like.</span>
-   <span class="signature">[`isNodeWritableStreamLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-node-writable-stream-like]</span><span class="delimiter">: </span><span class="description">test if a value is Node writable stream-like.</span>
-   <span class="signature">[`isNonConfigurablePropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonconfigurable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-configurable.</span>
-   <span class="signature">[`isNonConfigurableProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonconfigurable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-configurable.</span>
-   <span class="signature">[`isNonEnumerablePropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonenumerable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is non-enumerable.</span>
-   <span class="signature">[`isNonEnumerableProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonenumerable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is non-enumerable.</span>
-   <span class="signature">[`isNonNegativeFinite( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-finite]</span><span class="delimiter">: </span><span class="description">test if a value is a number having a nonnegative finite value.</span>
-   <span class="signature">[`isObjectLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is object-like.</span>
-   <span class="signature">[`isOdd( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-odd]</span><span class="delimiter">: </span><span class="description">test if a value is an odd number.</span>
-   <span class="signature">[`isPascalcase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-pascalcase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in Pascal case.</span>
-   <span class="signature">[`isPlainObject( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-plain-object]</span><span class="delimiter">: </span><span class="description">test if a value is a plain object.</span>
-   <span class="signature">[`isPositiveZero( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-positive-zero]</span><span class="delimiter">: </span><span class="description">test if a value is a number equal to positive zero.</span>
-   <span class="signature">[`isPrime( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-prime]</span><span class="delimiter">: </span><span class="description">test if a value is a prime number.</span>
-   <span class="signature">[`isPrimitive( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-primitive]</span><span class="delimiter">: </span><span class="description">test if a value is a JavaScript primitive.</span>
-   <span class="signature">[`isPRNGLike( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-prng-like]</span><span class="delimiter">: </span><span class="description">test if a value is PRNG-like.</span>
-   <span class="signature">[`isProbability( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-probability]</span><span class="delimiter">: </span><span class="description">test if a value is a probability.</span>
-   <span class="signature">[`isPropertyKey( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-property-key]</span><span class="delimiter">: </span><span class="description">test whether a value is a property key.</span>
-   <span class="signature">[`isPrototypeOf( obj, prototype )`][@zibuthe7j11/provident-incidunt-ipsum/is-prototype-of]</span><span class="delimiter">: </span><span class="description">test if an object's prototype chain contains a provided prototype.</span>
-   <span class="signature">[`isReadOnlyPropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-read-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is read-only.</span>
-   <span class="signature">[`isReadOnlyProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-read-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is read-only.</span>
-   <span class="signature">[`isReadWritePropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-read-write-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable and writable.</span>
-   <span class="signature">[`isReadWriteProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-read-write-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable and writable.</span>
-   <span class="signature">[`isReadablePropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-readable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is readable.</span>
-   <span class="signature">[`isReadableProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-readable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is readable.</span>
-   <span class="signature">[`isRegExpString( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-regexp-string]</span><span class="delimiter">: </span><span class="description">test if a value is a regular expression string.</span>
-   <span class="signature">[`isRelativePath( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-relative-path]</span><span class="delimiter">: </span><span class="description">test if a value is a relative path.</span>
-   <span class="signature">[`isRelativeURI( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-relative-uri]</span><span class="delimiter">: </span><span class="description">test whether a value is a relative URI.</span>
-   <span class="signature">[`isSameComplex128( v1, v2 )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-complex128]</span><span class="delimiter">: </span><span class="description">test if two arguments are both double-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameComplex64( v1, v2 )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-complex64]</span><span class="delimiter">: </span><span class="description">test if two arguments are both single-precision complex floating-point numbers and have the same value.</span>
-   <span class="signature">[`isSameNativeClass( a, b )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-native-class]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same native class.</span>
-   <span class="signature">[`isSameType( a, b )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-type]</span><span class="delimiter">: </span><span class="description">test if two arguments have the same type.</span>
-   <span class="signature">[`isSameValueZero( a, b )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-value-zero]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSameValue( a, b )`][@zibuthe7j11/provident-incidunt-ipsum/is-same-value]</span><span class="delimiter">: </span><span class="description">test if two arguments are the same value.</span>
-   <span class="signature">[`isSemVer( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-semver]</span><span class="delimiter">: </span><span class="description">test if a value is a semantic version string.</span>
-   <span class="signature">[`isSlice( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-slice]</span><span class="delimiter">: </span><span class="description">test if a value is a `Slice`.</span>
-   <span class="signature">[`isSnakecase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-snakecase]</span><span class="delimiter">: </span><span class="description">test if a value is a string in snake case.</span>
-   <span class="signature">[`isStartcase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-startcase]</span><span class="delimiter">: </span><span class="description">test if a value is a startcase string.</span>
-   <span class="signature">[`isStrictEqual( a, b )`][@zibuthe7j11/provident-incidunt-ipsum/is-strict-equal]</span><span class="delimiter">: </span><span class="description">test if two arguments are strictly equal.</span>
-   <span class="signature">[`isTruthy( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-truthy]</span><span class="delimiter">: </span><span class="description">test if a value is truthy.</span>
-   <span class="signature">[`isUNCPath( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-unc-path]</span><span class="delimiter">: </span><span class="description">test if a value is a UNC path.</span>
-   <span class="signature">[`isUndefinedOrNull( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-undefined-or-null]</span><span class="delimiter">: </span><span class="description">test if a value is undefined or null.</span>
-   <span class="signature">[`isUppercase( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-uppercase]</span><span class="delimiter">: </span><span class="description">test if a value is an uppercase string.</span>
-   <span class="signature">[`isURI( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-uri]</span><span class="delimiter">: </span><span class="description">test if a value is a URI.</span>
-   <span class="signature">[`isWhitespace( value )`][@zibuthe7j11/provident-incidunt-ipsum/is-whitespace]</span><span class="delimiter">: </span><span class="description">test whether a string contains only white space characters.</span>
-   <span class="signature">[`isWritablePropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-writable-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is writable.</span>
-   <span class="signature">[`isWritableProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-writable-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is writable.</span>
-   <span class="signature">[`isWriteOnlyPropertyIn( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-write-only-property-in]</span><span class="delimiter">: </span><span class="description">test if an object's own or inherited property is write-only.</span>
-   <span class="signature">[`isWriteOnlyProperty( value, property )`][@zibuthe7j11/provident-incidunt-ipsum/is-write-only-property]</span><span class="delimiter">: </span><span class="description">test if an object's own property is write-only.</span>
-   <span class="signature">[`tools`][@zibuthe7j11/provident-incidunt-ipsum/tools]</span><span class="delimiter">: </span><span class="description">assertion utility tools.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var assert = require( '@zibuthe7j11/provident-incidunt-ipsum' );

console.log( objectKeys( assert ) );
```

</section>

<!-- /.examples -->

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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@zibuthe7j11/provident-incidunt-ipsum.svg
[npm-url]: https://npmjs.org/package/@zibuthe7j11/provident-incidunt-ipsum

[test-image]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/zibuthe7j11/provident-incidunt-ipsum/main.svg
[coverage-url]: https://codecov.io/github/zibuthe7j11/provident-incidunt-ipsum?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/zibuthe7j11/provident-incidunt-ipsum.svg
[dependencies-url]: https://david-dm.org/zibuthe7j11/provident-incidunt-ipsum/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/deno
[deno-readme]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/blob/deno/README.md
[umd-url]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/umd
[umd-readme]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/blob/umd/README.md
[esm-url]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/esm
[esm-readme]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/blob/esm/README.md
[branches-url]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/zibuthe7j11/provident-incidunt-ipsum/main/LICENSE

<!-- <toc-links> -->

[@zibuthe7j11/provident-incidunt-ipsum/contains]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/contains

[@zibuthe7j11/provident-incidunt-ipsum/deep-equal]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/deep-equal

[@zibuthe7j11/provident-incidunt-ipsum/deep-has-own-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/deep-has-own-property

[@zibuthe7j11/provident-incidunt-ipsum/deep-has-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/deep-has-property

[@zibuthe7j11/provident-incidunt-ipsum/has-own-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-own-property

[@zibuthe7j11/provident-incidunt-ipsum/has-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-property

[@zibuthe7j11/provident-incidunt-ipsum/has-utf16-surrogate-pair-at]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-utf16-surrogate-pair-at

[@zibuthe7j11/provident-incidunt-ipsum/instance-of]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/instance-of

[@zibuthe7j11/provident-incidunt-ipsum/is-absolute-http-uri]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-absolute-http-uri

[@zibuthe7j11/provident-incidunt-ipsum/is-absolute-path]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-absolute-path

[@zibuthe7j11/provident-incidunt-ipsum/is-absolute-uri]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-absolute-uri

[@zibuthe7j11/provident-incidunt-ipsum/is-accessor-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-accessor-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-accessor-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-accessor-property

[@zibuthe7j11/provident-incidunt-ipsum/is-alphagram]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-alphagram

[@zibuthe7j11/provident-incidunt-ipsum/is-alphanumeric]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-alphanumeric

[@zibuthe7j11/provident-incidunt-ipsum/is-anagram]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-anagram

[@zibuthe7j11/provident-incidunt-ipsum/is-arguments]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-arguments

[@zibuthe7j11/provident-incidunt-ipsum/is-arrow-function]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-arrow-function

[@zibuthe7j11/provident-incidunt-ipsum/is-ascii]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-ascii

[@zibuthe7j11/provident-incidunt-ipsum/is-between]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-between

[@zibuthe7j11/provident-incidunt-ipsum/is-bigint]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-bigint

[@zibuthe7j11/provident-incidunt-ipsum/is-binary-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-binary-string

[@zibuthe7j11/provident-incidunt-ipsum/is-blank-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-blank-string

[@zibuthe7j11/provident-incidunt-ipsum/is-boxed-primitive]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-boxed-primitive

[@zibuthe7j11/provident-incidunt-ipsum/is-buffer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-buffer

[@zibuthe7j11/provident-incidunt-ipsum/is-camelcase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-camelcase

[@zibuthe7j11/provident-incidunt-ipsum/is-capitalized]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-capitalized

[@zibuthe7j11/provident-incidunt-ipsum/is-circular]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-circular

[@zibuthe7j11/provident-incidunt-ipsum/is-class]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-class

[@zibuthe7j11/provident-incidunt-ipsum/is-collection]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-collection

[@zibuthe7j11/provident-incidunt-ipsum/is-composite]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-composite

[@zibuthe7j11/provident-incidunt-ipsum/is-configurable-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-configurable-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-configurable-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-configurable-property

[@zibuthe7j11/provident-incidunt-ipsum/is-constantcase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-constantcase

[@zibuthe7j11/provident-incidunt-ipsum/is-current-year]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-current-year

[@zibuthe7j11/provident-incidunt-ipsum/is-data-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-data-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-data-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-data-property

[@zibuthe7j11/provident-incidunt-ipsum/is-dataview]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-dataview

[@zibuthe7j11/provident-incidunt-ipsum/is-digit-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-digit-string

[@zibuthe7j11/provident-incidunt-ipsum/is-domain-name]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-domain-name

[@zibuthe7j11/provident-incidunt-ipsum/is-duration-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-duration-string

[@zibuthe7j11/provident-incidunt-ipsum/is-email-address]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-email-address

[@zibuthe7j11/provident-incidunt-ipsum/is-empty-collection]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-empty-collection

[@zibuthe7j11/provident-incidunt-ipsum/is-empty-object]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-empty-object

[@zibuthe7j11/provident-incidunt-ipsum/is-empty-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-empty-string

[@zibuthe7j11/provident-incidunt-ipsum/is-enumerable-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-enumerable-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-enumerable-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-enumerable-property

[@zibuthe7j11/provident-incidunt-ipsum/is-even]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-even

[@zibuthe7j11/provident-incidunt-ipsum/is-falsy]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-falsy

[@zibuthe7j11/provident-incidunt-ipsum/is-finite]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-finite

[@zibuthe7j11/provident-incidunt-ipsum/is-generator-object-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-generator-object-like

[@zibuthe7j11/provident-incidunt-ipsum/is-generator-object]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-generator-object

[@zibuthe7j11/provident-incidunt-ipsum/is-gzip-buffer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-gzip-buffer

[@zibuthe7j11/provident-incidunt-ipsum/is-hex-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-hex-string

[@zibuthe7j11/provident-incidunt-ipsum/is-infinite]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-infinite

[@zibuthe7j11/provident-incidunt-ipsum/is-inherited-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-inherited-property

[@zibuthe7j11/provident-incidunt-ipsum/is-iterable-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-iterable-like

[@zibuthe7j11/provident-incidunt-ipsum/is-iterator-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-iterator-like

[@zibuthe7j11/provident-incidunt-ipsum/is-json]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-json

[@zibuthe7j11/provident-incidunt-ipsum/is-kebabcase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-kebabcase

[@zibuthe7j11/provident-incidunt-ipsum/is-leap-year]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-leap-year

[@zibuthe7j11/provident-incidunt-ipsum/is-localhost]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-localhost

[@zibuthe7j11/provident-incidunt-ipsum/is-lowercase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-lowercase

[@zibuthe7j11/provident-incidunt-ipsum/is-method-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-method-in

[@zibuthe7j11/provident-incidunt-ipsum/is-method]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-method

[@zibuthe7j11/provident-incidunt-ipsum/is-multi-slice]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-multi-slice

[@zibuthe7j11/provident-incidunt-ipsum/is-named-typed-tuple-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-named-typed-tuple-like

[@zibuthe7j11/provident-incidunt-ipsum/is-native-function]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-native-function

[@zibuthe7j11/provident-incidunt-ipsum/is-negative-zero]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-negative-zero

[@zibuthe7j11/provident-incidunt-ipsum/is-node-builtin]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node-builtin

[@zibuthe7j11/provident-incidunt-ipsum/is-node-duplex-stream-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node-duplex-stream-like

[@zibuthe7j11/provident-incidunt-ipsum/is-node-readable-stream-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node-readable-stream-like

[@zibuthe7j11/provident-incidunt-ipsum/is-node-repl]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node-repl

[@zibuthe7j11/provident-incidunt-ipsum/is-node-stream-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node-stream-like

[@zibuthe7j11/provident-incidunt-ipsum/is-node-transform-stream-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node-transform-stream-like

[@zibuthe7j11/provident-incidunt-ipsum/is-node-writable-stream-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node-writable-stream-like

[@zibuthe7j11/provident-incidunt-ipsum/is-nonconfigurable-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonconfigurable-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-nonconfigurable-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonconfigurable-property

[@zibuthe7j11/provident-incidunt-ipsum/is-nonenumerable-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonenumerable-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-nonenumerable-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonenumerable-property

[@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-finite]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonnegative-finite

[@zibuthe7j11/provident-incidunt-ipsum/is-object-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-object-like

[@zibuthe7j11/provident-incidunt-ipsum/is-odd]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-odd

[@zibuthe7j11/provident-incidunt-ipsum/is-pascalcase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-pascalcase

[@zibuthe7j11/provident-incidunt-ipsum/is-plain-object]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-plain-object

[@zibuthe7j11/provident-incidunt-ipsum/is-positive-zero]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-positive-zero

[@zibuthe7j11/provident-incidunt-ipsum/is-prime]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-prime

[@zibuthe7j11/provident-incidunt-ipsum/is-primitive]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-primitive

[@zibuthe7j11/provident-incidunt-ipsum/is-prng-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-prng-like

[@zibuthe7j11/provident-incidunt-ipsum/is-probability]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-probability

[@zibuthe7j11/provident-incidunt-ipsum/is-property-key]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-property-key

[@zibuthe7j11/provident-incidunt-ipsum/is-prototype-of]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-prototype-of

[@zibuthe7j11/provident-incidunt-ipsum/is-read-only-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-read-only-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-read-only-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-read-only-property

[@zibuthe7j11/provident-incidunt-ipsum/is-read-write-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-read-write-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-read-write-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-read-write-property

[@zibuthe7j11/provident-incidunt-ipsum/is-readable-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-readable-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-readable-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-readable-property

[@zibuthe7j11/provident-incidunt-ipsum/is-regexp-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-regexp-string

[@zibuthe7j11/provident-incidunt-ipsum/is-relative-path]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-relative-path

[@zibuthe7j11/provident-incidunt-ipsum/is-relative-uri]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-relative-uri

[@zibuthe7j11/provident-incidunt-ipsum/is-same-complex128]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-complex128

[@zibuthe7j11/provident-incidunt-ipsum/is-same-complex64]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-complex64

[@zibuthe7j11/provident-incidunt-ipsum/is-same-native-class]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-native-class

[@zibuthe7j11/provident-incidunt-ipsum/is-same-type]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-type

[@zibuthe7j11/provident-incidunt-ipsum/is-same-value-zero]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-value-zero

[@zibuthe7j11/provident-incidunt-ipsum/is-same-value]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-value

[@zibuthe7j11/provident-incidunt-ipsum/is-semver]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-semver

[@zibuthe7j11/provident-incidunt-ipsum/is-slice]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-slice

[@zibuthe7j11/provident-incidunt-ipsum/is-snakecase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-snakecase

[@zibuthe7j11/provident-incidunt-ipsum/is-startcase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-startcase

[@zibuthe7j11/provident-incidunt-ipsum/is-strict-equal]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-strict-equal

[@zibuthe7j11/provident-incidunt-ipsum/is-truthy]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-truthy

[@zibuthe7j11/provident-incidunt-ipsum/is-unc-path]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-unc-path

[@zibuthe7j11/provident-incidunt-ipsum/is-undefined-or-null]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-undefined-or-null

[@zibuthe7j11/provident-incidunt-ipsum/is-uppercase]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-uppercase

[@zibuthe7j11/provident-incidunt-ipsum/is-uri]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-uri

[@zibuthe7j11/provident-incidunt-ipsum/is-whitespace]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-whitespace

[@zibuthe7j11/provident-incidunt-ipsum/is-writable-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-writable-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-writable-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-writable-property

[@zibuthe7j11/provident-incidunt-ipsum/is-write-only-property-in]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-write-only-property-in

[@zibuthe7j11/provident-incidunt-ipsum/is-write-only-property]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-write-only-property

[@zibuthe7j11/provident-incidunt-ipsum/tools]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/tools

[@zibuthe7j11/provident-incidunt-ipsum/has-arraybuffer-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-arraybuffer-support

[@zibuthe7j11/provident-incidunt-ipsum/has-arrow-function-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-arrow-function-support

[@zibuthe7j11/provident-incidunt-ipsum/has-async-await-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-async-await-support

[@zibuthe7j11/provident-incidunt-ipsum/has-async-iterator-symbol-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-async-iterator-symbol-support

[@zibuthe7j11/provident-incidunt-ipsum/has-bigint-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-bigint-support

[@zibuthe7j11/provident-incidunt-ipsum/has-bigint64array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-bigint64array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-biguint64array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-biguint64array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-class-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-class-support

[@zibuthe7j11/provident-incidunt-ipsum/has-dataview-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-dataview-support

[@zibuthe7j11/provident-incidunt-ipsum/has-define-properties-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-define-properties-support

[@zibuthe7j11/provident-incidunt-ipsum/has-define-property-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-define-property-support

[@zibuthe7j11/provident-incidunt-ipsum/has-float32array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-float32array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-float64array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-float64array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-function-name-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-function-name-support

[@zibuthe7j11/provident-incidunt-ipsum/has-generator-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-generator-support

[@zibuthe7j11/provident-incidunt-ipsum/has-globalthis-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-globalthis-support

[@zibuthe7j11/provident-incidunt-ipsum/has-int16array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-int16array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-int32array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-int32array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-int8array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-int8array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-iterator-symbol-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-iterator-symbol-support

[@zibuthe7j11/provident-incidunt-ipsum/has-map-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-map-support

[@zibuthe7j11/provident-incidunt-ipsum/has-node-buffer-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-node-buffer-support

[@zibuthe7j11/provident-incidunt-ipsum/has-proxy-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-proxy-support

[@zibuthe7j11/provident-incidunt-ipsum/has-set-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-set-support

[@zibuthe7j11/provident-incidunt-ipsum/has-sharedarraybuffer-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-sharedarraybuffer-support

[@zibuthe7j11/provident-incidunt-ipsum/has-symbol-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-symbol-support

[@zibuthe7j11/provident-incidunt-ipsum/has-tostringtag-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-tostringtag-support

[@zibuthe7j11/provident-incidunt-ipsum/has-uint16array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-uint16array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-uint32array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-uint32array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-uint8array-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-uint8array-support

[@zibuthe7j11/provident-incidunt-ipsum/has-uint8clampedarray-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-uint8clampedarray-support

[@zibuthe7j11/provident-incidunt-ipsum/has-wasm-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-wasm-support

[@zibuthe7j11/provident-incidunt-ipsum/has-weakmap-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-weakmap-support

[@zibuthe7j11/provident-incidunt-ipsum/has-weakset-support]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/has-weakset-support

[@zibuthe7j11/provident-incidunt-ipsum/is-big-endian]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-big-endian

[@zibuthe7j11/provident-incidunt-ipsum/is-browser]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-browser

[@zibuthe7j11/provident-incidunt-ipsum/is-darwin]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-darwin

[@zibuthe7j11/provident-incidunt-ipsum/is-docker]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-docker

[@zibuthe7j11/provident-incidunt-ipsum/is-electron-main]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-electron-main

[@zibuthe7j11/provident-incidunt-ipsum/is-electron-renderer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-electron-renderer

[@zibuthe7j11/provident-incidunt-ipsum/is-electron]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-electron

[@zibuthe7j11/provident-incidunt-ipsum/is-little-endian]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-little-endian

[@zibuthe7j11/provident-incidunt-ipsum/is-mobile]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-mobile

[@zibuthe7j11/provident-incidunt-ipsum/is-node]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-node

[@zibuthe7j11/provident-incidunt-ipsum/is-touch-device]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-touch-device

[@zibuthe7j11/provident-incidunt-ipsum/is-web-worker]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-web-worker

[@zibuthe7j11/provident-incidunt-ipsum/is-windows]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-windows

[@zibuthe7j11/provident-incidunt-ipsum/is-error]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-error

[@zibuthe7j11/provident-incidunt-ipsum/is-eval-error]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-eval-error

[@zibuthe7j11/provident-incidunt-ipsum/is-range-error]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-range-error

[@zibuthe7j11/provident-incidunt-ipsum/is-reference-error]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-reference-error

[@zibuthe7j11/provident-incidunt-ipsum/is-syntax-error]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-syntax-error

[@zibuthe7j11/provident-incidunt-ipsum/is-type-error]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-type-error

[@zibuthe7j11/provident-incidunt-ipsum/is-uri-error]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-uri-error

[@zibuthe7j11/provident-incidunt-ipsum/is-accessor-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-accessor-array

[@zibuthe7j11/provident-incidunt-ipsum/is-array-length]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-array-length

[@zibuthe7j11/provident-incidunt-ipsum/is-array-like-object]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-array-like-object

[@zibuthe7j11/provident-incidunt-ipsum/is-array-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-array-like

[@zibuthe7j11/provident-incidunt-ipsum/is-arraybuffer-view]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-arraybuffer-view

[@zibuthe7j11/provident-incidunt-ipsum/is-arraybuffer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-arraybuffer

[@zibuthe7j11/provident-incidunt-ipsum/is-between-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-between-array

[@zibuthe7j11/provident-incidunt-ipsum/is-bigint64array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-bigint64array

[@zibuthe7j11/provident-incidunt-ipsum/is-biguint64array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-biguint64array

[@zibuthe7j11/provident-incidunt-ipsum/is-circular-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-circular-array

[@zibuthe7j11/provident-incidunt-ipsum/is-empty-array-like-object]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-empty-array-like-object

[@zibuthe7j11/provident-incidunt-ipsum/is-empty-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-empty-array

[@zibuthe7j11/provident-incidunt-ipsum/is-falsy-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-falsy-array

[@zibuthe7j11/provident-incidunt-ipsum/is-finite-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-finite-array

[@zibuthe7j11/provident-incidunt-ipsum/is-numeric-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-numeric-array

[@zibuthe7j11/provident-incidunt-ipsum/is-plain-object-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-plain-object-array

[@zibuthe7j11/provident-incidunt-ipsum/is-probability-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-probability-array

[@zibuthe7j11/provident-incidunt-ipsum/is-same-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-array

[@zibuthe7j11/provident-incidunt-ipsum/is-same-complex128array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-complex128array

[@zibuthe7j11/provident-incidunt-ipsum/is-same-complex64array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-complex64array

[@zibuthe7j11/provident-incidunt-ipsum/is-same-float32array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-float32array

[@zibuthe7j11/provident-incidunt-ipsum/is-same-float64array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-same-float64array

[@zibuthe7j11/provident-incidunt-ipsum/is-sharedarraybuffer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-sharedarraybuffer

[@zibuthe7j11/provident-incidunt-ipsum/is-truthy-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-truthy-array

[@zibuthe7j11/provident-incidunt-ipsum/is-typed-array-length]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-typed-array-length

[@zibuthe7j11/provident-incidunt-ipsum/is-typed-array-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-typed-array-like

[@zibuthe7j11/provident-incidunt-ipsum/is-typed-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-typed-array

[@zibuthe7j11/provident-incidunt-ipsum/is-unity-probability-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-unity-probability-array

[@zibuthe7j11/provident-incidunt-ipsum/is-complex-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex-like

[@zibuthe7j11/provident-incidunt-ipsum/is-complex-typed-array-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex-typed-array-like

[@zibuthe7j11/provident-incidunt-ipsum/is-complex-typed-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex-typed-array

[@zibuthe7j11/provident-incidunt-ipsum/is-complex]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex

[@zibuthe7j11/provident-incidunt-ipsum/is-complex128]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex128

[@zibuthe7j11/provident-incidunt-ipsum/is-complex128array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex128array

[@zibuthe7j11/provident-incidunt-ipsum/is-complex64]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex64

[@zibuthe7j11/provident-incidunt-ipsum/is-complex64array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex64array

[@zibuthe7j11/provident-incidunt-ipsum/is-centrosymmetric-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-centrosymmetric-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-complex128matrix-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex128matrix-like

[@zibuthe7j11/provident-incidunt-ipsum/is-complex128ndarray-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex128ndarray-like

[@zibuthe7j11/provident-incidunt-ipsum/is-complex128vector-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex128vector-like

[@zibuthe7j11/provident-incidunt-ipsum/is-complex64matrix-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex64matrix-like

[@zibuthe7j11/provident-incidunt-ipsum/is-complex64ndarray-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex64ndarray-like

[@zibuthe7j11/provident-incidunt-ipsum/is-complex64vector-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-complex64vector-like

[@zibuthe7j11/provident-incidunt-ipsum/is-float32matrix-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float32matrix-like

[@zibuthe7j11/provident-incidunt-ipsum/is-float32ndarray-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float32ndarray-like

[@zibuthe7j11/provident-incidunt-ipsum/is-float32vector-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float32vector-like

[@zibuthe7j11/provident-incidunt-ipsum/is-float64matrix-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float64matrix-like

[@zibuthe7j11/provident-incidunt-ipsum/is-float64ndarray-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float64ndarray-like

[@zibuthe7j11/provident-incidunt-ipsum/is-float64vector-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float64vector-like

[@zibuthe7j11/provident-incidunt-ipsum/is-matrix-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-matrix-like

[@zibuthe7j11/provident-incidunt-ipsum/is-ndarray-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-ndarray-like

[@zibuthe7j11/provident-incidunt-ipsum/is-nonsymmetric-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonsymmetric-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-persymmetric-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-persymmetric-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-skew-centrosymmetric-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-skew-centrosymmetric-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-skew-persymmetric-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-skew-persymmetric-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-skew-symmetric-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-skew-symmetric-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-square-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-square-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-symmetric-matrix]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-symmetric-matrix

[@zibuthe7j11/provident-incidunt-ipsum/is-vector-like]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-vector-like

[@zibuthe7j11/provident-incidunt-ipsum/is-float32array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float32array

[@zibuthe7j11/provident-incidunt-ipsum/is-float64array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-float64array

[@zibuthe7j11/provident-incidunt-ipsum/is-int16array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-int16array

[@zibuthe7j11/provident-incidunt-ipsum/is-int32array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-int32array

[@zibuthe7j11/provident-incidunt-ipsum/is-int8array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-int8array

[@zibuthe7j11/provident-incidunt-ipsum/is-uint16array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-uint16array

[@zibuthe7j11/provident-incidunt-ipsum/is-uint32array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-uint32array

[@zibuthe7j11/provident-incidunt-ipsum/is-uint8array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-uint8array

[@zibuthe7j11/provident-incidunt-ipsum/is-uint8clampedarray]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-uint8clampedarray

[@zibuthe7j11/provident-incidunt-ipsum/is-cube-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-cube-number

[@zibuthe7j11/provident-incidunt-ipsum/is-integer-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-integer-array

[@zibuthe7j11/provident-incidunt-ipsum/is-integer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-integer

[@zibuthe7j11/provident-incidunt-ipsum/is-negative-integer-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-negative-integer-array

[@zibuthe7j11/provident-incidunt-ipsum/is-negative-integer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-negative-integer

[@zibuthe7j11/provident-incidunt-ipsum/is-negative-number-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-negative-number-array

[@zibuthe7j11/provident-incidunt-ipsum/is-negative-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-negative-number

[@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-integer-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonnegative-integer-array

[@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-integer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonnegative-integer

[@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-number-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonnegative-number-array

[@zibuthe7j11/provident-incidunt-ipsum/is-nonnegative-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonnegative-number

[@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-integer-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonpositive-integer-array

[@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-integer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonpositive-integer

[@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-number-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonpositive-number-array

[@zibuthe7j11/provident-incidunt-ipsum/is-nonpositive-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nonpositive-number

[@zibuthe7j11/provident-incidunt-ipsum/is-positive-integer-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-positive-integer-array

[@zibuthe7j11/provident-incidunt-ipsum/is-positive-integer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-positive-integer

[@zibuthe7j11/provident-incidunt-ipsum/is-positive-number-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-positive-number-array

[@zibuthe7j11/provident-incidunt-ipsum/is-positive-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-positive-number

[@zibuthe7j11/provident-incidunt-ipsum/is-safe-integer-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-safe-integer-array

[@zibuthe7j11/provident-incidunt-ipsum/is-safe-integer]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-safe-integer

[@zibuthe7j11/provident-incidunt-ipsum/is-square-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-square-number

[@zibuthe7j11/provident-incidunt-ipsum/is-square-triangular-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-square-triangular-number

[@zibuthe7j11/provident-incidunt-ipsum/is-triangular-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-triangular-number

[@zibuthe7j11/provident-incidunt-ipsum/is-array-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-array-array

[@zibuthe7j11/provident-incidunt-ipsum/is-boolean-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-boolean-array

[@zibuthe7j11/provident-incidunt-ipsum/is-date-object-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-date-object-array

[@zibuthe7j11/provident-incidunt-ipsum/is-function-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-function-array

[@zibuthe7j11/provident-incidunt-ipsum/is-nan-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nan-array

[@zibuthe7j11/provident-incidunt-ipsum/is-null-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-null-array

[@zibuthe7j11/provident-incidunt-ipsum/is-number-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-number-array

[@zibuthe7j11/provident-incidunt-ipsum/is-object-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-object-array

[@zibuthe7j11/provident-incidunt-ipsum/is-string-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-string-array

[@zibuthe7j11/provident-incidunt-ipsum/is-symbol-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-symbol-array

[@zibuthe7j11/provident-incidunt-ipsum/is-array]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-array

[@zibuthe7j11/provident-incidunt-ipsum/is-boolean]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-boolean

[@zibuthe7j11/provident-incidunt-ipsum/is-date-object]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-date-object

[@zibuthe7j11/provident-incidunt-ipsum/is-function]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-function

[@zibuthe7j11/provident-incidunt-ipsum/is-nan]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-nan

[@zibuthe7j11/provident-incidunt-ipsum/is-null]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-null

[@zibuthe7j11/provident-incidunt-ipsum/is-number]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-number

[@zibuthe7j11/provident-incidunt-ipsum/is-object]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-object

[@zibuthe7j11/provident-incidunt-ipsum/is-regexp]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-regexp

[@zibuthe7j11/provident-incidunt-ipsum/is-string]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-string

[@zibuthe7j11/provident-incidunt-ipsum/is-symbol]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-symbol

[@zibuthe7j11/provident-incidunt-ipsum/is-undefined]: https://github.com/zibuthe7j11/provident-incidunt-ipsum/tree/main/is-undefined

<!-- </toc-links> -->

</section>

<!-- /.links -->
