# HTML

## Syntax

```html
<p>rendered text</p>
```

- `<p>` is a opening tag. It consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets.
- `</p>` is a closing tag, indicated by the forward slash
- `rendered text` is the content of the element
- `<p>rendered text</p>` all of these parts together make up an element

> [!NOTE]
> Most html elements are structured in this way, but not all are. Some elements do not have any content, for example the image tag:
> ```html
> <img src="" alt="" />
> ```

## Attributes

In the image tag example there is `src=""` and `alt=""`, these are attributes.

Attributes contain extra information about the element that isn't part of its content.

`src` specifies the URL or relative path (if an asset is in your local project) \
`alt` provides a text description for people who cannot see it

## Boilerplate

When you create a .html file, these elements must be added to maximize compatibility

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```
- `<!DOCTYPE>` tells the browser the version of HTML you’re using
- `<html>` represents the root (top-level element) of an HTML document. All other elements must be descendants of this element.
- `<head>`: contains metadata about the document like title, scripts, and style sheets
- `<body>`: contains the content of your website
Many programs have shortcuts to automatically add the boilerplate

## Tags I

A tag is used for creating an element which will render a certain format

### Headings

There are six heading elements: h1, h2, h3, h4, h5, and h6. Each element represents a different level of content in the document; h1 represents the main heading, h2 represents subheadings, h3 represents sub-subheadings, etc.

```html
<h1>heading one</h1>
<h2>heading two</h2>
<h3>heading three</h3>
<h4>heading four</h4>
<h5>heading five</h5>
<h6>heading six</h6>
```

### Paragraph

Paragraphs can be any structural grouping of related content, such as images or form fields

```html
<p>paragraph</p>
```

### Lists

There are ordered `ol` lists, for lists in which the order of the items does matter and unordered lists `ul`, for lists of items for which the order of the items doesn't matter

The items of the list are wrapped in a list item `li` tag

```html
<ol>
  <li>first</li>
  <li>second</li>
  <li>third</li>
</ol>

<ul>
  <li>item</li>
  <li>item</li>
  <li>item</li>
</ul>
```

the lists render as follows:

<ol>
  <li>first</li>
  <li>second</li>
  <li>third</li>
</ol>

<ul>
  <li>item</li>
  <li>item</li>
  <li>item</li>
</ul>
