# Forms and Input Tags in HTML

## &#x20;Introduction

HTML forms are used to collect user input. They are essential for user interaction on websites, such as login pages, signup forms, search bars, and feedback forms.

---

## &#x20;What is a Form?

An HTML form is created using the `<form>` tag. It acts as a container for different input elements like text fields, buttons, checkboxes, etc.

### Basic Syntax:

```html
<form action="server_url" method="GET/POST">
  <!-- form elements -->
</form>
```

### Attributes:

* **action** → URL where form data is sent
* **method** → HTTP method (`GET` or `POST`)

---

## &#x20;Input Tags in HTML

The `<input>` tag is used to create different types of input fields.

### Basic Syntax:

```html
<input type="type_name" name="field_name" placeholder="Enter text">
```

---

## &#x20;Common Input Types

### 1. Text Input

```html
<input type="text" name="username" placeholder="Enter your name">
```

### 2. Password Input

```html
<input type="password" name="password">
```

### 3. Email Input

```html
<input type="email" name="email">
```

### 4. Number Input

```html
<input type="number" name="age">
```

### 5. Radio Button

```html
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
```

### 6. Checkbox

```html
<input type="checkbox" name="hobby" value="reading"> Reading
<input type="checkbox" name="hobby" value="sports"> Sports
```

### 7. Submit Button

```html
<input type="submit" value="Submit">
```

### 8. Reset Button

```html
<input type="reset" value="Reset">
```

### 9. File Upload

```html
<input type="file" name="file">
```

---

## &#x20;Other Form Elements

### 1. Label

```html
<label for="username">Name:</label>
<input type="text" id="username">
```

### 2. Textarea

```html
<textarea name="message" rows="4" cols="50"></textarea>
```

### 3. Select (Dropdown)

```html
<select name="course">
  <option value="bca">BCA</option>
  <option value="btech">B.Tech</option>
</select>
```

### 4. Button

```html
<button type="button">Click Me</button>
```

---

## &#x20;Important Attributes

* **name** → Identifies form data
* **value** → Default value
* **placeholder** → Hint text
* **required** → Makes field mandatory
* **readonly** → Cannot modify value
* **disabled** → Field is inactive

Example:

```html
<input type="text" name="name" placeholder="Enter name" required>
```

---

## &#x20;Conclusion

HTML forms and input tags are fundamental for collecting user data. By combining different input types and attributes, you can create interactive and user-friendly forms.

---

## &#x20;Tip

Use proper labels and validation (`required`, `type="email"`, etc.) to improve user experience and data accuracy.
