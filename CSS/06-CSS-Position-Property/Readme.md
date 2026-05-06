# CSS Position Property

The `position` property in CSS is used to control how an element is placed on a webpage. It defines how an element is positioned and how it interacts with other elements.

---

## Syntax

```css
selector {
  position: value;
}
```

---

## Types of Position Values

### 1. Static (Default)

* Default value for all elements
* Elements follow normal document flow
* `top`, `right`, `bottom`, `left` do not work

```css
div {
  position: static;
}
```

---

### 2. Relative

* Positioned relative to its normal position
* Can be moved using `top`, `left`, `right`, `bottom`
* Original space is preserved

```css
div {
  position: relative;
  top: 10px;
  left: 20px;
}
```

---

### 3. Absolute

* Positioned relative to the nearest positioned ancestor
* If no ancestor exists, it uses the `<body>`
* Removed from normal flow

```css
div {
  position: absolute;
  top: 50px;
  left: 100px;
}
```

---

### 4. Fixed

* Positioned relative to the browser viewport
* Does not move when scrolling

```css
div {
  position: fixed;
  bottom: 0;
  right: 0;
}
```

---

### 5. Sticky

* Works like `relative` until a scroll point
* Then behaves like `fixed`

```css
div {
  position: sticky;
  top: 0;
}
```

---

## Positioning Properties

These properties work with non-static positions:

| Property | Description         |
| -------- | ------------------- |
| `top`    | Moves element down  |
| `right`  | Moves element left  |
| `bottom` | Moves element up    |
| `left`   | Moves element right |

---

## Key Differences

| Position | Reference                   | Scroll Behavior  |
| -------- | --------------------------- | ---------------- |
| Static   | Normal flow                 | Scrolls          |
| Relative | Itself                      | Scrolls          |
| Absolute | Nearest positioned ancestor | Scrolls          |
| Fixed    | Viewport                    | Does not scroll  |
| Sticky   | Scroll position             | Sticks on scroll |

---

## Conclusion

The `position` property is essential for layout control in CSS. By understanding each type, you can design flexible and responsive web pages.
