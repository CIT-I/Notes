# CSS

## Selectors III

With the `div` HTML tag, we will start to nest tags. Nesting HTML elements introduces new ways to utilize selectors.

### Child Combinator

The child combinator (`>`) is placed between two CSS selectors. It matches only those elements matched by the second selector that are the direct children of elements matched by the first.

```css

```

### Descendant Combinator

The descendant combinator — typically represented by a single space ("` `") character — combines two selectors such that elements matched by the second selector are selected if they have an ancestor element matching the first selector.

```css

```

## Properties

### Margin & Padding

<img height="360" alt="CSS box model" src="https://github.com/user-attachments/assets/534a0a4a-4162-41f3-be91-73bc5aeb86ff" />

Margins create extra space around an element. Padding creates extra space within an element

The distinction is illustrated in the following example:

```html
<body>
  <p>text</p>
</body>
```

```css
p {
  margin: 12px;
  padding: 8px;
}
```
Here there is a 12px spacing (margin) between the body tag and the paragraph tag, and a 8px spacing (padding) between the content of the paragraph tag and the area the paragraph tag occupies. To more clearly visualize this difference, you can add a background color to these elements.

### Flexbox

Flexbox is a layout model for arranging items horizontally or vertically within a container, in a responsive way.

When applying Flex properties, we typically want to establish the:

- Layout: how an elements children are displayed

```css
display: flex;
```

- Direction: how flex items are placed in the flex container defining the main axis and the direction

```css
/* items ordered left to right */
flex-direction: row;
/* items ordered top to bottom */
flex-direction: column;
/* items ordered right to left */
flex-direction: row-reverse;
/* items ordered bottom to top */
flex-direction: column-reverse;
```

- Distribution

`justify-content`: defines how space is distributed between and around content items along the main axis (flex-direction)

`align-items`: controls the alignment of items on the cross axis (opposite of flex-direction)

```css
justify-content: center;
align-items: center;
```
