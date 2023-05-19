# Web tech

Note on css and bootstrap 

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

Bootstrap
•	Bootstrap is a free front-end framework for faster and easier web development
•	Bootstrap includes HTML and CSS based design templates for typography, forms, buttons, tables, navigation, modals, image carousels and many other, as well as optional JavaScript plugins
•	Bootstrap also gives you the ability to easily create responsive designs
What is Responsive Web Design?

Responsive web design is about creating web sites which automatically adjust themselves to look good on all devices, from small phones to large desktops.
Advantages of Bootstrap:
•	Easy to use: Anybody with just basic knowledge of HTML and CSS can start using Bootstrap
•	Responsive features: Bootstrap's responsive CSS adjusts to phones, tablets, and desktops
•	Mobile-first approach: In Bootstrap 3, mobile-first styles are part of the core framework
•	Browser compatibility: Bootstrap is compatible with all modern browsers (Chrome, Firefox, Internet Explorer, Edge, Safari, and Opera)
Bootstrap Example
<div class="jumbotron text-center">
<h1>My First Bootstrap Page</h1>
<p>Resize this responsive page to see the effect!</p>
</div>

<div class="container">
<div class="row">
<div class="col-sm-4">
<h3>Column 1</h3>
<p>Lorem ipsum dolor..</p>
</div>
<div class="col-sm-4">
<h3>Column 2</h3>
<p>Lorem ipsum dolor..</p>
</div>
<div class="col-sm-4">
<h3>Column 3</h3>
<p>Lorem ipsum dolor..</p>
</div>
</div>
</div>
Bootstrap Grids
Bootstrap Grid System
Bootstrap's grid system allows up to 12 columns across the page.
If you do not want to use all 12 columns individually, you can group the columns together to create wider columns:
Bootstrap's grid system is responsive, and the columns will re-arrange automatically depending on the screen size.

Grid Classes
The Bootstrap grid system has four classes:
•	xs (for phones - screens less than 768px wide)
•	sm (for tablets - screens equal to or greater than 768px wide)
•	md (for small laptops - screens equal to or greater than 992px wide)
•	lg (for laptops and desktops - screens equal to or greater than 1200px wide)

Bootstrap vs. Browser Defaults
In this chapter, we will look at some HTML elements that will be styled a little bit differently by Bootstrap than browser defaults.

<h1> - <h6>
By default, Bootstrap will style the HTML headings (<h1> to <h6>) in the following way:
EXAMPLE
h1 Bootstrap heading (36px)
h2 Bootstrap heading (30px)
h3 Bootstrap heading (24px)
h4 Bootstrap heading (18px)
h5 Bootstrap heading (14px)
h6 Bootstrap heading (12px)
Breakpoints
Breakpoints are customizable widths that determine how your responsive layout behaves across device or viewport sizes in Bootstrap.
•	Breakpoints are the building blocks of responsive design. Use them to control when your layout can be adapted at a particular viewport or device size.
•	Use media queries to architect your CSS by breakpoint. Media queries are a feature of CSS that allow you to conditionally apply styles based on a set of browser and operating system parameters. We most commonly use min-width in our media queries.
•	Mobile first, responsive design is the goal. Bootstrap’s CSS aims to apply the bare minimum of styles to make a layout work at the smallest breakpoint, and then layers on styles to adjust that design for larger devices. This optimizes your CSS, improves rendering time, and provides a great experience for your visitors.
**Containers**
Containers are a fundamental building block of Bootstrap that contain, pad, and align your content within a given device or viewport.
Containers are the most basic layout element in Bootstrap and are required when using our default grid system. Containers are used to contain, pad, and (sometimes) center the content within them. While containers can be nested, most layouts do not require a nested container.
*Bootstrap comes with three different containers:
.container, which sets a max-width at each responsive breakpoint
.container-{breakpoint}, which is width: 100% until the specified breakpoint
.container-fluid, which is width: 100% at all breakpoints

Extra small<576px
Small≥576px
Medium≥768px
Large≥992px
X-Large≥1200px
XX-Large≥1400px   

 .container
100%
540px
720px
960px
1140px
1320px

