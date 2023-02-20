---
title: "HTML & CSS Notes"
excerpt: "My Notes from the unit 'Intro to HTML/CSS: Making webpages' on Khan Academy"
---


## Index
1. [HTML](#html)
2. [CSS](#css)

### HTML
```
<!DOCTYPE html>
```
```
<html>

<head>

<meta charset="utf-8">

<title> Name of the tab </title>  

</head>

<body>
```

Bigger Cool Heading
```
<h1> Biggest Heading </h1>
```
Big Cool Heading
```
<h2> 2nd Biggest Heading </h2>
```
To write a paragraph:
```
<p> Paragraph </p>
```
Line break:
```
<br> line break (</br> not required)
```
Text formatting:
```
<em>  Italic </em>

<strong> Bold </strong>
```
Unordered List
```
<ul>  

<li> List Item 1 </li>
<li> List Item 2 </li>

</ul>
```
Ordered list
```
<ol>

<li> List Item 1 </li>
<li> List Item 2 </li>

</ol>
```
Adding an image
```
 <img src= "Link/path to your image" alt="Text to display if image is not being rendered" width="mention either width or height and let the browser calculate the other dimension otherwise images will change based on the viewing device">
```
Make sure to close the tags:
```
</body>
</html>
```

<br>

---

<br>

### CSS

```
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>CSS Basics</title>
```

Use `<style>` to tell the browser to use css parser for reading the style changes:

```
<style>

h2 {  -- element selector
    color: rgb(0, 232, 15);
    }  

body {
    background-color: rgb(97, 250, 255);
      }

#a-unique-id {  -- to modify specific tags
         background-color: rgb(97, 250, 255);
      }

.multiple-para-style {
           background-color: rgb(97, 250, 255);
           }

</style>

</head>
<body>
```

Modifying a specific tag
```

<h2 id="a-unique-id">In the css code make sure to specify using '#'. Use "-" or "_" instead of spaces and make sure the id is unique or browser might do weird things</h2>
```

Modifying multiple tags at once
```
<p class="multiple-para-style">If you want to, for example, put the same bg color to multiple paragraphs/tags without having to define a unique id for all of them, then use the class attribute. In the css code make sure to specify this using "." (dot/period). </p>

<p class="multiple-para-style"> another one! </p>

<p class="multiple-para-style"> DJ KHALED!!! </p>
```
```
</body>
</html>
```
