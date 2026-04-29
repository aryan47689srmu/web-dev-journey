# CSS Selectors Masterclass

## Introduction

CSS selectors are used to target HTML elements so you can apply styles to them. Understanding selectors is essential for writing clean, efficient, and maintainable CSS.

---

## 1. Basic Selectors

### 1.1 Universal Selector

Selects all elements.

```css
* {
  margin: 0;
  padding: 0;
}
```

---

### 1.2 Element Selector

Selects elements by tag name.

```css
p {
  color: blue;
}
```

---

### 1.3 Class Selector

Selects elements with a specific class.

```css
.note {
  color: green;
}
```

---

### 1.4 ID Selector

Selects an element with a specific ID.

```css
#header {
  background-color: black;
}
```

---

## 2. Grouping Selector

Apply the same style to multiple elements.

```css
h1, h2, p {
  color: red;
}
```

---

## 3. Combinator Selectors

### 3.1 Descendant Selector

Selects elements inside another element.

```css
div p {
  color: blue;
}
```

---

### 3.2 Child Selector

Selects direct children.

```css
div > p {
  color: green;
}
```

---

### 3.3 Adjacent Sibling Selector

Selects the immediate next sibling.

```css
h1 + p {
  color: orange;
}
```

---

### 3.4 General Sibling Selector

Selects all siblings after an element.

```css
h1 ~ p {
  color: purple;
}
```

---

## 4. Attribute Selectors

### 4.1 Select by Attribute

```css
input[type] {
  border: 1px solid black;
}
```

---

### 4.2 Select by Attribute Value

```css
input[type="text"] {
  color: blue;
}
```

---

### 4.3 Starts With

```css
a[href^="https"] {
  color: green;
}
```

---

### 4.4 Ends With

```css
a[href$=".pdf"] {
  color: red;
}
```

---

### 4.5 Contains

```css
a[href*="google"] {
  color: purple;
}
```

---

## 5. Pseudo-Classes

Used to define a special state of an element.

```css
a:hover {
  color: red;
}
```

### Common Pseudo-Classes

```css
li:first-child { }
li:last-child { }
li:nth-child(2) { }
input:focus { }
```

---

## 6. Pseudo-Elements

Used to style specific parts of elements.

```css
p::first-letter {
  font-size: 30px;
}
```

### Common Pseudo-Elements

```css
p::first-line { }
::before { }
::after { }
```

---

## 7. Specificity

Defines which selector has priority.

| Selector Type | Priority |
| ------------- | -------- |
| Inline        | Highest  |
| ID            | High     |
| Class         | Medium   |
| Element       | Low      |

Example:

```css
#id { color: red; }
.class { color: blue; }
p { color: green; }
```

---

## 8. Best Practices

* Use classes instead of IDs for styling
* Avoid overly complex selectors
* Keep specificity low
* Write reusable CSS
* Use meaningful class names

---

## Conclusion

CSS selectors are the backbone of styling web pages. Mastering them allows you to write efficient and scalable CSS, making your projects more professional and maintainable.
