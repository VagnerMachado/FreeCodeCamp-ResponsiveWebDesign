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
