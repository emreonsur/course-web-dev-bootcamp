# The Developer Bootcamp on Udemy

## Course Notes

**Course link:** https://www.udemy.com/course/the-web-developer-bootcamp/

## Section 3: HTML: The Essentials

### `<p>` Element

### `<h1>`–`<h6>`: The HTML Section Heading elements

6 levels of the `h` element:

1. `<h1>`
2. `<h2>`
3. `<h3>`
4. `<h4>`
5. `<h5>`
6. `<h6>`

### Comments in HTML

```html
<!--This is a comment-->
```

### HTML Skeleton/Boilerplate

Standard HTML skeleton:

```html
<!DOCTYPE html>
<html>
    <head>
        <title>My Web Page</title>
    </head>
    <body>
        <!--Here is content-->
    </body>
</html
```

### Lists

#### Unordered Lists

```html
<ul>
  <li>Milk</li>
  <li>Eggs</li>
  <li>Bread</li>
  <li>Hummus</li>
</ul>
```

#### Ordered Lists

```html
<ol>
  <li>Go straight</li>
  <li>Turn left</li>
  <li>Take the second right</li>
  <li>Enter the red building</li>
</ol>
```

#### Nested Lists

### Hyperlinks / [`<a>: The Anchor Element`](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/a)

#### Anatomy of a Link

```html
<p>
  This is a link to
  <a href="https://developer.mozilla.org/en-US/">MDN Web Docs</a>.
</p>
```

#### `title` Attribute

> Supporting information can be added to links

```html
<a href="https://www.mozilla.org/en-US/" title="Mozilla's Official Website">
  The Mozilla Homepage</a
>
```

### Images / [`<img>`: The Image Embed element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/img)

```html
<img
  src="pictures/test.jpg"
  alt='The word "Text" (red T, green e, black s and t)'
  width="200"
/>
```

## Section 4: HTML: Next Steps & Semantics

### Block and Inline Elements - Divs and Spans

#### `div` Element

```html
<div>
  <p>This is a paragraph</p>
  <p>This is another paragraph</p>
  <p>
    This is also another paragraph, but all of these are contained in one
    div
  </p>
</div>
```

#### `span` Element

```html
<p>
  This is a paragraph and <span>this</span> and <span>this</span> are two
  spans.
</p>
```

### Assortment Elements

#### `hr` Elements

```html
<h1>A title</h1>

<hr>

<p>A paragraph</p>
```

#### `br` Element

```html
<p>
  A line <br />
  Another line
</p>
```

#### `sup` and `sub` Element

```html
a<sup>2</sup>
```

### HTML Entities

<a href="[HTML Standard](https://html.spec.whatwg.org/multipage/named-characters.html)">Named Character References</a>

### Semantic Elements

- `<main>`
- `<nav`
- `<section>`
- `<article>`
- `<aside>`
- `<header>`
- `<foot>`
- `<time>`
- `<figure>`
- `<figcaption>`
- `<abbr>`
- `data`

### Emmet

[Emmet — the essential toolkit for web-developers](https://emmet.io/)

## Section 5: HTML:  Forms & Tables

### Tables

- `<table>`
- `<tr>`
- `<td>`
- `<th>`
- `<thead>`
- `<tfoot>`
- `<tbody>`
- `colspan` and `rowspan` attributes

#### Demo

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Heaviest Birds Table</title>
  </head>

  <body>
    <h1>Tables Demo</h1>

    <h2>Heaviest Birds</h2>
    <table>
      <thead>
        <tr>
          <th>Animal</th>
          <th>Average Mass [kg (lb)]</th>
          <th>Maximum Mass [kg (lb)]</th>
          <th>Flighted</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Ostrich</td>
          <td>104 (230)</td>
          <td>156.8 (346)</td>
          <td>No</td>
        </tr>
        <tr>
          <td>Somali Ostrich</td>
          <td>90 (200)</td>
          <td>130 (287)</td>
          <td>No</td>
        </tr>
        <tr>
          <td>Wild Turkey</td>
          <td>13.5 (29.8)</td>
          <td>39 (86)</td>
          <td>Yes</td>
        </tr>
      </tbody>
    </table>

    <h2>Colspan and Rowspan Demo</h2>
    <table>
      <thead>
        <tr>
          <th rowspan="2">Animal</th>
          <th colspan="2">Average Mass</th>
          <th rowspan="2">Flighted</th>
        </tr>
        <tr>
          <th>kg</th>
          <th>lb</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Ostrich</td>
          <td>104</td>
          <td>230</td>
          <td>No</td>
        </tr>
        <tr>
          <td>Somali Ostrich</td>
          <td>90</td>
          <td>200</td>
          <td>No</td>
        </tr>
        <tr>
          <td>Wild Turkey</td>
          <td>13.5</td>
          <td>29.8</td>
          <td>Yes</td>
        </tr>
      </tbody>
    </table>
  </body>
</html>
```

### Forms

- The `<form>` container element
  - `<input>` element
    - `type` Attribute / Input Types
      - text
      - password
      - color
      - number
      - checkbox
      - radio
      - range
      - url
  - `<label>` Element
  - `<select>` Element
    - `<option>`
  - `placeholder` Attribute
  - `<button>` Element
    - `type` Attribute
  - `<textarea>` Element

#### Validations

We can talk about two different approaches to validation:

- **Client-side validation**
- **Server-side validation**

##### HTML Form Validations

- `required`
- `minlength`
- `maxlength`

## Section 6: CSS: The Very Basics

CSS is a language describing how documents are presented visually.

### CSS Rule Syntax

```
selector {
	property: value;
}
```

> A CSS rule makes all `<h1>` elements purple

```css
h1 {
	color: purple;
}
```

### Including Styles

#### Inline Styles

```html
<h1 style="color: wheat; background-color: brown">CSS Lab</h1>
<button style="border-style: dashed">Button</button>
```

#### `<style` Element

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Lab</title>  

    <style>
      h1 {
        color: green
      }
    </style>
  </head>
  <body>
    <h1>First h1</h1>
    <h1>Second h1</h1>
    <h1>Third h1</h1>
  </body>
</html>
```

#### External Stylesheet — Best Practice

> styles.css file contains CSS rules.

```css
h1 {
  color: red;
}
```

This file needs to be linked to the HTML document in which we want to use the styles. We can do this with the `<link>` element.

> styles.css is now linked to index.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Lab</title>
    <link rel="stylesheet" href="style.css">
    </style>
  </head>
  <body>
    <h1>First h1</h1>
    <h1>Second h1</h1>
    <h1>Third h1</h1>
  </body>
</html>
```

## deneme



## Section 7

## Section 8

## Section 9

## Section 10

## Section 11

## Section 12

## Section 13