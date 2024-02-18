# README

## Purpose
This is a repository where I will add the content from FreeCodeCamp Responsive Web Design.
If you wish to follow the same steps, please visit https://www.freecodecamp.org/learn/2022/responsive-web-design

The course is made up of several small projects so each one will be hosted in its folder and ordered numerically.   

---

## CSS Colors

Common approaches to color in CSS is to us3:
- RGB Model: rgb(int,int,int) where int can range from 0 - 255
	- Where zero is black and 255 is max intensity for that color. 
- HEX Model: #AABBCC Where all values range from 0 to 9, A to F.
	- This is the hexadecimal model
- The HSL color model, or hue, saturation, and lightness, is another way to represent colors.
	The CSS hsl function accepts 3 values: a number from 0 to 360 for hue, a percentage from 0 to 100 for saturation, and a percentage from 0 to 100 for lightness.
	If you imagine a color wheel, the hue red is at 0 degrees, green is at 120 degrees, and blue is at 240 degrees.
	Saturation is the intensity of a color from 0%, or gray, to 100% for pure color. You must add the percent sign % to the saturation and lightness values.
	Lightness is how bright a color appears, from 0%, or complete black, to 100%, complete white, with 50% being neutral.
 
A gradient is when one color transitions into another. The CSS linear-gradient function lets you control the direction of the transition along a line, and which colors are used.
One thing to remember is that the linear-gradient function actually creates an image element, and is usually paired with the background property which can accept an image as a value.
The linear-gradient function is very flexible -- here is the basic syntax you'll use in this tutorial:    
`linear-gradient(gradientDirection, color1, color2, ...);`   gradientDirection is the direction of the line used for the transition. color1 and color2 are color arguments, which are the colors that will be used in the transition itself. These can be any type of color, including color keywords, hex, rgb, or hsl.
If no gradientDirection argument is provided to the linear-gradient function, it arranges colors from top to bottom, or along a 180 degree line, by default.

Color-stops allow you to fine-tune where colors are placed along the gradient line. They are a length unit like px or percentages that follow a color in the linear-gradient function.
For example, in this red-black gradient, the transition from red to black takes place at the 90% point along the gradient line, so red takes up most of the available space:
`linear-gradient(90deg, red 90%, black);`

## Comit in other date
`git commit --amend --no-edit --date="Mon Feb 05 20:00:00 2024 -0600"`

## Box Model  
By default, the browser includes the border and padding when determining an element's size. 

To solve this, reset the box model by creating a `*` selector and giving it a `box-sizing` property of `border-box`.

![Box Model](https://cdn.freecodecamp.org/curriculum/css-box-model/diagram-3.png "Box Model")

## CSS References
https://www.w3schools.com/css/default.asp

## Flex Box
Flexbox has a main and cross axis. The main axis is defined by the flex-direction property, which has four possible values:

- `row` (default): horizontal axis with flex items from left to right   
- `row-reverse`: horizontal axis with flex items from right to left   
- `column`: vertical axis with flex items from top to bottom   
- `column-reverse`: vertical axis with flex items from bottom to top   
Note: The axes and directions will be different depending on the text direction. The values shown are for a left-to-right text direction.

The `flex-wrap` property determines how your flex items behave when the flex container is too small. Setting it to `wrap` will allow the items to wrap to the next row or column. `nowrap` (default) will prevent your items from wrapping and shrink them if needed.

The `justify-content` property determines how the items inside a flex container are positioned along the main axis, affecting their position and the space around them.

The `align-items` property positions the flex content along the cross axis. In this case, with your `flex-direction` set to `row`, your cross axis would be `vertical`.
Notice how some images may have become distorted. This is because the images have different aspect ratios. Rather than setting each aspect ratio individually, you can use the `object-fit` property to determine how images should behave.

The `gap` CSS shorthand property sets the gaps, also known as gutters, between rows and columns. The gap property and its row-gap and column-gap sub-properties provide this functionality for flex, grid, and multi-column layout. 

## CSS Position

CSS positioning lets you set how you want an element to be positioned in the browser. It has a position property you can set to static, absolute, relative, sticky or fixed.
Once you set the position property of the element, you can move the element around by setting a pixel or a percentage value for one or more of the top, right, left, or bottom properties.
static is the default positioning for all elements. If you assign it to an element, you won't be able to move it around with top, right, left, or bottom.

The transform property allows you to modify the shape, position, and size of an element without changing the layout or affecting the surrounding elements. It has functions such as translate(), rotate(), scale(), skew(), and matrix()

## Media Queries

The `@media` at-rule, also known as a media query, is used to conditionally apply CSS. Media queries are commonly used to apply CSS based on the `viewport` width using the `max-width` and `min-width` properties.

In the below example the padding is applied to the .card class when the `viewport` is `960px` wide and below.
```CSS
@media (max-width: 960px) {   
  .card {    
    padding: 2rem;   
  }     
}   
```