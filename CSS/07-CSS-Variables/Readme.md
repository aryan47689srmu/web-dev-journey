# CSS Variables

CSS Variables, also known as **Custom Properties**, allow developers to store reusable values in CSS. These values can be used throughout the stylesheet, making code cleaner, easier to maintain, and more flexible.

CSS variables are especially useful for managing colors, fonts, spacing, themes, and repeated values.

---

# Syntax of CSS Variables

CSS variables are defined using `--` followed by the variable name.

```css
:root {
    --main-color: blue;
}
```

To use the variable, the `var()` function is used.

```css
h1 {
    color: var(--main-color);
}
```

---

# Why Use CSS Variables?

## 1. Reusability

You can define a value once and use it multiple times.

```css
:root {
    --primary-color: #3498db;
}

button {
    background-color: var(--primary-color);
}

h1 {
    color: var(--primary-color);
}
```

---

## 2. Easy Maintenance

If you want to change a repeated value, you only need to update the variable once.

```css
:root {
    --font-size: 18px;
}
```

Changing `18px` to another value automatically updates all places using that variable.

---

## 3. Better Readability

Variables make CSS easier to understand.

```css
:root {
    --danger-color: red;
}
```

This is more meaningful than repeatedly writing `red` everywhere.

---

# Global Variables Using `:root`

The `:root` selector is commonly used to define global variables.

```css
:root {
    --main-bg: lightgray;
    --text-color: black;
}
```

These variables can be accessed anywhere in the stylesheet.

```css
body {
    background-color: var(--main-bg);
    color: var(--text-color);
}
```

---

# Local Variables

Variables can also be defined inside specific selectors.

```css
.card {
    --card-color: white;
    background-color: var(--card-color);
}
```

This variable only works inside `.card`.

---

# Using Fallback Values

A fallback value is used if the variable is not defined.

```css
p {
    color: var(--para-color, black);
}
```

If `--para-color` does not exist, the text color becomes black.

---

# Changing Variables with Media Queries

CSS variables can be changed for different screen sizes.

```css
:root {
    --font-size: 16px;
}

body {
    font-size: var(--font-size);
}

@media (max-width: 600px) {
    :root {
        --font-size: 14px;
    }
}
```

This helps create responsive designs.

---

# Dark Mode Example

CSS variables are commonly used for dark mode themes.

```css
:root {
    --bg-color: white;
    --text-color: black;
}

.dark-mode {
    --bg-color: black;
    --text-color: white;
}

body {
    background-color: var(--bg-color);
    color: var(--text-color);
}
```

---

# Advantages of CSS Variables

- Reduces repeated code
- Makes maintenance easier
- Improves readability
- Supports dynamic styling
- Helpful in responsive design
- Useful for themes and dark mode

---

# Limitations of CSS Variables

- Older browsers may have limited support
- Variable names are case-sensitive
- Too many variables can make code harder to manage

---

# Difference Between CSS Variables and Preprocessor Variables

| Feature | CSS Variables | SASS/LESS Variables |
|---|---|---|
| Works in browser | Yes | No |
| Dynamic updates | Yes | No |
| Can change with JavaScript | Yes | No |
| Defined using | `--name` | `$name` |

---

# Best Practices

## Use Meaningful Names

```css
--primary-color
--heading-font
--main-padding
```

---

## Store Global Variables in `:root`

```css
:root {
    --main-color: blue;
}
```

---

## Avoid Too Many Variables

Only create variables for reusable values.

---

# Conclusion

CSS Variables are a powerful feature that makes stylesheets more organized, reusable, and easier to maintain. They help developers create scalable designs, responsive layouts, and themes efficiently. Using CSS variables improves both development speed and code quality.
