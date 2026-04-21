# SEO & Core Web Vitals in HTML

## What is SEO?

**SEO (Search Engine Optimization)** is the process of improving a website so that it ranks higher in search engine results (like Google). It helps increase visibility, traffic, and user engagement.

---

## SEO in HTML

HTML plays a very important role in SEO because search engines read your website structure through HTML.

### Important HTML Elements for SEO

#### 1. **Title Tag**

```html
<title>Learn Web Development | Beginner Guide</title>
```

* Appears in search results
* Should be clear and keyword-rich

---

#### 2. **Meta Description**

```html
<meta name="description" content="Learn HTML, CSS, and JavaScript with easy examples.">
```

* Summary of your page
* Improves click-through rate

---

#### 3. **Heading Tags (H1–H6)**

```html
<h1>Main Title</h1>
<h2>Subheading</h2>
```

* Helps structure content
* Use only one `<h1>` per page

---

#### 4. **Alt Attribute for Images**

```html
<img src="image.jpg" alt="HTML tutorial image">
```

* Helps search engines understand images
* Improves accessibility

---

#### 5. **Semantic HTML Tags**

```html
<header>, <nav>, <article>, <section>, <footer>
```

* Improves readability for search engines
* Better page structure

---

#### 6. **URL Structure**

```
https://example.com/learn-html
```

* Clean and readable URLs are better for SEO

---

#### 7. **Internal Linking**

```html
<a href="/about">About Us</a>
```

* Helps search engines crawl your site

---

## What are Core Web Vitals?

Core Web Vitals are metrics defined by Google to measure **user experience** on a webpage.

---

## Three Main Core Web Vitals

### 1. **Largest Contentful Paint (LCP)**

* Measures loading performance
* Ideal: **< 2.5 seconds**
* Example: Time taken for main content to load

---

### 2. **First Input Delay (FID)**

* Measures interactivity
* Ideal: **< 100 ms**
* Example: Time taken to respond to a click

---

### 3. **Cumulative Layout Shift (CLS)**

* Measures visual stability
* Ideal: **< 0.1**
* Example: Elements moving unexpectedly while loading

---

## How to Improve Core Web Vitals in HTML

### Optimize Images

```html
<img src="image.jpg" loading="lazy" alt="image">
```

---

### Use Proper Font Loading

```html
<link rel="preload" href="font.woff2" as="font" type="font/woff2" crossorigin>
```

---

### Minimize Render Blocking

```html
<link rel="stylesheet" href="style.css">
<script defer src="script.js"></script>
```

---

### Set Width & Height for Images

```html
<img src="img.jpg" width="300" height="200">
```

---

### Use Lazy Loading

```html
<img src="image.jpg" loading="lazy">
```

---

## Why SEO + Core Web Vitals Matter

* Better ranking on search engines
* Faster website performance
* Improved user experience
* Higher traffic and engagement

---

## Summary

| Feature         | Purpose                                  |
| --------------- | ---------------------------------------- |
| SEO             | Improves visibility on search engines    |
| HTML SEO Tags   | Helps search engines understand content  |
| Core Web Vitals | Measures performance and user experience |
| Optimization    | Improves speed and ranking               |

---

## Final Tip

A fast, well-structured HTML page = Better SEO + Better User Experience 

---
