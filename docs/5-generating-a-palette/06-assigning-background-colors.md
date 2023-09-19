### **Assign Background Colors to the Color Divs**

**Issue**: Your color divs are currently colorless.

**Goal**: Within the loop, assign background colors to each of the color divs.

**Confirming You Succeeded**: Your browser should display each div in the palette with its distinct color.

<details>
<summary>Hint 1</summary>

If you're unsure how to set styles in JavaScript, consider searching for "Setting CSS styles using JavaScript".

</details>

<details>
<summary>Hint 2</summary>

The [MDN documentation on styling](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/style) can provide insights.

</details>

<details>
<summary>Hint 3</summary>

A snippet

 to guide:

```javascript
someElement.styling.backgroundColor = "blue";
```

There's a mistake in the property accessing style. Can you identify and fix it?

</details>

<details>
<summary>Hint 4</summary>

Here's a refined example:

```javascript
shadeDiv.style.backgroundColor = "cyan";
```

Replace "cyan" with the appropriate color from your array.

</details>
