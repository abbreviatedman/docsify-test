### **Assign a Class to Each Palette Color Div**

**Issue**: Uniform styling and behavior is needed for your palette colors.

**Goal**: While creating each color div in the loop, append a class for uniformity.

**Confirming You Succeeded**: Check out the rendered app in your browser. Ensure all divs share the same appearance, reflecting the applied class.

<details>
<summary>Hint 1</summary>

Not sure how to add classes in JavaScript? Look up "Adding classes to elements in JavaScript".

</details>

<details>
<summary>Hint 2</summary>

The [MDN documentation on `classList.add()`](https://developer.mozilla.org/en-US/docs/Web/API/Element/classList) can be your guide.

</details>

<details>
<summary>Hint 3</summary>

Here's a guiding snippet:

```javascript
someElement.classes.add("sample-class");
```

There's an error in accessing the class list. Can you identify and fix it?

</details>

<details>
<summary>Hint 4</summary>

Here's a refined example:

```javascript
shadeDiv.classList.add("sample-class");
```

Ensure you replace "sample-class" with your intended class name.

</details>
