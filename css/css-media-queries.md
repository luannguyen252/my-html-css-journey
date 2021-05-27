# CSS Media Queries

[A Complete Guide to CSS Media Queries](https://css-tricks.com/a-complete-guide-to-css-media-queries/)

[Media Queries for Standard Devices](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

**Anatomy of a Media Query**

```css
@media [media-type] ([media-feature]) {
  /* ... */
}
```

`[media-type]`:

- `all`: Matches all devices
- `print`: Matches documents that are viewed in a print preview or any media that breaks the content up into pages intended to print.
- `screen`: Matches devices with a screen

`[media-feature]`:

- `width`: Defines the widths of the viewport.
- `height`: Defines the height of the viewport.
- `aspect-ratio`: Defines the width-to-height aspect ratio of the viewport
- `orientation`: The way the screen is oriented, such as tall (portrait) or wide (landscape) based on how the device is rotated.

```css
/* When the browser is at least 600px and above */
@media screen and (min-width: 600px) {
  .element {
    /* Apply some styles */
  }
}
```

1. HTML

```html
<html>
  <head>
    <!-- Served to all users -->
    <link rel="stylesheet" href="all.css" media="all" />
    <!-- Served to screens that are at least 20em wide -->
    <link rel="stylesheet" href="small.css" media="(min-width: 20em)" />
    <!-- Served to screens that are at least 64em wide -->
    <link rel="stylesheet" href="medium.css" media="(min-width: 64em)" />
    <!-- Served to screens that are at least 90em wide -->
    <link rel="stylesheet" href="large.css" media="(min-width: 90em)" />
    <!-- Served to screens that are at least 120em wide -->
    <link rel="stylesheet" href="extra-large.css" media="(min-width: 120em)" />
    <!-- Served to print media, like printers -->
    <link rel="stylesheet" href="print.css" media="print" />
  </head>
  <!-- ... -->
</html>
```

2. CSS

```css
/* Viewports between 320px and 480px wide */
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
  .element {
    /* ... */
  }
}
/* Matches screen between 320px AND 768px */
@media screen (min-width: 320px) and (max-width: 768px) {
  .element {
    /* ... */
  }
}
```

Avoid using `@import` if possible!

```css
/* Base styles for all screens */
@import url("style.css") screen;
/* Styles for screens in a portrait (narrow) orientation */
@import url("landscape.css") screen and (orientation: portrait);
/* Print styles */
@import url("print.css") print;
```

3. Using min- and max- to match value ranges

```css
body {
  background-color: #fff;
}

@media (min-width: 30em) and (max-width: 80em) {
  body {
    background-color: #000;
  }
}
```

4. Target an iPhone in landscape mode

```css
/* iPhone X Landscape */
@media only screen and (min-device-width: 375px) and (max-device-width: 812px) and (-webkit-min-device-pixel-ratio: 3) and (orientation: landscape) {
  /* Styles! */
}
```

5. `prefers-color-scheme`

```css
body {
  --bg-color: white;
  --text-color: black;

  background-color: var(--bg-color);
  color: var(--text-color);
}

@media screen and (prefers-color-scheme: light) {
  body {
    --bg-color: black;
    --text-color: white;
  }
}
```
