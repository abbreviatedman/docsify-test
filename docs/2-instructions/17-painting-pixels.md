### **Paint Pixels on Click**

**Issue**: Pixels remain unresponsive to color selection.

**Goal**: Allow pixels to adopt the color of the last clicked color div.

<details>
<summary>Hint 1</summary>
You'll need a variable to hold the currently selected color, and then use `addEventListener` for the pixel divs.
</details>

<details>
<summary>Example Code</summary>

```javascript
let currentColor = null; // This can be updated in your color div click handler
for (let count = 0; count < 100; count++) {
  // For a 10x10 grid
  let artPixel = document.createElement("div");
  pixelContainer.appendChild(artPixel);
  artPixel.addEventListener("click", function () {
    artPixel.style.backgroundColor = currentColor;
  });
}
```

</details>

**Confirming You Succeeded**: Select a color from the palette and then click on a pixel. The pixel should adopt the selected color.
