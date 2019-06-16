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


## Internal Stylesheets/Anatomy of the Declaration Block

This is a good time to break into an internal style sheet.

We don't have to spend too much time on this section. Show them how the style tag should look and break into the anatomy of a declaration block.

Now that we can see how these declaration blocks should look we can grab an `<h1>` tag and add some simple styling (color is an easy one to demonstrate with).

Once we add some styling to an `<h1>` tag it's important to show the potential strength and weakness of using a tag as a selector. Do this by adding more `<h1>` tags to the page and explaining that you may or may not actually want to manipulate all of your `<h1>` tags. If thats what we want, using the html tag as a selector is a great idea. If not we probably want to be a little more specific.


## Three Main Types of CSS Selectors

Here we can discuss that there are other types of selectors. Be sure to mention that there are a lot of different selectors, but that we're only going to be discussing three because these are the ones that we will be interacting with most often.

We've seen how to add stying to an html element. Now we want to add a class to a single tag and throw some styling on it. Then we take that class and add it to an additional tag.

Once we have some classes thrown about we can take a moment to talk about the id tag and how its the most specific of the selectors we've discussed. We can demonstrate this by adding an id tag to a tag that has a class and changing the value of a property set by its class.

We should then demonstrate how to select multiple elements at once with commas.


## External Stylesheets

Now that we have some styling built in to our internal stylesheet we are beginning to see the clutter that this can lead to. We can also choose to quickly create another html file with a similar layout and demonstrate that if we want to use the styling from that other sheet here we would need to copy and paste the style tag.

This is where external style sheets come into play.

We can create a css file here and paste the declaration blocks from the internal stylesheet into the external sheet, add a link to the css file within our head tags and show how both html files are now using the same styles now.

The benefits of using an external stylesheet should be clear at this point.

## The Box Model

If we haven't already done so this is a good time to bring up the break tag and how we don't need (and should not) rely on these for spacing anymore.

It is easiest to show the box model off inside of the Chrome Web Developer Tools.

Take any element on the page and add a margin, border, and padding to it and then over over each with the dev tools open and point out all of the highlighted parts.

When adding these properties to the element it could be a good idea to show off some of the different properties and values that accomplish the same things.

For example, we could show the class that `margin-top`, `margin-right`, `margin-bottom` and `margin-left` exist, but that we can accomplish the same goals by simply using `margin`

## __THIS CONCLUDES PART ONE OF THIS LECTURE__

In part two we will cover flexbox, grid (maybe?) and linking to external frameworks.
