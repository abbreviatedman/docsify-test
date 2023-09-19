### **Creating a Color Div Inside the Loop**

**Issue**: We need divs to visually represent each color.

**Goal**: Inside the loop, spawn a `div` for each color.

**Confirming You Succeeded**: By logging the `colorDiv` inside the loop, you should observe new div elements in the console. Remember to clean up your `console.log` afterward.

<details>
<summary>Hint 1</summary>
For creating HTML elements dynamically using JavaScript, consider searching for "MDN creating an HTML element using JavaScript".
</details>

<details>
<summary>Hint 2</summary>
Consult the [MDN documentation on `createElement`](https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement) to understand how to produce an element programmatically.
</details>

<details>
<summary>Hint 3</summary>

Here's a snippet to guide you:

```javascript
const newElement = document.createAnElement();
```

There's a mistake in the method name. Can you spot it and rectify it? Additionally, ensure you save the newly created element in a variable.

</details>

<details>
<summary>Hint 4</summary>

Here's a more specific example:

```javascript
const colorDiv = document.createElement("span");
```

This snippet makes a `span` element. However, you need to generate a `div`. Modify the code accordingly.

</details>
