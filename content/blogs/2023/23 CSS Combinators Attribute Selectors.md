---
title: "CSS Combinators Unveiled: Harnessing Attribute Selectors"
author: "Maheen Waris"
description: ""
url: "/blogs/CSS-Combinators-Attribute-Selectors/"
date: "2023-09-23"
tags: ["CSS"]
draft: "false"
toc: "true"
---

## 1. Combinators

In CSS, combinators are used to define relationships between selectors to target specific elements in the HTML document. There are four main types of combinators in CSS: descendant, child, adjacent sibling, and general sibling combinators. Here are examples of each:

### 1. Descendant Combinator (space):

The descendant combinator selects all elements that are descendants of a specified element.

```css
div p {
  color: blue;
}
```

### 2. Child Combinator (>):

The child combinator selects all elements that are direct children of a specified element.

```css
ul > li {
  list-style-type: square;
}
```

### 3. Adjacent Sibling Combinator (+):

The adjacent sibling combinator selects an element that is immediately preceded by a specified element.

```css
h2 + span {
  font-weight: bold;
}
```

### 4. General Sibling Combinator (~):

The general sibling combinator selects all elements that are siblings of a specified element and share the same parent.

```css
h2 ~ p {
  font-style: italic;
}
```

These combinators allow you to create more specific and targeted CSS rules to style different elements based on their relationships within the HTML document.

<hr>

## 2. Attribute Selectors

Attribute selectors allow you to target elements based on their attributes. For example, you can select all elements with a specific `target` attribute value or all input elements with a specific `type` attribute. This provides fine-grained control over your styling.
Here are some examples of attribute selectors:

### 1. Selecting elements with a specific attribute:

```css
a[target] {
  color: red;
}
```

### 2. Selecting elements with a specific attribute value:

```css
input[type="checkbox"] {
  border: 2px solid green;
}
```

### 3. Selecting elements with attributes containing a specific value:

```css
[class*="btn"] {
  background-color: #f0f0f0;
}
```

### 4. Selecting elements with attributes starting with a specific value (prefix match):

```css
img[src^="https://"]
{
  border: 1px solid blue;
}
```

### 5. Selecting elements with attributes ending with a specific value (suffix match):

```css
a[href$=".pdf"] {
  font-weight: bold;
}
```

### 6. Selecting elements with attributes that exactly match a specific value:

```css
input[type="text"] {
  background-color: #fff;
}
```

Attribute selectors are powerful and flexible, allowing you to target and style elements based on their attributes and attribute values.

<script src="https://utteranc.es/client.js"
        repo="maheenwaris/Website"
        issue-term="pathname"
        theme="github-dark"
        crossorigin="anonymous"
        async>
</script>

---
