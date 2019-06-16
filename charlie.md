## Lecture Notes

Things to have open before the lecture begins:
  - html.html
  - hasselhoff.html
  - csszengarden.com
  - aliweb.com
  - http://css.maxdesign.com.au/selectutorial/advanced_cascade.htm
  - lingscars.com


First we need to go over the objectives of the lecture. The objectives of the lecture will obviously depend on the classes level of understanding of HTML/CSS going into the lecture. The lecture notes will assume the bare minimum level of understanding. Be sure to tailor the list of objectives before going puling this up in front of everyone.  


Full list of objectives:  
  - Discuss what CSS does and why it's important
  - Cover the basics of HTML
  - Differentiate between inline, internal, and external stylesheets
  - Demonstrate the anatomy of a declaration block
  - Understand how to use class, id, and element selectors, and selector order of importance
  - Demonstrate the use of the box model, floats, clear and positioning
  - Demonstrate the use of flex box, CSS grid in page layout
  - Introduce CSS Frameworks like Bootstrap and Semantic UI


# CSS Basics
Q: What does CSS mean?  
A: Cascading Stylesheets.
Bonus A (if someone asks what "cascading" means): "Cascading" means that styles can fall (or cascade) from one style sheet to another, enabling multiple style sheets to be used on one HTML document.

Q: Why do we use it?  
A: To make the our websites more interesting to look at.


# The Good, the Bad and the Ugly
Take a moment to examine some well styled sites, some poorly styled sheets, and then also lingscars.com because its in some incredible sort of grey area between awful and awesome.  

Briefly explain that well styled sites will get more traffic than poorly styled sites. Poorly styled sites can have some seriously negative impacts on the user experience and make it less likely for the user to make a return visit.


## The Basics of HTML
Begin the lecture with a blank html file.  

Take the time to walk through the basic makeup of an HTML file.

A declaration that the document is an HTML:  
`<!DOCTYPE html>`  

A `head` section - This is a container for metadata (data about data). HTML metadata is data about the HTML document. The metadata is not displayed. Metadata will typically define the document title, character set, styles, links, scripts, and other meta information. It's not _what_ the user will see, but it's _how_ the user will see it.

A `body` section - This contains what the user will actually see.

After describing the above, take a moment to type out some of the more basic tags and demonstrate how they look on the page.  

Headings, paragraphs, and lists are what I think are the more important tags to demonstrate at this point. To show a self closing tag use the image tag with a picture of literally anything. It may also be a good idea to show breaks at this point so that we can mention that now that we are using CSS, we no longer want to rely on breaks to space out our website.  

It may be a good idea to mention `<span>` and `<div>` at this point, but keep in mind that since we aren't styling yet the usefullness of these tags may be hard to explain.

```
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
<p>Paragraph tag - Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
<ol>
  <li>First list item</li>
  <li>Second list item</li>
  <li>Third list item</li>
</ol>
<img src="" alt="Pup Pic"/>
```


## Inline Styling

This is a good time to segue into inline styling. We can do this by explaining that there really isn't anything special about all of these tags. These are mostly here to help us organize our file (we can easily see where our heading is because we used an h1 tag). All of these tags come with some pre-existing stying attached to them.  

Here we can show the class that a `<h1>` tag is no different from an `<p>` tag once you give it a `font-size` of `32px` and a `font-weight` of `bold`

Talk about how inline styling is done.

`<tag style="property:value or values;”>`

Take the `<p>` tag that you built with them and add the inline styling mentioned above:  

`<p style="font-size: 32px; font-weight: bold;">I'm a p tag disguised as an h1 tag 🤫</p>`


## Internal Stylesheets
