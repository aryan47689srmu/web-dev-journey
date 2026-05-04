# CSS Specificity and Cascade

## Introduction

CSS (Cascading Style Sheets) determines how HTML elements are styled. When multiple CSS rules apply to the same element, the browser decides which rule to apply based on **specificity** and the **cascade**.

Understanding these concepts is essential for writing predictable and maintainable CSS.

---

## What is CSS Cascade?

The **cascade** is the process used by browsers to resolve conflicts when multiple CSS rules target the same element.

### Cascade Priority Order

The browser applies styles in the following order:

1. Inline styles (highest priority)
2. Internal and external stylesheets
3. Browser default styles (lowest priority)

If multiple rules have the same origin and importance, then **specificity** is used.

---

## What is CSS Specificity?

**Specificity** is a ranking system that determines which CSS rule is applied when multiple rules target the same element.

Each selector is assigned a weight based on its type.

---

## Specificity Hierarchy

| Selector Type        | Example            | Specificity Value |
|---------------------|------------------|------------------|
| Inline styles       | style=""          | 1000             |
| ID selector         | #id              | 100              |
| Class selector      | .class           | 10               |
| Attribute selector  | [type="text"]    | 10               |
| Pseudo-class        | :hover           | 10               |
| Element selector    | p, div           | 1                |
| Pseudo-element      | ::before         | 1                |

---

## Example of Specificity

```css
p {
  color: blue;
}

.text {
  color: green;
}

#heading {
  color: red;
}