.container
100%
540px
720px
960px
1140px
1320px

.container-sm
100%
540px
720px
960px
1140px
1320px

.container-md
100%
100%
720px
960px
1140px
1320px

.container-lg
100%
100%
100%
960px
1140px
1320px

.container-xl
100%
100%
100%
100%
1140px
1320px

.container-xxl
100%
100%
100%
100%
100%
1320px

.container-fluid
100%
100%
100%
100%
100%
100%

**Default Containers**
Our default .container class is a responsive, fixed-width container, meaning its max-width changes at each breakpoint.
<div class="container">
<!-- Content here -->
</div>
**Responsive containers**
Responsive containers allow you to specify a class that is 100% wide until the specified breakpoint is reached, after which we apply max-widths for each of the higher breakpoints. For example, .container-sm is 100% wide to start until the sm breakpoint is reached, where it will scale up with md, lg, xl, and xxl.
<div class="container-sm">100% wide until small breakpoint</div>
<div class="container-md">100% wide until medium breakpoint</div>
<div class="container-lg">100% wide until large breakpoint</div>
<div class="container-xl">100% wide until extra large breakpoint</div>
<div class="container-xxl">100% wide until extra extra large breakpoint</div>
Fluid containers
Use .container-fluid for a full width container, spanning the entire width of the viewport.
<div class="container-fluid">
...
</div>
**Grid System**
Bootstrap's grid system allows up to 12 columns across the page.
If you do not want to use all 12 columns individually, you can group the columns together to create wider columns:
Grid classes
The Bootstrap grid system has four classes:
xs (for phones - screens less than 768px wide)
sm (for tablets - screens equal to or greater than 768px wide)
md (for small laptops - screens equal to or greater than 992px wide)
lg (for laptops and desktops - screens equal to or greater than 1200px wide)
The classes above can be combined to create more dynamic and flexible layouts.

**How it works**
Breaking it down, here’s how the grid system comes together:
Our grid supports six responsive breakpoints. Breakpoints are based on min-width media queries, meaning they affect that breakpoint and all those above it (e.g., .col-sm-4 applies to sm, md, lg, xl, and xxl). This means you can control container and column sizing and behavior by each breakpoint.
Our grid supports six responsive breakpoints. Breakpoints are based on min-width media queries, meaning they affect that breakpoint and all those above it (e.g., .col-sm-4 applies to sm, md, lg, xl, and xxl). This means you can control container and column sizing and behavior by each breakpoint.
Containers center and horizontally pad your content. Use .container for a responsive pixel width, .container-fluid for width: 100% across all viewports and devices, or a responsive container (e.g., .container-md) for a combination of fluid and pixel widths.
Rows are wrappers for columns. Each column has horizontal padding (called a gutter) for controlling the space between them. This padding is then counteracted on the rows with negative margins to ensure the content in your columns is visually aligned down the left side. Rows also support modifier classes to uniformly apply column sizing and gutter classes to change the spacing of your content.
Columns are incredibly flexible. There are 12 template columns available per row, allowing you to create different combinations of elements that span any number of columns. Column classes indicate the number of template columns to span (e.g., col-4 spans four). widths are set in percentages so you always have the same relative sizing.
Gutters are also responsive and customizable. Gutter classes are available across all breakpoints, with all the same sizes as our margin and padding spacing. Change horizontal gutters with .gx-* classes, vertical gutters with .gy-*, or all gutters with .g-* classes. .g-0 is also available to remove gutters.

Sass variables, maps, and mixins power the grid. If you don’t want to use the predefined grid classes in Bootstrap, you can use our grid’s source Sass to create your own with more semantic markup. We also include some CSS custom properties to consume these Sass variables for even greater flexibility for you.
Equal width
The following example shows how to get two various-width columns starting at tablets and scaling to large desktops:
<div class="container text-center">
<div class="row">
<div class="col">
1 of 2
</div>
<div class="col">
2 of 2
</div>
</div>
<div class="row">
<div class="col">
1 of 3
</div>
<div class="col">
2 of 3
</div>
<div class="col">
3 of 3
</div>
</div>
</div>