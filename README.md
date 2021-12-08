# Shapes

[![npm version](http://img.shields.io/npm/v/elr-scss-shapes.svg)](https://www.npmjs.org/package/elr-scss-shapes)
[![CI](https://github.com/Beth3346/elr-scss-shapes/actions/workflows/node.js.yml/badge.svg)](https://github.com/Beth3346/elr-scss-shapes/actions/workflows/node.js.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm](https://img.shields.io/npm/dm/elr-scss-shapes.svg?style=flat)](https://npmjs.com/package/elr-scss-shapes)

some scss mixins for shapes

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install elr-scss-shapes
```

or

```sh
yarn add elr-scss-shapes
```

## Implementation

- height "half" will be half of the base
- height "auto" will be the same height as the base
- right triangles will always be equal width and height

```scss
@import "elr-scss-shapes/src/main";
```

```scss
.triangle-top {
  @include elr-triangle(
    $config: (
      base: 100px,
      height: "half",
      color: $primary-color,
      direction: "top",
    )
  );
}
```

```scss
.triangle-right {
  @include elr-triangle(
    $config: (
      base: 100px,
      direction: "right",
    )
  );
}
```

```scss
.triangle-bottom {
  @include elr-triangle(
    $config: (
      base: 100px,
      direction: "bottom",
    )
  );
}
```

```scss
.triangle-left {
  @include elr-triangle(
    $config: (
      base: 100px,
      direction: "left",
    )
  );
}
```

```scss
.triangle-top-right {
  @include elr-triangle(
    $config: (
      base: 100px,
      direction: "top-right",
    )
  );
}
```

```scss
.triangle-bottom-right {
  @include elr-triangle(
    $config: (
      base: 100px,
      direction: "bottom-right",
    )
  );
}
```

```scss
.triangle-top-left {
  @include elr-triangle(
    $config: (
      base: 100px,
      direction: "top-left",
    )
  );
}
```

```scss
.triangle-bottom-left {
  @include elr-triangle(
    $config: (
      base: 100px,
      direction: "bottom-left",
    )
  );
}
```

## License

SEE LICENSE IN LICENSE.md
