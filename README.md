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

All templates are stored in black and white (no transparent support). Use the tint feature to shift the color profile. The tint works as a basic color shift to the grayscale pixels.

|   | Red | Green | Blue |
|---|-----|-------|------|
| Original Pixel | 0 | 0 | 0 |
| Brown | 150 | 75 | 0 |
| Updated Pixel | 150 | 75 | 0 |

## Source

This was hacked together a while back and is one of those it meets my needs type projects, so it might not support everything. Would be interested to hear if you use this or find it useful. Contact me on Mastodon or open an issue in the tab above.

The source code is basically unreadable as each new feature was cobbled onto the last. I do want to do a full rewrite, but it might be a bit.

To develop, use node to or any service to startup a local http server.

```bash
npx http-server
```