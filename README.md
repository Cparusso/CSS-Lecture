# CSS Fundamentals
## Part One: The Key Principles of CSS

## Objectives

* (p1) Discuss what CSS does and why it's important
* (p1) Differentiate between inline, internal, and external stylesheets
* (p1) Demonstrate the anatomy of a declaration block
* (p1) Understand how to use class, id, and element selectors, and selector order of importance
* (p1) Demonstrate the use of the box model, floats, clear and positioning
* (p2) Demonstrate the use of flex box, CSS grid in page layout
* (p2) Introduce CSS Frameworks like Bootstrap and Semantic UI


## CSS Basics

What does CSS mean?  
<!-- Cascading stylesheets -->

Why do we use it?  
<!-- Make it pretty. -->


## The Good, the Bad and the Ugly

* CSS Zen Garden:  
csszengarden.com

* Eteamz:  
eteamz.com/soccer/pills/jpill.htm

* My Favorite:  
lingscars.com


## Anatomy of the Declaration Block

selectors {
  property: value or values; <!--declaration-->
  property: value; <!--declaration-->
} <!--rule set-->


## Three Types of CSS Selectors

* HTML tags/elements - Least specific
  * Some elements need an opening and a closing tag.
    * `<tag>Content</tag>`
  * Some elements are self closing.
    * `<tag />`
  * `<h1>Heading</h1>`
    * h1 - h6
  * `<p>Paragraph</p>`
  * `<ul></ul>` (Unordered list) / `<ol></ol>` (Ordered list)
    * `<li>List Item</li>`
  * `<div></div>` (block) / `<span></span>` (inline)
  * `<br />`
  * `<img />`
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


## The Box Model

4 Elements of the box model:
* Margin
* Border
* Padding
* Content

(Use Chrome Web Developer to explore!)


## Three Types of CSS

How do we add CSS to our HTML page?
* Inline
```
<h2 style=property:value or values;”>
```

* Internal
```
<head>
<meta…></meta>
<title…></title>
<style>
h2 {
  property: property value or values;
}
</style>
</head>
```

* External
- For an external stylesheet we have to add a link in the head that looks something like this:

```
<link rel="stylesheet" href="./hasselhoff.css">
```

## Layouts & Positioning - Floats & Clear
Floats - take our elements outside of the standard flow of the webpage
_Go to the w3schools css resource below and play around with these and other properties in the "try it yourself!" section._
```
.grand-canyon-image {
  width: 400px;
  float: left;
}
```
Use clear to make your elements 'clear' any floats and sit inline with the regular flow of the page
```
.park-info {
  clear: both;
}
```


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
