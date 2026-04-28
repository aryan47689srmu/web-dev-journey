# Entities  in HTML

### What are HTML Entities?

HTML entities are special codes used to display reserved characters or symbols in HTML that would otherwise be interpreted as HTML code.

### Why Use HTML Entities?

Some characters have predefined meanings in HTML:

* `<` is used for tags
* `>` is used to close tags
* `&` is used to define entities

To display these characters on a webpage, we must use HTML entities.

### Syntax

```
&entity_name;
```

or

```
&#entity_number;
```

### Common HTML Entities

| Character | Entity Name | Entity Number |
| --------- | ----------- | ------------- |
| `<`       | `&lt;`      | `&#60;`       |
| `>`       | `&gt;`      | `&#62;`       |
| `&`       | `&amp;`     | `&#38;`       |
| `"`       | `&quot;`    | `&#34;`       |
| `'`       | `&apos;`    | `&#39;`       |
| Space     | `&nbsp;`    | `&#160;`      |

### Example

```html
<p>This is less than symbol: &lt;</p>
<p>This is greater than symbol: &gt;</p>
<p>This is ampersand: &amp;</p>
```
