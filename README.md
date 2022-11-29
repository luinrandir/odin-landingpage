# :rocket: Odin's Landing Page

## About

Odin's Landing Page was written to accomplish a project from [The Odin Project](https://www.theodinproject.com/) (TOP). The site is a basic landing page that demonstrates the use of several CSS properties and HTML layouts.

## Built Using

- HTML
- CSS

## Reflection

After doing other projects from TOP, I realized that I can refactor this code to make much more sense semantically for the HTML portion. The use of many `<div>` tags that are properly named with class selectors help slightly to read the HTML. Aside from that, the use of the `flex` property did add some more understanding, but felt odd to use with the "employee" pictures. I do have plans to refactor and transform the landing page, as mentioned below.

## Future Plans

1. Rewrite the HTML to use semantic tags, making it easier to read.

   Take the following snippet of code:

   ```html
   <div class="header">
     <div class="header-left">The box</div>
     <div class="header-right">
       <a href="#" class="nav-link">Our story</a>
       <a href="#" class="nav-link">Who Are We</a>
       <a href="#" class="nav-link">Contact</a>
     </div>
   </div>
   ```

   Even though the class names do mention what each `<div>` is representing, it feels more natural to read the code if it were refactored to the below snippet:

   ```html
   <header>
     <div class="header-left">The box</div>
     <nav class="header-right">
       <a href="#" class="nav-link">Our story</a>
       <a href="#" class="nav-link">Who Are We</a>
       <a href="#" class="nav-link">Contact</a>
     </nav>
   </header>
   ```

   Here when we see the `<header>` tag, we know that we are dealing with the header of the page. Likewise when we see the `<nav>` tag, we know we are dealing with navigation for the page.

2. Refactor CSS by finding similar blocks of code. Will also consider using more utility classes that could assist, such as:

   ```css
   .flex {
     display: flex;
     justify-content: center;
     align-items: center;
   }
   ```

3. Re-purpose the landing page. At the moment, the landing page was created to simply complete the project. Instead, the landing page will be used to be a home page for all completed projects from TOP.

## Live Demo

[Live Demo of Odin's Landing Page](https://luinrandir.github.io/odin-landingpage/)
