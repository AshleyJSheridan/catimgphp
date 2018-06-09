# CatImgPHP

A simple silly tool used to display a preview of an image on the command line using escape code sequences.

This was inspired by the [`catimg` tool written in C](https://github.com/posva/catimg).

Like that tool, this requires the use of a terminal that supports 256 colours.

## Installation

Checkout the source and make the `catimgphp` file executable.

Add to path if desired as a globally available tool

### Requirements

* PHP CLI
* GD

## Usage

```sh
catimgphp /path/to/image/file
```

Currently, only JPG, GIF, and PNG images are supported because of the use of GD to read in the source image.

## Results

![](https://raw.githubusercontent.com/AshleyJSheridan/catimgphp/master/examples/result.jpg)

## Future Improvements

* Allow more detailed image drawing using block drawing characters ontop of the background colours
* Support for transparency
* Improve speed of renders

## License

[MIT](http://opensource.org/licenses/MIT)

