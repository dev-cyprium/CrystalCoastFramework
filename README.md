# About
Welcome to Crystal Coast. It's a light weight 12 column framework written in SASS. It's inspired by Bootstrap, but contains much fewer features. It's intended for smaller web applications and personal use.
The aim of this framework is to force little design on the website itself. My main vision is to use it as a 'steketon' tool just to layout all the elements on a website and make them responsive.

At this point in time, it doesn't contain any javascript.

This is a student project for ICT Collage by Stefan Kupresak ( github dev-cyprium ).

It's used on a live web-site here as a project to lessons on course "Web design". You can check out the website [here](#).


# Preview
You can preview the examples:
  - Grid example: [open in browser](https://htmlpreview.github.io/?https://github.com/dev-cyprium/CrystalCoastFramework/blob/master/example/grid_example.html)
  - Grid example(with flex layout): [open in browser](https://htmlpreview.github.io/?https://github.com/dev-cyprium/CrystalCoastFramework/blob/master/example/grid_example2.html)
  - Navigation bar example: [open in browser](https://htmlpreview.github.io/?https://github.com/dev-cyprium/CrystalCoastFramework/blob/master/example/navigation_example.html)
  - *TODO: ADD MORE*

# Instalation
You can download the source from github and compile it with SASS, or use download the raw compiled
ready to use css file (`crystal-coast-min.css`).

The project is broken down intro serval modules(components):
  - Grid
  - Reset
  - Typography
  - UI
  - Main

 The compiled version creates one minified file containing all of the components.
 You can change which components to include in your project by downloading the src and exclude
 unwanted components from the `main.scss` file.
 To compile the the source you can use:
 ```shell
 sass main.scss:output.css --style compressed
 ```
 **Warning!!** Mixins are required in order for the other components to work. ( Also, they need to be included **first** ).

# Guide
## The Grid System
Crystal coast supports 12 based grid system. To use it, you need to have a container element and place the desired layout of columns inside. All the elements in the container **MUST** add up to 12.
Supported responsive classes are:
  - m ( medium )
Example 1:
```html
<div class="container">
  <div class="row">
    <div class="c-m-6">6 column span element</div>
    <div class="c-m-3">3 column span element</div>
    <div class="c-m-3">3 column span element</div>
  </div>
</div>	
```
Example 2:
```html
<div class="container">
  <div class="row">
      <div class="c-m-2">2 column span element</div>
      <div class="c-m-8">8 column span element</div>
      <div class="c-m-2">2 column span element</div>
  </div>
</div>
```

## Navigation bar
Crystal coast supports the main navigation bar. To use it, just add the class `.navbar-main` to the nav tag and nest your links in the `<ul> <li> <a>` tags. You can highlit any item in the navigation bar with the class `.active` added to the `<a>` tag.

The navigation bar isn't supported for mobile just yet.

Example:
```html
  <nav class="navbar-main">
    <ul>
      <li><a href="#" class="active">Link 1</a></li>
      <li><a href="#">Link 2</a></li>
      <li><a href="#">Link 3</a></li>
      <li><a href="#">Link 4</a></li>
    </ul>
  </nav>
```


> TODO: WRITE MORE

# Change Log & download
Stable version: 1.0 beta download: [src](#)/[minified](#)

Change log:
 
### version 1.0 beta

 - Add navigation bar
 - Move Mixins to a file including all mixins as helper functions
 - Remove unfinished responsive support tags (l, xl, s, xs)

> TODO: WRITE
