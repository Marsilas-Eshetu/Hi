# Bootstrap

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
Containers
Containers are a fundamental building block of Bootstrap that contain, pad, and align your content within a given device or viewport.
Containers are the most basic layout element in Bootstrap and are required when using our default grid system. Containers are used to contain, pad, and (sometimes) center the content within them. While containers can be nested, most layouts do not require a nested container.
Bootstrap comes with three different containers:
.container, which sets a max-width at each responsive breakpoint
.container-{breakpoint}, which is width: 100% until the specified breakpoint
.container-fluid, which is width: 100% at all breakpoints

Default Containers
Our default .container class is a responsive, fixed-width container, meaning its max-width changes at each breakpoint.
<div class="container">
<!-- Content here -->
</div>
Responsive containers
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
Grid System
Bootstrap's grid system allows up to 12 columns across the page.
If you do not want to use all 12 columns individually, you can group the columns together to create wider columns:
Grid classes
The Bootstrap grid system has four classes:
xs (for phones - screens less than 768px wide)
sm (for tablets - screens equal to or greater than 768px wide)
md (for small laptops - screens equal to or greater than 992px wide)
lg (for laptops and desktops - screens equal to or greater than 1200px wide)
The classes above can be combined to create more dynamic and flexible layouts.

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