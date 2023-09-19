### **Paint Pixels on Click**

**Issue**: Pixels aren't adopting the selected colors when they're clicked.

**Goal**: Allow clicked pixel divs to take on the color of the last clicked color div.

**Confirming You Succeeded**: After choosing a palette color, click on a pixel. The pixel should display the selected color.

<details>
<summary>Hint 1</summary>

Think about how you'd keep track of a "currently selected color" and then apply it to another element.

</details>

<details>
<summary>Hint 2</summary>

The [MDN documentation on setting element styles](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/style) might be a helpful resource.

</details>

<details>
<summary>Hint 3</summary>

Here's a snippet to guide:

```javascript
let pickedColor;
pixelBox.style.bgColor = pickedColor;
```

Can you spot the error in the style property and think about where and how to update `pickedColor`?

</details>

<details>
<summary>Hint 4</summary>

Here's a more refined example:

```javascript
let currentColor;
artBox.style.bgColor = currentColor;
```

Ensure you adjust the style property to correctly set the background color and think about where and how to update `currentColor`.

</details>
