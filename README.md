# Pocket Journal Generator

Generate 3.5" x 5" Pocket Notebook Journals.

## Usage

https://templarian.github.io/journal-generator/

Steps to use the app are in the left section of the app.

## Features

- Lots of Templates
  - 1/4 inch, 1 cm, 5 mm
  - Template text placement
- Page Numbers
  - Font selection
  - Optional page numbers on detail page
- Printer Tweaks
  - Offset pages to correct for printer alignment
    - Cover and Inner are saved seperately as these often use different page weights
- Custom Text Overlay
  - Preview and save presets.
  - Font selection
- Persistent Configs
  - All setting changes and custom template uploads persist.

## Request New Templates

Use the issues tab to request new templates. Explain the new template request or upload an image.

For templates with dynamic text use the export accessible from the dropdown to generate the JSON.

**Note:** All templates need a base grid measurement (inch, cm, or mm). Text values use this as their unit of measure. Page number placement will vary slightly based on this value.

## Templates

All built-in templates are stored in black and white. Templates must have a base color of hex #AAA or RGB 170, 170, 170.

## Detail / Inner Page Opacity

- 75% Opacity
  - Text
  - Checkbox Squares
- 50% Opacity
  - Dots / Lines
  - Drawing guidance lines
- 25% Opacity
  - Secondary drawing guidance lines
  - Symbols or Info Boxes
  - Watermarks

### Tint

Use the tint feature to shift the color profile to the newly selected color.

A common cover paper when making journals is a light brown. Using the out of the box grayscale template without a tint will produced a washed out print. To correct for this select the preset tint `Light Brown`.

Similarly when printing journals a small amount of color give each journal a more unique look. Try tinting the grid template with the `Blue Print`.

> Note: These color profiles are tested on an calibrated CYMK Epson, but will vary based on the paper and your intended design.

### Fade

The fade feature is primarily used when printing on non-white paper to allow the natural paper's colors pop. Pixels are grouped by brightness and given a opacity modifier. Essentially letting the natural paper's color from being washed out by the ink.

> The process of picking the right fade will require test printing. There are too many variables in play especially when printing on different paper types.

## Source

This was hacked together a while back and is one of those it meets my needs type projects, so it might not support everything. Would be interested to hear if you use this or find it useful. Contact me on Mastodon or open an issue in the tab above.

The source code is basically unreadable as each new feature was cobbled onto the last. I do want to do a full rewrite, but it might be a bit.

To develop, use node to or any service to startup a local http server.

```bash
npx http-server
```

## Specific Paper

What paper should I use? To make this easy I'll simply say [Field Notes](https://fieldnotesbrand.com/) knows more about paper than I'll ever be able to explain. As someone that owns hundreds of their notebooks I'll recommend doing the same and decide which is your favorite that way. The specification tab or the back of the notebook will list the paper used.

While the official supplier may not ship to an individual you can usually find it through a larger seller. Not all paper comes in letter size unfortantly, so if you don't have a paper cutter it might not be an option.

### Cover

[Packing Brown Wrap Cardstock (Dur-O-Tone, Cover Weight)](https://www.frenchpaper.com/products/packing-brown-wrap-cardstock-dur-o-tone-cover?variant=39835421245619)
> If you like [Field Notes](https://fieldnotesbrand.com/products/original-kraft) this is the same paper. This is not the same as craft paper and will print in a inkjet printer!

### Inner

There are two types of paper you'll be looking at.
- Text - This is your standard copy paper.
- Writing - This paper has a bit more texture, but is difficult to find as it usually comes in non-letter sized and has to be cut down.

[Smooth, 96 Bright White Paper (Finch Opaque Digital, Text Weight)](https://www.frenchpaper.com/products/smooth-96-white-paper-finch-opaque-digital-text-weight)
> This is almost always sold out, but is also what [Field Notes](https://fieldnotesbrand.com/products/original-kraft) uses.

HP Paper - BrightWhite 24 lb 100 Bright
> You want 96 or 100 Bright White at 24 lb or 60 lb text.
