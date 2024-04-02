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

<div id="placeholder"></div>

(the 'hello' text is added by JS @ bottom of page)

If I edit anything inside the wrapper div, the hot reload replaces the top element, removing the hello text

</div>

```js echo
document.getElementById('placeholder').textContent = "hello";
```

(real usecase is to maintain the state of a dynamic vega visual)