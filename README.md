# CSS Fundamentals
## Part One: The Key Principles of CSS

## Objectives

- Discuss what CSS does and why it's important
- Cover the basics of HTML
- Differentiate between inline, internal, and external stylesheets
- Demonstrate the anatomy of a declaration block
- Understand how to use class, id, and element selectors, and selector order of importance
- Demonstrate the use of the box model, floats, clear and positioning
- Demonstrate the use of flex box, CSS grid in page layout
- Introduce CSS Frameworks like Bootstrap and Semantic UI

## CSS Basics

What does CSS mean?  
Cascading Stylesheets

Why do we use it?
Make it pretty

## The Good, the Bad and the Ugly

* CSS Zen Garden:  
csszengarden.com

* Eteamz:  
eteamz.com/soccer/pills/jpill.htm

* My Favorite:  
lingscars.com


## The basics of HTML

* Some elements need an opening and a closing tag.
  * `<tag>Content</tag>`
  * `<h1>Heading</h1>`
    * h1 - h6
  * `<p>Paragraph</p>`
* You can nest elements within other elements.
  * `<ul></ul>` (Unordered list) / `<ol></ol>` (Ordered list)
    * `<li>List Item</li>`
  * `<div></div>` (block) / `<span></span>` (inline)
* Some elements are self closing.
  * `<tag />`
  * `<br />`
  * `<img />`


## Inline Styling
```
<tag style="property:value or values;”>
```


## Internal Stylesheets
```
<head>
<meta…></meta>
<title…></title>
<style>
  tag {
    property: property value or values;
  }
</style>
</head>
```


## Anatomy of the Declaration Block

selector(s) { <!--rule set-->
  property: value or values; <!--declaration-->
  property: value; <!--declaration-->
}


## Three Main Types of CSS Selectors

* HTML tags/elements - Least specific
* Classes
  * `.class-name`
* Ids - Most specific
  * `#id-name`

Element Selector:
```
p {
  font-size: 20px;
}
```

Class Selector:
```
.navbar {
  margin-bottom: 0px;
}
```

ID Selector:
```
#main-page-title {
  font-family: sans-serif;
}
```

Selecting Multiple Elements:
```
p, .navbar, #main-page-title {
  color: green;
}
```


## External Stylesheets
- For an external stylesheet we have to add a link in the head that looks something like this:

```
<link rel="stylesheet" href="./stylesheet.css">
```


## The Box Model

4 Elements of the box model:
* Margin
* Border
* Padding
* Content


## Layouts & Positioning - CSS Grid / Flex
Flex-based layout system
- Use this to organize your elements horizontally OR vertically
- CSS Flexbox Froggy is a great resource for this! vvv

Grid-based layout system
- Use this to organize your elements horizontally AND vertically all at once
- CSS Grid Garden is a great resource for this! vvv

These properties make it easy to create well-designed and responsive pages


## CSS Frameworks

Frameworks do a lot of the CSS work for us!!!
You can style your website very quickly by using a framework, but there are some drawbacks.  
[Semantic UI](https://semantic-ui.com/) *my personal favorite*  
[Bootstrap](https://getbootstrap.com/)  
[Materialize](https://materializecss.com/)


## Resources

[Awwwards](https://www.awwwards.com/)  
[codrops](https://tympanus.net/codrops/css_reference/) - Fantastic resource for all things CSS  
[w3schools](https://www.w3schools.com/html/default.asp) - Great HTML resource  
[w3schools](https://www.w3schools.com/html/html_elements.asp) - Great CSS resource  
[CSS Tricks](https://css-tricks.com/) - The best resource for learning and understanding flexbox and grid  
[CSS Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/) - Takes you straight to the grid page  
[CSS MDN](https://developer.mozilla.org/en-US/docs/Web/CSS) - Another goodie  
[CSS Zen Garden](http://www.csszengarden.com/) - Great examples of some rock solid CSS experiences  
[Flexbox Froggy](https://flexboxfroggy.com/) - THE BEST way to learn flex  
[CSS Grid Garden](http://cssgridgarden.com/) - THE BEST way to learn grid





<!-- 
body {
  background-color: green;
  color: purple;
  margin: 0px;
}

/* TITLE START */
#title {
  text-align: center;
  width: 50%;
  /* border-width: 40px 80px;
  border-color: #8600abbd;
  border-style: groove; */
  border: 40px #8600abbd groove;
  margin: auto;
  padding: 50px 30px;
  background-color: thistle;
}
/* TITLE START */

/* BANNER START */
#banner {
  background-color: #4ca4b9;
  border: 40px orange groove;
  border-radius: 100px;
  width: 40%;
  margin-left: 600px;
  text-align: center;
}

#banner-container {
  background-color: grey;
  padding: 20px;
}
/* BANNER END */


/* FUN FACTS START */

/* FUN FACTS END */


/* HORIZONTAL IMAGE START */
#horizontal-image {
  display: flex;
  flex-direction: row-reverse;
  justify-content: center;
}
/* HORIZONTAL IMAGE END */


/* VERTICAL IMAGE START */
#vertical-image {
  display: flex;
  flex-direction: column;
  align-items: center;
}

#vertical-image img {
  width: 50%;
}
/* VERTICAL IMAGE END */

/* GRID-FLEX-IMAGE START */
#grid-flex-image {
  display: flex;
  flex-direction: column;
}

#grid-flex-image img {
  width: 20%;
}

.row {
  display: flex;
}

.yana {
  background-image: url("https://d30womf5coomej.cloudfront.net/ua/c3/f9/19/c2/74c64fdaf592494b83488be5347b8fc9.jpg");
}


/* GRID-FLEX-IMAGE END */


/* GRID IMAGE START */

/* GRID IMAGE END */


/* CARD START */

/* CARD END */ -->
