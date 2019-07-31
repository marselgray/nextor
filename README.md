# Nextor

This is an advanced CSS and Sass project that uses CSS Grid.

### Planning/ Execution:
1. Overall layout

### Advanced CSS and Sass Concepts used:
1. CSS Grid
2. CSS Grid Techniques
3. Row/Column Track Sizes

###  Notes
CSS Grid:
- brings a 2D grid system to CSS
- works great with FlexBox
- display is set to grid with row axis and column axis
- grid items in a grid container 

```
grid-template-rows: 150px 150px;
grid-template-rows: repeat(2, 150px);
defines the heights of the rows

grid-template-columns: 150px 150px 150px;
grid-template-columns: repeat(2, 150px);
defines the heights of the columns

grid-row-gap: 30px;
puts a gap between the rows

grid-column-gap: 30px;
puts a gap between the column

grid-gap: 30px;
puts the same number gap between
rows and columns;
acts a combination of grid-row-gap
and grid-column-gap

grid-row-start: 2;
the row at which we want it start

grid-row-end: 3;
the row at which we want it end

these can be written in short hand as grid-row: 2/3;

grid-column-start: 2;
the column at which we want it start

grid-column-end: 3;
the column at which we want it end

these can be written in short hand as grid-column: 2/3;

a third short hand exists for a combination of grid-row and grid-column called grid-area with grid start, column start, grid end, and column end
the above example would be grid-area: 1 / 3 / 2 / 4;
```

Fractional Unit (fr):
- using repeat after grid-template-rows or columns means repeat for this number this length

- 1fr is  fraction of the available space

- grid-template-columns: 1fr 2fr 1fr; would mean 2fr would be 2x the size of the 1fr

- grid-template-columns: 50% 1fr 1fr; would mean 50% of the container width

The Difference Between Explicit and Implicit Grids:
- We can define a fixed number of lines and tracks that form a grid by using the properties grid-template-rows, grid-template-columns, and grid-template-areas. This manually defined grid is called the explicit grid.

- If there are more grid items than cells in the grid or when a grid item is placed outside of the explicit grid, the grid container automatically generates grid tracks by adding grid lines to the grid. The explicit grid together with these additional implicit tracks and lines forms the so called implicit grid.

- use you can use this code below to help with auto setting additional items
```
grid-auto-columns: 200px;
grid-auto-rows: 60px;
grid-auto-flow: rows (or columns);
```

Advanced CSS Grid: Min-Content/ Max-Content/ MinMax()
- min-content can be used to take the min content
- max-content can be used to take the max content
- minmax(250px, 1fr) allows you to create grid tracks that flex to the available space, but that don’t shrink narrower than a specified size; first value is min second value is max

Advanced CSS Grid: Auto Fit and Auto Fill
Auto-fill creates the number of tracks needed to fit the container
Auto-fit creates the number of tracks needed to fit the container while collapsing the unfilled tracks
```
grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
```

### Final Product:

**Desktop**

<!-- ![](project-large.jpg) -->

**Mobile**

<!-- ![](project-small.jpg) -->

#### Future Developers:
`npm install`

`live-server` to run live server

`npm start` to compile sass into css && watch for changes

ENJOY!