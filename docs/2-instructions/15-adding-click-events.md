### **Add Click Event to Each Color Div**

**Issue**: Your color divs don't respond to user interaction.

**Goal**: Incorporate a click event listener for each color div within the loop.

<details>
<summary>Hint 1</summary>
Consider the `addEventListener` method.
</details>

<details>
<summary>Example Code</summary>

Always keep your code within the loop context.

```javascript
for (let index = 0; index < colorList.length; index++) {
  let shadeDiv = document.createElement("div");
  shadeDiv.style.backgroundColor = colorList[index];
  chosenContainer.appendChild(shadeDiv);
  shadeDiv.addEventListener("click", function () {
    // Your logic for handling the click event
  });
}
```

</details>

**Confirming You Succeeded**: Click on a color div. You should see an effect, even if it's a console message for now.
