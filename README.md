# Fylgja - Sass

[![NPM version](https://img.shields.io/npm/v/@fylgja/sass.svg)](https://www.npmjs.org/package/@fylgja/sass)

Adds more SCSS super powers functions.

This repo will add more functions that adds options
not found in the core sass project.

- [Installation](#installation)
- [How to use](#how-to-use)

## Installation

```bash
npm install @fylgja/sass
```

## How to use

Since this is a Sass function library it require only usages where it is needed.
So if you need to string replace something.

Then include the specific sass typed function via;

```scss
@use "@fylgja/sass/string" as str;

.str-replace {
    content: str.replace("Hello World", "World", "🌍");
}
```

We advice to use the library with a prefixed `@use`.
Similar to an `@use "sass:string"`.

This package offers the following functions.

| Function Name  | Type   | Description                                       |
| -------------- | ------ | ------------------------------------------------- |
| luminance      | color  | Calculate the luminance for a color               |
| contrast-ratio | color  | Calculate the contrast ratio between two colors   |
| contrast       | color  | Sets an dark or light color based on the contrast |
| gray           | color  | Get a specific gray based an a given precentage   |
| nth-side       | list   | Extract value based on shorthand sizing property  |
| strip-unit     | math   | Removes the unit (e.g. px, em, rem) from a value  |
| replace        | string | Replace part of a string with new value           |
| url-encode     | string | Encode Unsafe urls to safe urls                   |
| svg-url        | string | Use SVG anywhere as dataUri (inline background)   |
