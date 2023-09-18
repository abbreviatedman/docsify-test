### **Pixel Art Maker: A Frontend Project**

**Introduction**:

Welcome to the Pixel Art Maker project! This hands-on activity is designed to give you practical experience with key web development concepts. By the end of this project, you'll have a functioning pixel art maker that you can use to create unique designs.

**Learning Objectives**:

- Get hands-on experience with DOM manipulation.
- Dive deep into the process of small app creation.
- Understand user stories and how they can be expressed in code.

---

### **Understanding the Pixel Art Maker App**

Before diving into code, let's visualize the end goal and understand the Pixel Art Maker's functionality.

**User Stories**:

1. **Palette Color Selection**:

   - **Story**: The user can click a palette color to update the current color square with that selected color.
   - **Before Screenshot**: ![Palette with various colors, cursor hovering over blue, current color square displays red.](https://dummy-url.com/palette_before.png)
   - **After Screenshot**: ![After clicking blue shade in the palette, current color square displays blue.](https://dummy-url.com/palette_after.png)

2. **Canvas Coloring**:
   - **Story**: The user can click any canvas square to fill it with the color from the current color square.
   - **Before Screenshot**: ![Canvas of blank squares, cursor hovering over a square, ready to color it green.](https://dummy-url.com/canvas_before.png)
   - **After Screenshot**: ![Canvas square filled with green after clicking.](https://dummy-url.com/canvas_after.png)

**Finished Project Preview**:
You can view the finished Pixel Art Maker project for reference. Remember, the real learning is in the building process!

[View the Completed Pixel Art Maker App](https://dummy-url.com/finished_project)

---

### **Prepare Your Environment**

**Issue**: To start, you need to ensure you're all set up to code along.

**Goal**: Fork and clone the provided repo, have it open in VS Code, and be running with the Live Server extension.

**Confirming You Succeeded**: Look at your browser; you should see a blank canvas awaiting your artistic touch.

---

### **Examine Existing HTML**

**Issue**: Before diving in, it's wise to understand the foundation.

**Goal**: Go through the provided HTML code. Familiarize yourself with the structure and think about what you might add or modify.

**Confirming You Succeeded**: Can you explain the existing code? Do you have an idea of where your pixels and color palettes will go?

---

### **Incorporate JavaScript**

**Issue**: Your page is static. Let's change that.

**Goal**: Add a `script` tag linked to a JavaScript file. Make sure to use the `defer` attribute.

Why might you want to use the `defer` attribute in your script tag?

<details>
<summary>Hint 1</summary>
Using `defer` ensures that the script is executed in order after the HTML is parsed.
</details>

<details>
<summary>Example Code</summary>

Remember to adjust placeholder names.

```html
<script src="scriptFile.js" defer></script>
```

</details>

**Confirming You Succeeded**: Check your page. If nothing is broken and your browser's developer console shows no errors, you're on track!

---

### **Create the Palette Container in HTML**

**Issue**: To display the color palette, you need a specific area on your webpage.

**Goal**: In your HTML file, insert a `div` container element dedicated to your color palette. Make sure to apply our provided class name to get the styling.

<details>
<summary>Hint 1</summary>
Make use of the `div` element and give it the class name `color-palette-container` to ensure it acquires the styling we've prepared.
</details>

<details>
<summary>Example Code</summary>

```html
<div class="color-palette-container"></div>
```

</details>

**Confirming You Succeeded**: Check your HTML. You should see the div container. Open Chrome's Dev Tools and inspect the element to ensure you've added the correct class.

---

### **Create the Canvas Container in HTML**

**Issue**: You're missing a canvas area for painting.

**Goal**: Add a `div` container element in your HTML that serves as the pixel canvas. Remember to use our designated class name for the correct styling.

<details>
<summary>Hint 1</summary>
Employ the `div` element and bestow it the class name `pixel-canvas-container` so it obtains the styling we've furnished.
</details>

<details>
<summary>Example Code</summary>

```html
<div class="pixel-canvas-container"></div>
```

</details>

**Confirming You Succeeded**: The div container should now be in your HTML. To verify, open Chrome's Dev Tools and inspect the element to make sure you've attached the right class.

---

### **Create the Pixel Canvas**

**Issue**: We need pixels to paint on!

**Goal**: In your JavaScript file, generate a grid of divs in your canvas container.

<details>
<summary>Hint 1</summary>
Nested loops will help you construct a grid of divs.
</details>

<details>
<summary>Example Code</summary>

```javascript
let pixelContainer = document.querySelector(".pixelCanvasContainer");
for (let row = 0; row < 10; row++) {
  // Assuming a 10x10 grid
  for (let col = 0; col < 10; col++) {
    let pixelDiv = document.createElement("div");
    pixelContainer.appendChild(pixelDiv);
  }
}
```

</details>

**Confirming You Succeeded**: Your canvas should be populated with a grid of smaller divs.

---

### **Create an Array for Your Palette Colors**

**Issue**: To efficiently generate the color palette programmatically, it's beneficial to have all our desired colors stored in one place.

**Goal**: In your JavaScript file, construct an array containing your list of colors. Each color should be represented as a string, using the standard CSS color names.

<details>
<summary>Hint 1</summary>
An array in JavaScript is defined using square brackets `[]`, and individual items within the array are separated by commas.
</details>

<details>
<summary>Example Code</summary>

```javascript
let colorArray = ["red", "green", "blue"];
```

Remember, the colors provided are just placeholders. Replace them with the colors of your choice.

</details>

**Confirming You Succeeded**: To ensure your array is structured correctly, try logging it to the console. The result should be an array of color strings. After checking, remove the `console.log` statement for cleanliness!

---

### **Initiate a Loop for Color Array**

**Issue**: To generate color divs, loop through a color array.

**Goal**: Craft a loop to iterate over your color array.

<details>
<summary>Hint 1</summary>
A `for` loop should work well here.
</details>

<details>
<summary>Example Code</summary>

Adjust the placeholder names.

```javascript
for (let counter = 0; counter < colorList.length; counter++) {
  // Your code here
}
```

</details>

**Confirming You Succeeded**: Inside the loop, console.log `counter`. If you see numbers from `0` to the array's length minus one, you're doing well! Remove the log.

---

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

---

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

---

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

---

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

---

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

---

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

---

### **Paint Pixels on Click**

**Issue**: Pixels remain unresponsive to color selection.

**Goal**: Allow pixels to adopt the color of the last clicked color div.

<details>
<summary>Hint 1</summary>
You'll need a variable to hold the currently selected color, and then use `addEventListener` for the pixel divs.
</details>

<details>
<summary>Example Code</summary>

```javascript
let currentColor = null; // This can be updated in your color div click handler
for (let count = 0; count < 100; count++) {
  // For a 10x10 grid
  let artPixel = document.createElement("div");
  pixelContainer.appendChild(artPixel);
  artPixel.addEventListener("click", function () {
    artPixel.style.backgroundColor = currentColor;
  });
}
```

</details>

**Confirming You Succeeded**: Select a color from the palette and then click on a pixel. The pixel should adopt the selected color.

---

### **Reflecting on the Pixel Art Maker Journey**

Congratulations on completing the Pixel Art Maker project! 🎉

Let's take a moment to reflect on what you've achieved and the objectives you've met:

1. **DOM Manipulation**: Throughout the project, you've dynamically altered the structure and content of your web page using JavaScript. This gave your app its dynamic and interactive elements, letting users truly engage with what you've created.
2. **Small App Creation**: Starting with just an idea, you've built a functioning app piece by piece. This experience is invaluable. Overcoming each challenge and problem-solving each feature provides a foundation upon which you can build more complex projects in the future.
3. **User Stories to Code**: With each feature you've added to your Pixel Art Maker, you've brought a user story to life. This approach ensures the apps you build in the future will be user-focused, fulfilling the needs and desires of those who interact with your creations.

Take pride in what you've accomplished. This project serves not only as a testament to your coding capabilities but also as a stepping stone to even greater things in your coding journey. Onward and upward! 🚀
