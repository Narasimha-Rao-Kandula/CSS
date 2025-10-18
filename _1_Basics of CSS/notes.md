# Basics of CSS

## What is CSS?

CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation of a document written in HTML or XML. It controls the layout, colors, fonts, and overall visual appearance of web pages. CSS separates the content (HTML) from the styling, making websites more maintainable and flexible.

## Types of CSS

There are three main ways to apply CSS to HTML documents:

### 1. Inline CSS
Inline CSS is applied directly to individual HTML elements using the `style` attribute. It has the highest specificity and overrides other styles.

**Example:**
```html
<p style="color: red; font-size: 20px;">This is a red paragraph with large font.</p>
```

### 2. Internal CSS
Internal CSS is defined within the `<style>` tag in the `<head>` section of an HTML document. It applies to the entire page and is useful for single-page styles.

**Example:**
```html
<head>
<style>
  body {
    background-color: lightblue;
  }
  h1 {
    color: navy;
    text-align: center;
  }
</style>
</head>
```

### 3. External CSS
External CSS is stored in a separate `.css` file and linked to the HTML document using the `<link>` tag. This is the most recommended approach for larger websites as it promotes reusability and easier maintenance.

**Example:**
In HTML file:
```html
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

In style.css file:
```css
.container {
  width: 80%;
  margin: 0 auto;
}