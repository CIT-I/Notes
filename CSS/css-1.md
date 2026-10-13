# CSS

## Selectors I

CSS selectors are patterns used to target and select specific elements for styling.

```css
/*
This selects all paragraph tags and changes the text color to green
*/

p {
  color: green;
}
```

## Where to add CSS

### Inline

Inline CSS is attached to a specific tag. It does not use selectors

```html
<!--
only this h1 tag will have this style applied to it, other h1 tags (or any other tag) will not be effected 
-->

<h1 style="color: blue; font-size: 40px">text</h1>
```

### Internal

Internal CSS is kept in the same file as your HTML

```html
<!--
Internal CSS is placed in the head of the document inside of the style tag
-->

<!DOCTYPE html>
<html>
  <head>
    <title>Title</title>
    <style>
      body {
        background-color: white;
        font-family: sans-serif;
      }
      h1 {
        color: green;
      }
    </style>
  </head>
  <body>
    <h1>text</h1>
  </body>
</html>
```

### External

External CSS is kept in a seperate file from your HTML

```css
/* styles.css */

body {
  background-color: white;
  font-family: sans-serif;
}

h1 {
  color: green;
}
```

```html
<!-- index.html -->

<!--
External CSS needs to be linked to the HTML. The link is placed in the head of the document inside of a link tag
-->

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Title</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>text</h1>
  </body>
</html>
```

## Selectors II

So far we have only seen how selectors can be attached to tags. Now we will see how to be more specific in applying CSS

### Universal Selector

Targets all page elements

```css
* {
  color: green;
}
```

### Class Selector

Targets elements using a specific class attribute

```html
<h1 class="primary">header</h1>
<p class="primary">text</p>
```

```css
.primary {
  color: green;
}
```

### ID Selector

Targets a unique element with a matching id attribute. Should be used like inline CSS (applied to only one specific element)

```html
<h1 id="main">text</h1>
```

```css
#main {
  color: green;
}
```

There are many more selectors and ways to use selectors, but this should be sufficient for now

## Properties

There are many CSS properties. It is helpful to be aware of what you are able to do with CSS so you can search for a property when you need it

List of all CSS properties:
https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties
