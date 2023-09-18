### **Creating a Color Div Inside the Loop**

**Issue**: To represent each color, you need a div.

**Goal**: Inside the loop, spawn a `div` for each color.

<details>
<summary>Hint 1</summary>
Use `document.createElement()`.
</details>

<details>
<summary>Example Code</summary>

Ensure your code is within the loop context.

```javascript
for (let counter = 0; counter < colorList.length; counter++) {
  let newDiv = document.createElement("div");
  // Your following code
}
```

</details>

**Confirming You Succeeded**: Console.log `newDiv` inside the loop. You should witness newly crafted div elements in the console. Remove the log.
