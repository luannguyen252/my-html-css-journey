# CSS Flexbox

[CSS Flexbox Tutorial](https://www.quackit.com/css/flexbox/tutorial/)

[CSS Flexbox Examples](https://www.quackit.com/css/flexbox/examples/)

[Flexbox Cheat Sheet](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

1. display

> Enables flex for all children.

```css
display: flex;
display: inline-flex;
```

2. flex-direction

> Establishes the main axis.

```css
flex-direction: row;
flex-direction: row-reverse;
flex-direction: column;
flex-direction: column-reverse;
```

3. flex-wrap

> Wraps items if they can't all be made to fit on one line.

```css
flex-wrap: nowrap;
flex-wrap: wrap;
flex-wrap: wrap-reverse;
```

4. justify-content

> Attempts to distribute extra space on the main axis.

```css
justify-content: flex-start;
justify-content: flex-end;
justify-content: center;
justify-content: space-between;
justify-content: space-around;
justify-content: space-evenly;
```

5. align-items

> Determines how items are laid out on the cross axis.

```css
align-items: flex-start;
align-items: flex-end;
align-items: center;
align-items: baseline;
align-items: stretch;
```

6. align-content

> Only has an effect with more than one line of content. Examples shown here use flex-wrap.

```css
align-content: flex-start;
align-content: flex-end;
align-content: center;
align-content: space-between;
align-content: space-around;
align-content: stretch;
```
