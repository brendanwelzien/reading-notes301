# CSS Grid
- A more advanced tool compared to flexbox.. Better suited for larger-scale adjustments
    - changes columns/rows in multiples
    - gives control over how wide/narrow each grid cell gets
    - utilized by `grid-template-columns`

- to prevent images from *distorting* we can use `object-fit: cover;`

- the `grid-gap` property defines size of space between columns and rows,

## Parent Properties

Properties | Values
---------- | -------
Display | grid: generates block-level inline-grid: generates inline-level
grid-template-columns | defines columns of grid with separated list of values track-size: unit for space
grid-template-rows | defines rows of grid with separated list of values track-size: unit for space
grid-template-areas (defines template by referencing names of grid areas specified by *grid-area* property) | `<grid-area-name>` is name of grid area . = empty grid cell
grid-template | shorthand for rows, columns, areas
gap/grid-gap | gives length values
justify-items(inline row axis) | start, end, center, stretch
align-items(block column axis) | start, end, center, stretch


## Child Properties

Properties | Values
---------- | -------
grid-column-start (grid-column is shorthand)| starting point
grid-column-end | ending point
grid-row-start(grid-row is shorthand) | starting point
grid-row-end | ending point 
grid-area | manipulates area of grid
justify-self | aligns a grid item along inline row axis
align-self | aligns a grid item along block column axis
place-self | sets both align/justify in a single declaration


[<=Back](README.md)