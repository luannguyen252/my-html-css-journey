# My HTML/CSS Journey

> The source about design and code with HTML/CSS.

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
