### **Add Click Event to Each Color Div**

**Issue**: Your color divs currently don't interact with user clicks.

**Goal**: Within your loop, attach a click event listener to every color div.

**Confirming You Succeeded**: Test by clicking on a color div. You should observe some form of reaction, even if it's just a console message.

<details>
<summary>Hint 1</summary>

If you're unsure how to add event listeners in JavaScript, try searching for "JavaScript event listeners".

</details>

<details>
<summary>Hint 2</summary>

Review the [MDN documentation on `addEventListener`](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener).

</details>

<details>
<summary>Hint 3</summary>

A guiding snippet:

```javascript
element.on("click", function() {
  // Handle the click
});
```

Spot the error in how the event is added. Can you fix it?

</details>

<details>
<summary>Hint 4</summary>

Here's a closer example:

```javascript
shadeBox.onEvent("click", function() {
  // Your click handling logic here
});
```

Update the method to the correct one to add an event listener.

</details>
