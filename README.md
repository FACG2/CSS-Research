# CSS-Research
### The reserch contains this main topics: 
* Responsive vs mobile-first design.
* How to write CSS with BEM.

## Responsive vs mobile-first design
> Mobile first is the new RESPONSIVE

**Responsive** It is used to describe the possibility of websites adapting to various output devices. The layout, fonts, image sizes etc. change and or scale according to the size of the browser. This principle enables good readability and usability on desktops, tablets and smartphones. If you’re reading this on a desktop, you can see the effects of the responsiveness by scaling the browser window. Make it very narrow to simulate the look of this site on a smartphone.

**Mobile first** is an approach to responsive design: design for smaller screens first, then add more features and content for bigger and bigger screens. This design approach is also known as "progressive enhancement.

![Mobile First vs. Responsive](http://metamonks.com/wp-content/uploads/responsive-vs-mobile-first-webdesign-022-1024x689.png "Mobile First vs. Responsive")

### Is a mobile-first strategy right for me?
A mobile-first strategy can be immensely successf.
Many companies prefer investing in a website that is adapted for desktop computers and ensuring that mobile users can quickly easily find the information that they are looking for.
So how do you know if you really need to create a mobile-first website? Start by learning more about your website visitors and creating personas based on your most important customer segments and overall business goals; after all, you know more than anyone else who you are trying to target and what you need to achieve. The ideal solution will depend on your clientele, what devices it uses and your budget.
Here are some questions you need to ask yourself:
* Do my customers prefer searching the web on computers or mobile devices?
* Does my clientele mainly use mobile devices to browse the we
___
## CSS with BEM
The **Block**, **Element**, **Modifier** methodology (commonly referred to as BEM) is a popular naming convention for classes in HTML and CSS. Developed by the team at Yandex, its goal is to help developers better understand the relationship between the HTML and CSS in a given project.

CSS Code

```CSS
/* Block component */
.btn {}

/* Element that depends upon the block */ 
.btn__price {}

/* Modifier that changes the style of the block */
.btn--orange {} 
.btn--big {}
```

HTML CODE
```CSS
<a class="btn btn--big btn--orange" href="http://css-tricks.com">
  <span class="btn__price">$9.99</span>
  <span class="btn__text">Subscribe</span>
</a>
```
## Why should we consider BEM?

1. If we want to make a new style of a component, we can easily see which modifiers and children already exist. We might even realize we don't need to write any CSS in the first place because there is a pre-existing modifier that does what we need.
2. If we are reading the markup instead of CSS, we should be able to quickly get an idea of which element depends on another (in the previous example we can see that ```.btn__price``` depends on ```.btn```, even if we don't know what that does just yet.)
3. Designers and developers can consistently name components for easier communication between team members. In other words, BEM gives everyone on a project a declarative syntax that they can share so that they're on the same page.
```diff
-Thanks for your time 
``` 
:bowtie:

