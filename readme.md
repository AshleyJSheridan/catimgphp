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

This is the higher quality version that matches more closely the results of the original `catimg` tool. The colours on this are a little better with less blurring than `catimg`

![](https://raw.githubusercontent.com/AshleyJSheridan/catimgphp/master/examples/result_high_quality.jpg)

This is the older result from the initial attempt at the script

![](https://raw.githubusercontent.com/AshleyJSheridan/catimgphp/master/examples/result.jpg)

## Future Improvements

* Allow more detailed image drawing using block drawing characters ontop of the background colours
    * Improved quality using half block drawing characters and CLI foreground colours
* Support for transparency
* Improve speed of renders
    * Speed initially reduced to less than 23× the time taken for the first attempt
    * This speed gap was lessened when the higher quality was added, and now is only 18× faster
    * Speed comparison for a like-for-like CLI render of the same size in the `catimg` written in `C` is: the `C` version is about twice as fast as the `PHP` version on the PHP7 engine

## License

[MIT](http://opensource.org/licenses/MIT)

