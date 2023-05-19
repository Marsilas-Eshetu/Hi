# Bootstrap

# Bootstrap
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

Some components of Bootstrap are the following: navbar, card, alerts, dropdown, containers, and breakpoint.

## Containers in Bootstrap

Containers can be applied by naming the class as “container”. They contain and center the contents placed in them. They also provide margin, padding, alignment and other specifications.

Bootstrap comes with three different containers:

- `.container-{breakpoint}`, which is `width: 100%` until the specified breakpoint
- .container, which sets a max-width at each responsive breakpoint
- `.container-fluid`, which is `width: 100%` at all breakpoints

## Breakpoints in Bootstrap

Breakpoints determine how your responsive layout behaves across device or viewport sizes in Bootstrap.

## The Grid System in Bootstrap

It’s used to divide the page into different components displaying different contents. By default, every screen is assumed to have 12 columns. So these columns are divided to contain contents. classes, “row” and “col” are needed for this system to function.

Example: The following code gives 6 columns if screen is medium and above while it gives full screen for lower screens.
<div class=''-col-mid-6''>
  <p> This is a text </p>
  </div>
