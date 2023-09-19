### **Extract Background Color from Clicked Color Div**

**Issue**: You need to obtain the color value of a selected color.

**Goal**: Inside your click event handler, obtain the background color of the clicked div.

**Confirming You Succeeded**: After clicking a color div, the retrieved color value is visible in the console. Ensure you remove the log after confirming.

<details>
<summary>Hint 1</summary>

Consider searching for "JavaScript get computed style" to understand how to retrieve CSS values.

</details>

<details>
<summary>Hint 2</summary>

Look into the [MDN documentation for `window.getComputedStyle()`](https://developer.mozilla.org/en-US/docs/Web/API/Window/getComputedStyle).

</details>

<details>
<summary>Hint 3</summary>

Here's a template to guide:

```javascript
let colorValue = window.getStyle(element).backgroundColor;
```

There are errors in the method name and how it's used. Can you identify and correct them?

</details>

<details>
<summary>Hint 4</summary>

Here's a refined example:

```javascript
let selectedColor = window.getComputedStyle(shadeBox).colorValue;
```

Ensure you adapt the property you're trying to fetch (from colorValue).

</details>
