# html

### elements

```html
<div> <!-- opening tag -->
    i am some text
</div> <!-- closing tag -->

<img /> <!-- img is a self-closing element -->

<a href="https://google.com">google</a>
```

**some useful elements:**

- `<div>`: empty box with no default style
- `<img>`: image (it needs a "src" attribute)
- `<a>`: link (needs an "href" attribute)
- `<input>`: attributes: "type", "value"
- `<textarea>`: big text input box
- `<button>`: clickable!
- `<select>`: select from a list of options

**other common elements**
- `<header>`
- `<footer>`
- `<section>`
- `<main>`
- `<p>`: paragraph (has some default margin)

### attributes

**allow you to modify HTML elements. In React, these are called "props"**

Attributes are added to the opening tag, before the `>` character. Multiple attributes can be added with spaces between

```html
<!-- apply a class -->
<div class="my-class"></div>

<!-- apply "inline" styles -->
<div style="height:40px"></div>

<!-- listen for a click -->
<button onclick="runFunction()" onhover=""></button>
```
