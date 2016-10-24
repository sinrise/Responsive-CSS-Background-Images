# Responsive-CSS-Background-Images

This leverages the programmatic aspects of Sass (SCSS) in order to save a ton of typing and a make easier to maintain responsive background images. This is particularly useful for things like hero images if your site has lots of pages, or (the reason I developed this method) to quickly output the styles I need for a carousel with responsive images.

If you have even 5 pages each with 4 slides, that's 20 background images you must include in your stylesheet. That's a lot to type. This method makes it easy as you only have to type the area (sub-folder), name of the class and the file name (without extension).

This SCSS script outputs a media query for screen width, pixel depth or both, for each size you specify. The demo shows 5 sizes: XL, LG, MD, SM, XS but it can be easily adapted for any number/combination of sizes.

Prerequisites:
You must use a file naming convention. In the demo, the script uses a set of contants for screen widths, an array of slides, and an array of sizes, including the abbreviation (as $key) and the width constant ($screen-*).

The size loop includes the abbreviation and width connstant because of limitations of concatenation in Sass. There may in fact be a slightly DRYer way to do this but this is pretty clean as it is.

Any advice/forks/complaints/comments welcome! :)
