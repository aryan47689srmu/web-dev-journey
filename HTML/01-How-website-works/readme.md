# 🌐 How Frontend of a Website Works

Frontend is what happens inside your browser after a website is loaded. It is the part you **see and interact with**.

---

## 📦 1. Browser Receives Files

When you open a website, the browser downloads:

* **HTML** → Structure of the page
* **CSS** → Styling and design
* **JavaScript** → Interactivity and logic

---

## 🧱 2. HTML → DOM (Structure)

The browser converts HTML into a tree-like structure called the **DOM (Document Object Model)**.

### Example:

```html
<h1>Hello</h1>
```

Becomes:

```
Document
 └── h1 → "Hello"
```

👉 Think of this as the **skeleton** of the webpage.

---

## 🎨 3. CSS → CSSOM (Styling)

CSS is parsed into the **CSSOM (CSS Object Model)**.

It controls:

* Colors
* Fonts
* Spacing
* Layout

---

## 🔗 4. DOM + CSSOM → Render Tree

The browser combines both:

```
DOM + CSSOM = Render Tree
```

👉 This defines:

* What elements appear
* How they look

---

## 📐 5. Layout (Reflow)

The browser calculates:

* Element positions
* Width and height
* Spacing

👉 This step decides **where everything appears on screen**.

---

## 🖌️ 6. Painting

Now the browser draws everything:

* Text
* Images
* Colors

👉 Pixels are rendered on your screen.

---

## ⚡ 7. JavaScript (Interactivity)

JavaScript makes the page dynamic.

### Example:

```javascript
document.querySelector("h1").innerText = "Hi Aryan";
```

It can:

* Handle clicks
* Update content
* Call APIs
* Modify DOM

---

## 🔄 8. Re-rendering (Updates)

When something changes:

1. DOM updates
2. Layout recalculates
3. Page re-renders

👉 This happens instantly without refreshing the page.

---

## 🔁 Flow Summary

```
HTML → DOM
CSS → CSSOM
        ↓
   Render Tree
        ↓
     Layout
        ↓
     Paint
        ↓
  JavaScript Updates
```

---

## 🧠 Simple Analogy

Frontend is like building a house:

* HTML → Structure (bricks 🧱)
* CSS → Design (paint 🎨)
* JavaScript → Functionality (electricity ⚡)

---

## 🚀 Final Note

Frontend is all about:

* Displaying content
* Making it look good
* Making it interactive

Mastering these three (HTML, CSS, JS) is the foundation of web development.
