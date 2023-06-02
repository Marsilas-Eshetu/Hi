# Css

CSS NOTES

- CSS is the language we use to style an HTML document.
CSS describes how HTML elements should be displayed

CSS Syntax

A CSS rule consists of a selector and a declaration block.

p {
color: red;
text-align: center;
}

The selector(p) points to the HTML element you want to style.
The declaration block contains one or more declarations separated by semicolons.
Each declaration includes a CSS property name and a value, separated by a colon.

CSS Backgrounds

The CSS background properties are used to add background effects for elements.
background-color

background-image

background-repeat

background-attachment

background-position

background (shorthand property)

CSS Margins

The CSS margin properties are used to create space around elements, outside of any defined borders.
Note:Negative values are allowed.

CSS Padding

The CSS padding properties are used to generate space around an element's content, inside of any defined borders.
Note: Negative values are not allowed.

CSS Icons

The simplest way to add an icon to your HTML page, is with an icon library
Add the name of the specified icon class to any inline HTML element (like <i> or <span>).

CSS Lists

The CSS list properties allow you to:

Set different list item markers for ordered lists

Set different list item markers for unordered lists

Set an image as the list item marker

Add background colors to lists and list items

CSS Layout - Horizontal & Vertical Align

To horizontally center a block element (like <div>), use margin: auto;
Setting the width of the element will prevent it from stretching out to the edges of its container.
The element will then take up the specified width, and the remaining space will be split equally between the two margins:
Note: Center aligning has no effect if the width property is not set (or set to 100%).

Center align text-To just center the text inside an element, use text-align: center;

CSS Height, Width and Max-width

The CSS height and width properties are used to set the height and width of an element.
The CSS max-width property is used to set the maximum width of an element.
The height and width properties do not include padding, borders, or margins. It sets the height/width of the area inside the padding, border, and margin of the element.
Example

Set the height and width of a <div> element:

div {
height:200px;
width: 50%;
background-color: powderblue;
}

CSS Navigation Bar

Having easy-to-use navigation is important for any web site.
With CSS you can transform boring HTML menus into good-looking navigation bars.

Navigation Bar = List of Links

A navigation bar needs standard HTML as a base.
A navigation bar is basically a list of links, so using the <ul> and <li> elements makes perfect sense

CSS Counters

CSS counters are "variables" maintained by CSS whose values can be incremented by CSS rules (to track how many times they are used). Counters let you adjust the appearance of content based on its placement in the document.

Automatic Numbering With Counters
CSS counters are like "variables". The variable values can be incremented by CSS rules (which will track how many times they are used).
To work with CSS counters we will use the following properties:
•	counter-reset - Creates or resets a counter
•	counter-increment - Increments a counter value
•	content - Inserts generated content
•	counter() or counters() function - Adds the value of a counter to an element
To use a CSS counter, it must first be created with counter-reset.

Example
body {
counter-reset: section;
}

h2::before {
counter-increment: section;
content: "Section " counter(section) ": ";
}
