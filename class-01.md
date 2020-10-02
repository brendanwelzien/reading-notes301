# SMACCS and Responsive Web Design

## Shay Howe's Intro to RWD
Responsive web design is the practice of building a website that is suited to work across all platforms, it is intuitive.

*Responsive vs Adaptive vs Mobile*
- responsive and adaptive refer to fluid change based on factors
- mobile means to build a separate website commonly on a new domain for mobile users (usually is not a good idea)

- Responsive web design is broken into 3 parts...
    1. flexible layouts
    2. media queries
    3. flexible media
1. flexible layouts is practice of building layout of a website dynamically using units %, em, then integrated into width, margin, and padding 
    - responsive viewport lengths= vw, vh, vmin, vmax
    - formula for **identifying** proportions of a flexible layout using relative values...
        - **target / context = result**
2. media queries: an extension to media types, specifies styles for browser and devices
- use the *media* tag inside linked style sheet
- *import* a new style sheet
- *link* to a separate style sheet within HTML document   
    - you can then specify the media type (all, screen(default), print, tv, and braille)

*Logical Operators in Media Queries*
- logical operators in media queries build powerful expressions
operators:
- and
    - extra condition to be added
- not
    - negates the query, specifies others
- only
    - new, selects specified queries

- the most responsive design commonly uses min-width and max-width
- the **orientation** media feature determines if a device is in landscape or portrait orientation
```html
@media all and (orientation: landscape) {...}
```
- the **aspect-ratio** and **device-aspect-ratio** media features specify the width/height pixel ratio of target rendering area
    - the value for aspect is two positive integers separated by a forward slash 15 (width px) / 8 (height px)
- the **resolution** media feature specifies the pixel density in dots per inch or DPI

*Viewport Height and Width*
- for mobile devices it is recommended to use the **device-height** and **device-width** values

*Flexible Media*
- in scaling the changing in size of images, text, etc. it is valuable to use the **max-width** property with a value of **100%**
    - does not work well with all instances of media (usually embedded)
    - needs to be *absolutely* positioned within the parent element, needs a height of 0

## All About Floats
- property that gives text wrap
    - floated elements remain a part of the flow of the web page
    - **absolutely** positioned elements are *removed* from the flow of webpage and will not affect position of other elements 
- floats can be used to create *entire web layouts!*, stronger tools include `flexbox` and `grid`
    - floats are useful for layout in smaller instances
    - the `clear` property will move down the content past the float if you do not want it to be adjacent

[<=Back](README.md)