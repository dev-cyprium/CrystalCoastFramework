# About
Welcome to Crystal Coast. It's a light weight 12 column framework written in SASS. It's inspired by Bootstrap, but contains much fewer features. It's intended for smaller web applications and personal use.
The aim of this framework is to force little design on the website itself. My main vision is to use it as a 'steketon' tool just to layout all the elements on a website and make them responsive.

At this point in time, it doesn't contain any javascript.

# Preview
You can preview the examples:
  - Grid example: [open in browser](https://htmlpreview.github.io/?https://github.com/dev-cyprium/CrystalCoastFramework/blob/master/example/grid_example.html)
  - Grid example(with flex layout): [open in browser](https://htmlpreview.github.io/?https://github.com/dev-cyprium/CrystalCoastFramework/blob/master/example/grid_example2.html)
  - *TODO: ADD MORE*

# Instalation
You can download the source from github and compile it with SASS, or use download the raw compiled
ready to use css file (`crystal-coast-min.css`).

The project is broken down intro serval modules(components):
  - Grid
  - Reset
  - Typography
  - Ui
  - Main

 The compiled version creates one minified file containing all of the components.
 You can change which components to include in your project by downloading the src and exclude
 unwanted components from the `main.scss` file.
 To compile the the source you can use:
 ```shell
 sass main.scss:output.css --style compressed
 ```

# Guide
## The Grid System
Crystal coast supports 12 based grid system. To use it, you need to have a container element and place the desired layout of columns inside. All the elements in the container `MUST` add up to 12.
Supported responsive classes are:
  - m ( medium )
  - xs ( extra small )
  - TODO: ADD
Example:
```
<div class="container">
  <div class="c-m-6">6 column span element</div>
  <div class="c-m-3">3 column span element</div>
  <div class="c-m-3">3 column span element</div>
</div>	
```

> TODO: WRITE MORE

# Change Log & download
Stable version: 0.1 beta download: [src](#)/[minified](#)

> TODO: WRITE
