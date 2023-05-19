# Css note

h2::before {
counter-increment: section;
content: "Section " counter(section) ": ";
}

Example
body {
counter-reset: section;
}

Automatic Numbering With Counters
CSS counters are like "variables". The variable values can be incremented by CSS rules (which will track how many times they are used).
To work with CSS counters we will use the following properties:
•	counter-reset - Creates or resets a counter
•	counter-increment - Increments a counter value
•	content - Inserts generated content
•	counter() or counters() function - Adds the value of a counter to an element
To use a CSS counter, it must first be created with counter-reset.

CSS counters are "variables" maintained by CSS whose values can be incremented by CSS rules (to track how many times they are used). Counters let you adjust the appearance of content based on its placement in the document.

CSS Counters

A navigation bar needs standard HTML as a base.
A navigation bar is basically a list of links, so using the <ul> and <li> elements makes perfect sense

Navigation Bar = List of Links

Having easy-to-use navigation is important for any web site.
With CSS you can transform boring HTML menus into good-looking navigation bars.

CSS Navigation Bar

div {
height:200px;
width: 50%;
background-color: powderblue;
}

Set the height and width of a <div> element:

The CSS height and width properties are used to set the height and width of an element.
The CSS max-width property is used to set the maximum width of an element.
The height and width properties do not include padding, borders, or margins. It sets the height/width of the area inside the padding, border, and margin of the element.
Example

CSS Height, Width and Max-width

Center align text-To just center the text inside an element, use text-align: center;

To horizontally center a block element (like <div>), use margin: auto;
Setting the width of the element will prevent it from stretching out to the edges of its container.
The element will then take up the specified width, and the remaining space will be split equally between the two margins:
Note: Center aligning has no effect if the width property is not set (or set to 100%).

CSS Layout - Horizontal & Vertical Align

Add background colors to lists and list items

Set an image as the list item marker

Set different list item markers for unordered lists

Set different list item markers for ordered lists

The CSS list properties allow you to:

CSS Lists

The simplest way to add an icon to your HTML page, is with an icon library
Add the name of the specified icon class to any inline HTML element (like <i> or <span>).

CSS Icons

The CSS padding properties are used to generate space around an element's content, inside of any defined borders.
Note: Negative values are not allowed.

CSS Padding

The CSS margin properties are used to create space around elements, outside of any defined borders.
Note:Negative values are allowed.

CSS Margins

background (shorthand property)

background-position

background-attachment

background-repeat

background-image

The CSS background properties are used to add background effects for elements.
background-color

CSS Backgrounds

The selector(p) points to the HTML element you want to style.
The declaration block contains one or more declarations separated by semicolons.
Each declaration includes a CSS property name and a value, separated by a colon.

p {
color: red;
text-align: center;
}

A CSS rule consists of a selector and a declaration block.

CSS Syntax

- CSS is the language we use to style an HTML document.
CSS describes how HTML elements should be displayed

CSS NOTES