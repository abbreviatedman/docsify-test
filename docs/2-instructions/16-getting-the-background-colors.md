### **Extract Background Color from Clicked Color Div**

**Issue**: When a color is selected, you need its color value.

**Goal**: Inside your click event handler, obtain the background color of the clicked div.

<details>
<summary>Hint 1</summary>
Research `window.getComputedStyle()`.
</details>

<details>
<summary>Example Code</summary>

Here's how you'd get it within your loop and click event:

```javascript
for (let step = 0; step < colorList.length; step++) {
  let tintDiv = document.createElement("div");
  tintDiv.style.backgroundColor = colorList[step];
  chosenContainer.appendChild(tintDiv);
  tintDiv.addEventListener("click", function () {
    let selectedStyle = window.getComputedStyle(tintDiv);
    let chosenColor = selectedStyle.backgroundColor;
    // Use the chosenColor in your logic
  });
}
```

</details>

**Confirming You Succeeded**: Inside the click handler, log the `chosenColor`. When you click on a color div, its RGB value should display in the console. Don't forget to remove the log afterward.
