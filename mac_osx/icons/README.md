# macOS icons

This folder contains vector graphics to create the macOS icons from.

There are two variants for 16x16 sized and 32x32 sized icons.
In both variants, the stroke width of the logo is increased to keep it at least
someone legible on the small icon sizes. The 16x16 stroke width is even heavier
than the 32x32 stroke width.

Use the SVG files to generate the following PNG file in folder ending with
`.iconset` (use grayscale with alpha channel):

* `icon_16x16.png`
* `icon_16x16@2x.png'
* `icon_32x32.png`
* `icon_32x32@2x.png'

Then the folder can be converted to an ICNS file with `iconutil`:

```shell
iconutil -c icns -o output.icns input.iconset
```

The ICNS file can then be assigned to the respective layout in the bundle file
with Ukelele.

