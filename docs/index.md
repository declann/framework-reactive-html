---
title: issue description
toc: false
---

<style>
  #wrapper {
    background: lightgreen;
  }

  #placeholder {
    background: green;
    color: white;
  }
</style>

<div id="wrapper">

## a header in a wrapper

a palceholder in a wrapper:

```js
const placeholder = html`<div id="placeholder"></div>`
display(placeholder)
display("width generator on wrapper element:")
display(content_width)
```

**If I edit anything inside the wrapper div, the reactive width is set to 0**

</div>

```js
placeholder; // force order dependency
document.getElementById('placeholder').textContent = "hello";
```

```js
const content_width = Generators.width(document.getElementById("wrapper"));
```