# Flexbox Guide

## Introduction
Flexbox (Flexible Box Layout) is a CSS layout module that allows you to design complex layouts with ease. It enables efficient alignment, distribution, and responsiveness of elements within a container.

## Getting Started
To use Flexbox, define a flex container using `display: flex;`. This enables Flexbox properties on its child elements.

```css
.container {
  display: flex;
}
```

## Key Concepts

### Flex Container Properties
The parent element (container) can have the following properties:

- **`display: flex;`** – Enables Flexbox on the container.
- **`flex-direction`** – Defines the direction of flex items.
  - `row` (default) – Items are placed left to right.
  - `column` – Items are placed top to bottom.
  - `row-reverse` – Items are placed right to left.
  - `column-reverse` – Items are placed bottom to top.
- **`justify-content`** – Aligns items along the main axis.
  - `flex-start` (default) – Items start from the beginning.
  - `flex-end` – Items align at the end.
  - `center` – Items are centered.
  - `space-between` – Items are spaced evenly with no gaps at edges.
  - `space-around` – Items have equal spacing around them.
  - `space-evenly` – Items have equal space between them.
- **`align-items`** – Aligns items along the cross axis.
  - `stretch` (default) – Items stretch to fill container.
  - `flex-start` – Items align at the start of the cross axis.
  - `flex-end` – Items align at the end of the cross axis.
  - `center` – Items are centered.
  - `baseline` – Items align based on their text baseline.
- **`align-content`** – Aligns rows within a container when wrapped.

### Flex Item Properties
The child elements (items) can have the following properties:

- **`order`** – Specifies the order of items (default is 0).
- **`flex-grow`** – Defines how much a flex item grows relative to others.
- **`flex-shrink`** – Defines how much a flex item shrinks relative to others.
- **`flex-basis`** – Specifies the initial size before applying flex-grow/shrink.
- **`align-self`** – Overrides `align-items` for an individual item.

## Example Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Example</title>
    <style>
        .container {
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: center;
            height: 100vh;
            border: 2px solid #333;
        }
        .item {
            background-color: lightblue;
            padding: 20px;
            margin: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
    </div>
</body>
</html>
```

## Resources
For a more detailed guide, visit the [Flexbox tutorial](https://internetingishard.netlify.app/html-and-css/flexbox/index.html).

## Conclusion
Flexbox simplifies layout design, making it easier to create responsive and flexible web pages. Mastering Flexbox is essential for modern web development!

