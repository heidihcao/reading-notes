# [<==Home](README.md)

## CSS: Cascading Style Sheets ##

[x] *Up in <head. </head> add a link tag in order to link HTML to CSS sheet*
![image](https://user-images.githubusercontent.com/89883742/133905208-b52d7ba0-aea7-4c25-b578-2b2e73715736.png)

[x] [TWO OTHER WAYS TO INSERT CSS](https://www.w3schools.com/css/css_howto.asp)

### CSS Syntax ###
>h1 {
>    color: red;
>    font-size: 5em;
>}

>p {
>    color: black;
>}

### CSS Color Property ###
Value | Day
------------ | -------------
color| Specifies the text color. [CSS Color Values, a complete list of possible color values](https://www.w3schools.com/cssref/css_colors_legal.asp)
initial| [Sets this property to its default value](https://www.w3schools.com/cssref/css_initial.asp)
inherit| [Inherits this property from its parent element](https://www.w3schools.com/cssref/css_inherit.asp)


#### inherit ####
span {
  color: blue;
}

.extra span {
  color: inherit;
}

#### initial ####
div {
  color: red;
}

h1 {
  color: initial;
}

#### Different HEX colors with transparency ####
#p1a {background-color: #ff000080;}   /* red transparency */
#p2a {background-color: #00ff0080;}   /* green transparency */
#p3a {background-color: #0000ff80;}   /* blue transparency */

#### RGB Colors ####
**An RGB color value is specified with the rgb() function, which has the following syntax:
rgb(red, green, blue)**

#p1 {background-color: rgb(255, 0, 0);}   /* red */
#p2 {background-color: rgb(0, 255, 0);}   /* green */
#p3 {background-color: rgb(0, 0, 255);}   /* blue */
