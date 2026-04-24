# ID and Classes in HTML

## Introduction

In HTML, `id` and `class` are attributes used to identify and style elements. They are widely used in CSS and JavaScript.

---

## ID in HTML

### Definition

The `id` attribute uniquely identifies an HTML element.

### Rules

* Must be unique within the page
* Used for a single element only

### Example

```html
<h1 id="title">Hello World</h1>
```

### CSS Usage

```css
#title {
  color: red;
}
```

---

## Class in HTML

### Definition

The `class` attribute is used to group multiple elements.

### Rules

* Can be used multiple times
* One element can have multiple classes

### Example

```html
<p class="text">Paragraph 1</p>
<p class="text">Paragraph 2</p>
```

### CSS Usage

```css
.text {
  color: blue;
}
```

---

## Difference Between ID and Class

| Feature    | ID             | Class             |
| ---------- | -------------- | ----------------- |
| Uniqueness | Unique         | Multiple use      |
| CSS Symbol | #              | .                 |
| Usage      | Single element | Multiple elements |
| Priority   | High           | Low               |

---

## Conclusion

* Use `id` for unique elements.
* Use `class` for reusable styles.
* Both are essential for styling and scripting in web development.
