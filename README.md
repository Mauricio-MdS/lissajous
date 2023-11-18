# Lissajous

Lissajous generates GIF animations of random [Lissajous figures](https://en.wikipedia.org/wiki/Lissajous_curve).

![gif example](./lissajous.gif)

These are exercises 1.5 and 1.6 from the book The Go Programming Language by Brian W. Kernighan and Alan Donovan.

## How to Run

To run the Lissajous program, use the following command:

```bash
go run lissajous.go [main_color] [background_color] > [file_name]
```

### Optional Arguments

- **main_color**: Specify the main color of the Lissajous figure. Options: black, white, red, green, blue, yellow, magenta, cyan. Defaults to green if not provided a valid option.

- **background_color**: Specify the background color of the GIF. Options: black, white, red, green, blue, yellow, magenta, cyan. Defaults to black if not provided a valid option.

## Example Usage

```bash
# Run with default colors (green on black)
go run lissajous.go > image.gif

# Run with custom colors
go run lissajous.go blue white > image2.gif
```

## Tasks

[ x ] Change the Lissajous program’s color palette to green on black, for added authenticity. To create the web color #RRGGBB, use color.RGBA{0xRR, 0xGG, 0xBB, 0xff}, where each pair of hexadecimal digits represents the intensity of the red, green, or blue component of the pixel.

[ x ] Modify the Lissajous program to produce images in multiple colors by adding more values to palette and then displaying them by changing the third argument of SetColorIndex in some interesting way.
