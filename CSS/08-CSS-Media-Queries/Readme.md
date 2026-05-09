# CSS Media Queries

## Introduction

CSS Media Queries are used to apply different styles to a webpage based on the device characteristics such as screen size, width, height, orientation, and resolution.

They are an essential part of Responsive Web Design (RWD), helping websites look good on desktops, tablets, and mobile devices.

---

# Why Use Media Queries?

Media Queries help to:

- Create responsive websites
- Improve user experience on different devices
- Adjust layouts for mobile screens
- Change font sizes and spacing
- Hide or show elements based on screen size

---

# Basic Syntax

```css
@media media-type and (condition) {
    /* CSS Rules */
}
````

---

# Example

```css
@media screen and (max-width: 768px) {
    body {
        background-color: lightblue;
    }
}
```

### Explanation

* `screen` → applies styles for screens
* `max-width: 768px` → styles apply when screen width is 768px or smaller

---

# Types of Media Queries

## 1. max-width

Applies styles when the screen width is less than or equal to a specific size.

```css
@media (max-width: 600px) {
    body {
        font-size: 14px;
    }
}
```

---

## 2. min-width

Applies styles when the screen width is greater than or equal to a specific size.

```css
@media (min-width: 600px) {
    body {
        font-size: 18px;
    }
}
```

---

## 3. Orientation

Checks whether the device is in portrait or landscape mode.

```css
@media (orientation: landscape) {
    body {
        background-color: lightgray;
    }
}
```

---

# Common Breakpoints

| Device Type | Screen Width     |
| ----------- | ---------------- |
| Mobile      | up to 600px      |
| Tablet      | 601px to 768px   |
| Laptop      | 769px to 1024px  |
| Desktop     | 1025px and above |

---

# Responsive Navigation Example

```css
.navbar {
    display: flex;
    justify-content: space-between;
}

/* Mobile View */
@media (max-width: 600px) {
    .navbar {
        flex-direction: column;
    }
}
```

### Result

* Desktop → navbar items appear in a row
* Mobile → navbar items appear in a column

---

# Multiple Conditions

You can combine conditions using `and`.

```css
@media screen and (min-width: 600px) and (max-width: 900px) {
    body {
        background-color: lightgreen;
    }
}
```

---

# Using Media Queries for Dark Mode

```css
@media (prefers-color-scheme: dark) {
    body {
        background-color: black;
        color: white;
    }
}
```

---

# Responsive Image Example

```css
img {
    width: 100%;
    height: auto;
}
```

This makes images responsive and prevents overflow on smaller screens.

---

# Advantages of Media Queries

* Improves responsiveness
* Better user experience
* Supports multiple devices
* Makes layouts flexible
* Essential for modern web design

---

# Disadvantages of Media Queries

* Can increase CSS complexity
* Requires testing on multiple devices
* Too many breakpoints can make code harder to manage

---

# Best Practices

* Use mobile-first design
* Keep breakpoints simple
* Avoid excessive media queries
* Use relative units like `%`, `em`, `rem`
* Test on different screen sizes

---

# Mobile-First Approach

In mobile-first design:

1. Write CSS for mobile devices first
2. Use `min-width` media queries for larger screens

Example:

```css
body {
    font-size: 14px;
}

/* Larger screens */
@media (min-width: 768px) {
    body {
        font-size: 18px;
    }
}
```

---

# Conclusion

CSS Media Queries are a powerful feature used to create responsive and adaptive web designs. They allow developers to apply different styles depending on device size and characteristics, ensuring websites work properly across mobiles, tablets, laptops, and desktops.

Responsive design using media queries is a fundamental skill in modern frontend development.

```
```
