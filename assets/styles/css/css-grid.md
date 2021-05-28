# CSS Grid

- [CSS Grid Tutoria - Quackit](https://www.quackit.com/css/grid/tutorial/)
- [CSS Grid Examples - Quackit](https://www.quackit.com/css/grid/examples/)
- [Grid Layout Generator - Layout It](https://grid.layoutit.com/)

1. display

> Establishes a new grid formatting context for children.

```css
display: grid;
display: inline-grid;
display: subgrid;
```

2. grid-template

> Defines the rows and columns of the grid.

```css
/* 1. */
grid-template-columns: 12px 12px 12px;
grid-template-rows: 12px 12px 12px;
/* 2. */
grid-template-columns: repeat(3, 12px);
grid-template-rows: repeat(3, auto);
/* 3. */
grid-template-columns: 8px auto 8px;
grid-template-rows: 8px auto 12px;
/* 4. */
grid-template-columns: 22% 22% auto;
grid-template-rows: 22% auto 22%;
```

3. grid-gap

> Specifies the size of column and row gutters.

```css
/* 1. */
grid-row-gap: 1px;
/* 2. */
grid-column-gap: 9px;
/* 3. */
grid-gap: 1px 9px;
/* 4. */
grid-gap: 6px;
```

4. justify-items

> Aligns content in a grid item along the row axis.

```css
justify-items: start;
justify-items: end;
justify-items: center;
justify-items: stretch;
```

5. align-items

> ligns content in a grid item along the column axis.

```css
align-items: start;
align-items: end;
align-items: center;
align-items: stretch;
```

6. justify-content

> Justifies all grid content on row axis when total grid size is smaller than container.

```css
justify-content: start;
justify-content: end;
justify-content: center;
justify-content: stretch;
justify-content: space-around;
justify-content: space-between;
justify-content: space-evenly;
```

7. align-content

> Justifies all grid content on column axis when total grid size is smaller than container.

```css
align-content: start;
align-content: end;
align-content: center;
align-content: stretch;
align-content: space-around;
align-content: space-between;
align-content: space-evenly;
```

8. grid-auto-flow

> Algorithm for automatically placing grid items that aren't explictly placed.

```css
grid-auto-flow: row;
grid-auto-flow: column;
grid-auto-flow: dense;
```

9. grid-column

> Determines an items column-based location within the grid.

```css
/* 1. */
grid-column-start: 1;
grid-column-end: 3;
/* 2. */
grid-column-start: span 3;
/* 3. */
grid-column-start: 2;
grid-column-end: 4;
/* 4. */
grid-column: 2 / 3
/* 5. */
grid-column: 2 / span 2
```

10. grid-row

> Determines an items row-based location within the grid.

```css
/* 1. */
grid-row-start: 1;
grid-row-end: 3;
/* 2. */
grid-row-start: span 3;
/* 3. */
grid-row-start: 2;
grid-row-end: 4;
/* 4. */
grid-row: 1 / 3;
/* 5. */
grid-row: 1 / span 3;
```

11. grid-row + grid-column

> Combining grid rows with grid columns.

```css
/* 1. */
grid-row: 1 / span 2;
grid-column: 1 / span 2;
/* 2. */
grid-row: 2 / span 2;
grid-column: 2 / span 2;
```

12. justify-self

> Aligns content for a specific grid item along the row axis.

```css
justify-self: start;
justify-self: end;
justify-self: center;
justify-self: stretch;
```

13. align-self

> Aligns content for a specific grid item along the column axis.

```css
align-self: start;
align-self: end;
align-self: center;
align-self: stretch;
```
