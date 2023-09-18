### **Assign Background Colors to the Color Divs**

**Issue**: Your color divs don't show their colors yet.

**Goal**: Within the loop, assign background colors to each of the color divs.

<details>
<summary>Hint 1</summary>
You can utilize the `style.backgroundColor` property on the div element.
</details>

<details>
<summary>Example Code</summary>

Ensure you're working within the loop context.

```javascript
for (let cycle = 0; cycle < colorList.length; cycle++) {
  let hueDiv = document.createElement("div");
  chosenContainer.appendChild(hueDiv);
  hueDiv.classList.add("palette-color");
  hueDiv.style.backgroundColor = colorList[cycle];
}
```

</details>

**Confirming You Succeeded**: Observe your palette in the browser. Each div should now display a distinct color.
