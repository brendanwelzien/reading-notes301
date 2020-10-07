## Flexbox and Templating

Javascript Templating = technique used to render client-side view templates by using JSON
    - comprised of HTML markeup, with added templating tags that inserts variables  or runs programming logic
## Mustache
- logic-less template syntax... Used for HTML, config files, source code, etc.
- it works by expanding tags in a template using values provided in a *hash* or *object*
    - there are no **if-statements, else clauses, or for loops**
    - Mustache.render("Hello, {{name}}", { name: "Sherlynn" });
        - this returns **Hello, Sherylnn**
        - the two braces signify a **placeholder** and looks for name property in the code

## Flexbox
- idea behind flex layout is its ability to alter items' width and height to best fill space
- it is a direction-agnostic as opposed to regular layouts(which are vertically led and inline is horizontally led)
- lacks flexibility to support large apps
- appropriate for **small-scale layouts** while *Grid* is for **larger scale layouts**
    - items will be laid out following either the main axis from main-start to main-end
    - or following cross axis from cross-start to cross-end (y axis)

### PARENT PROPERTIES (FLEX CONTAINER)
- display: this defines a flex container; inline or block.. Gives flex content to direct children
- flex-direction: establishes main-axis (x) and gives direction of flex items
    - lays out either horizontally or vertically (row, row-reverse, column, column-reverse)
- flex-wrap: by default, all flex items will try to fit onto one line... you can change by...
    - wrap: wraps onto multiple lines, from top to bottom
    - wrap-reverse: flex items wraps multiple lines from bottom to top
- flex-flow: shorthand for *flex-direction* and *flex-wrap* properties, which defines the container's main and cross axes
    - the default value is row nowrap
- justify-content: this defines the alignment along the *main* axis, it helps distribute free space
    - gives some control over alignment of items when they overflow the line
    - flex-start: items packed toward start of flex-direction
    - flex-end: items packed toward end of flex-direction
    - start, end, left, space-around, space-between, space-evenly
- align-items: defines alignment along *cross* axis
    - uses stretch as default to fill container
    - flex-start, start, self-start
    - baseline: items aligned such as baselines align
- align-content: this aligns a flex container's lines within when there is extra space in cross-axis

### CHILDREN PROPERTIES (FLEX ITEMS)
- order: laid out in source order as default
- flex-grow: defines ability for flex item to grow if necessary, if a child is set to 2, it takes 2x space
- flex-shrink: defines ability for a flex item to shrink if necessary
- flex-basis: defines default size of an element before remaining space is distributed
- flex: shorthand for flex-grow, flex-shrink, and flex-basis (recommended)
- align-self: allows default alignment to be overriden for individual items
[<=Back](README.md)