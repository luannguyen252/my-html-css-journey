# BEM

[BEM](http://getbem.com/)

1. Block

```html
<div class="block">
  <!-- ... -->
</div>
```

```css
.block {
  color: #042;
}
```

2. Element

```html
<div class="block">
  <!-- ... -->
  <span class="block__elem">
    <!-- ... -->
  </span>
</div>
```

```css
.block__elem {
  color: #042;
}
```

3. Modifier

```html
<div class="block block--hidden block--mod">
  <div class="block__elem block__elem--mod"></div>
</div>
<div class="block block--size-big block--shadow-yes">...</div>
```

```css
.block--hidden {
  /* ... */
}

.block--mod .block__elem {
  /* ... */
}

.block__elem--mod {
  /* ... */
}
```
