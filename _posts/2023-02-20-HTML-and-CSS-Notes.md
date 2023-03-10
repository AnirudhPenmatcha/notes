---
title: "HTML & CSS Notes"
excerpt: "My Notes from the unit 'Intro to HTML/CSS: Making webpages' on Khan Academy"
---


## Jump to section:
- [CSS](#css)

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
Adding a Link
```
<a href="www.google.com"> click here to open google </a>
```
> `<a>` - stands for anchor

If you use the attribute "target" with the value `_blank`, then you can open the link in a new tab

`<a target="_blank" href="www.google.com"> click here to open google </a>`

We can also turn an image into a clickable hyperlink by including it in b/w the anchor tag

`<a target="_blank" href="www.google.com"> click here to open google <img src="link to an image" width="300"> </a>`

To create internal links a.k.a link to a particular section within a page then we can do it with the help of an id. First assign a unique id to that section

`<h2 id="web-history">History of the web</h2>`

Then you can create a table of contents at the top of your webpage like this
```
       <ul>
            <li><a href="#web-history">History of the web</a></li>
            <li>History of HTML versions</li>
        </ul>
```        
Tables (In order to add to add borders and customize them you need to do it through CSS)
```
<table>
  <thead> <!-- Table Column Labels -->
      <tr>
          <th>Pet name</th>
          <th>Species</th>
          <th>Color</th>
      </tr>
  </thead>
  <tbody> <!-- Table Content -->
      <tr> <!-- Entry for the next row -->
          <td>Black & white</td>
          <td>rabbit</td>
          <td>black and white</td>
      </tr>
      <tr>
          <td>Daemon</td>
          <td>cat</td>
          <td>black</td>
      </tr>
      <tr>
          <td>Angel</td>
          <td>cat</td>
          <td>orange</td>
      </tr>
  </tbody>
</table>
```

To comment

`<!-- Comment here whatever you would like to -->`

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
CSS text properties

Changing the font-family
```
p {
     font-family: "Helvetica", sans-serif;
}
```
> The first font will be used. In case it is not available, then the second font will be used. Another thing to note is "serif" or "sans-serif" might be processed differently depending on what the default language of that device is.

Changing the font-size

By default, heading's size is relative to body text size. Here we use "px" and "em" as units for size. "em" is what calculates the relative size. There are multiple types of units for size. You can check online for more info on that.
```
body {
    font-size: 12px;
}
h2 {
    font-size: 1.5em;
}  
```
CSS font styles and shorthand

You can bolden or italicize with CSS too
```
#rabbits-info {
  font-weight: bold;
}

.song-lyrics {
  font-family: fantasy;
  font-size: 13px;
  font-style: italic;
}
```
You can also use something called as a shorthand in the order "style size fontfamily", like so:
<br>
`font: italic 13px fantasy;`

Spacing b/w sentences, underlining, text alignment(left, center, right, justify)
```
.song-lyrics {
 text-decoration: underline;
 line-height: 1.5em;
 text-align: center;
}
```
>You can even use "text-decoration" to remove underlining from hyperlinks

CSS inheritance<br>
When you modify properties in tags like body, the changes will be reflected throughout the page unless overridden. For example, if you set the font size as 10 in body and in a h2 tag you modify it to 5, then the h2 heading will be 5.
However, not all properties are inherited by the entire page.   





```
</body>
</html>
```
## Jump to sections:
- [HTML](#html)
