# My HTML/CSS Journey

> The source about design and code with HTML/CSS.

## Tutorials

- [HTML Tutorial - W3Schools](https://www.w3schools.com/html/)
- [HTML Tutorial - Tutorials Point](https://www.tutorialspoint.com/html/index.htm)
- [HTML Tutorial - JavaTpoint](https://www.javatpoint.com/html-tutorial)
- [CSS Tutorial - W3Schools](https://www.w3schools.com/css/default.asp)
- [CSS Tutorial - Tutorials Point](https://www.tutorialspoint.com/css/index.htm)
- [CSS Tutorial - JavaTpoint](https://www.javatpoint.com/css-tutorial)

## Courses

- [HTML & CSS Crash Course - Scrimba](https://scrimba.com/learn/htmlcss)
- [Learn CSS Variables for free - Scrimba](https://scrimba.com/learn/cssvariables)
- [Introduction to CSS - Scrimba](https://scrimba.com/learn/introtocss)
- [Introduction to HTML - Scrimba](https://scrimba.com/learn/html)
- [Learn Flexbox for free - Scrimba](https://scrimba.com/learn/flexbox)
- [Learn CSS Grid for free - Scrimba](https://scrimba.com/learn/cssgrid)

## BEM

[BEM](http://getbem.com/)

> Block Element Modifier is a methodology that helps you to create reusable components and code sharing in front-end development

**Block**

```html
<div class="block"></div>
```

```css
.block {
  color: #042;
}
```

**Element**

```html
<div class="block">
  <span class="block__elem"></span>
</div>
```

```css
.block__elem {
  color: #042;
}
```

**Modifier**

```html
<div class="block block--mod"></div>
<div class="block block--size-big block--shadow-yes"></div>
```

```css
.block--hidden {
}
.block--mod .block__elem {
}
.block__elem--mod {
}
```

**Example**

```html
<form class="form form--theme-xmas form--simple">
  <input class="form__input" type="text" />
  <input class="form__submit form__submit--disabled" type="submit" />
</form>
```

```css
.form {
}
.form--theme-xmas {
}
.form--simple {
}
.form__input {
}
.form__submit {
}
.form__submit--disabled {
}
```
