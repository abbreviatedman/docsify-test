### **Appending Each Color Div**

**Issue**: Generated divs are in limbo, only present in JavaScript memory.

**Goal**: After forging each color div, affix it to the palette container.

**Confirming You Succeeded**: View your webpage. Spot the color divs in the palette container? Perfect!

<details>
<summary>Hint 1</summary>
The method `appendChild()` on the palette container will be handy.
</details>

<details>
<summary>Example Code</summary>

Make sure you're still within your loop.

```javascript
for (let counter = 0; counter < colorList.length; counter++) {
  let newDiv = document.createElement("div");
  chosenContainer.appendChild(newDiv);
}
```

</details>
