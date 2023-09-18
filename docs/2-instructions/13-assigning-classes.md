### **Assign a Class to Each Palette Color Div**

**Issue**: Uniformity is vital for each color in your palette regarding appearance and behavior.

**Goal**: Within the loop where you're creating the color div, ensure each is equipped with our class name.

<details>
<summary>Hint 1</summary>
The `classList.add()` method is invaluable when wanting to add a class to an element.
</details>

<details>
<summary>Example Code</summary>

While inside the loop:

```javascript
for (let hue = 0; hue < randomColors.length; hue++) {
  let shadeDiv = document.createElement("div");
  containerDiv.appendChild(shadeDiv);
  shadeDiv.classList.add("palette-color");
}
```

</details>

**Confirming You Succeeded**: Due to the class applied, all colors in your palette should now share a consistent appearance and behavior. To confirm, open Chrome's Dev Tools and inspect the elements, ensuring each color div has the correct class.
