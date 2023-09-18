### **Appending Each Color Div**

**Issue**: Divs currently reside only in JavaScript memory.

**Goal**: After forging each color div, affix it to the palette container.

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

**Confirming You Succeeded**: Peek at your browser. Witness the color divs inside the palette container? Great!
