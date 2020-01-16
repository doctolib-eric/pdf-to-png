# Browser-side PDF to PNG conversion

## Usage

```js
import pdfToPng from "pdf-to-png";

// [...]

const pngBlob = await pdfToPng(pdfBlob);
```

Take a [Blob](https://developer.mozilla.org/en-US/docs/Web/API/Blob) as its unique mandatory argument and returns another Blob.

Most of the time, the entry will be a very specific type of Blob, the [File](https://developer.mozilla.org/en-US/docs/Web/API/File).

## Caveats

Will only work within the context of a webpack-based project for now due to the hardcoded dependency to the webpack-configured version of PDF.js

## Development

### Release

```js
yarn prepublish
```

Inspired by ([this comment](https://stackoverflow.com/questions/29738381/how-to-publish-a-module-written-in-es6-to-npm/33976278#33976278))