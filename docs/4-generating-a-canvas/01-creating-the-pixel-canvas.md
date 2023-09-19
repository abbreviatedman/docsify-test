### **Generate the Pixel Canvas**

**Issue**: A canvas to paint on is essential.

**Goal**: Use JavaScript to populate your canvas container with a grid of div elements.

**Confirming You Succeeded**: Your canvas should be populated with a grid of smaller divs.

<details>
<summary>Hint 1</summary>
Nested loops will help you construct a grid of divs.
</details>

<details>
<summary>Example Code</summary>

```javascript
let pixelContainer = document.querySelector(".pixel-canvas-container");
for (let row = 0; row < 10; row++) {
  // Assuming a 10x10 grid
  for (let col = 0; col < 10; col++) {
    let pixelDiv = document.createElement("div");
    pixelContainer.appendChild(pixelDiv);
  }
}
```

</details>
