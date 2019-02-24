# svg-halftone

[![Travis Build Status](https://api.travis-ci.org/evestera/svg-halftone.svg?branch=master)](https://travis-ci.org/evestera/svg-halftone)
[![Appveyor build status](https://ci.appveyor.com/api/projects/status/github/evestera/svg-halftone?svg=true)](https://ci.appveyor.com/project/evestera/svg-halftone)

Tool for converting [raster] images (png, jpg, gif) to SVG [halftone] patterns
that can be cut on a laser cutter, turning the halftone dots into holes.

[raster]: https://en.wikipedia.org/wiki/Raster_graphics
[halftone]: https://en.wikipedia.org/wiki/Halftone

## Installation

There are precompiled binaries of releases on [the releases page](https://github.com/evestera/svg-halftone/releases).

If you have [Rust installed](https://rustup.rs/) you can build from source with:

```bash
cargo install --git https://github.com/evestera/svg-halftone
```

## Usage

```bash
svg-halftone my-image.jpg
```

### Options

From `svg-halftone --help`

- `--grid <grid>`: Grid to lay samples out on. "rect", "hex", "diamond" or "poisson" [default: rect]
- `--output <output>`: Output path [default: out.svg]
- `--output-width <output-width>`: Output width in mm [default: 300]
- `--shape <shape>`: Shape used for samples. "circle" or "diamond" [default: circle]
- `--spacing <spacing>`: Horizontal spacing between samples in mm [default: 5]

## Useful programs/tools

- [remove.bg](https://www.remove.bg/): Easily replace backgrounds of images of people with a single color.

- [Gapplin](http://gapplin.wolfrosch.com/) (macOS): SVG viewer which automatically redraws the file when it is updated.

## License

This project is licensed under the MIT License.