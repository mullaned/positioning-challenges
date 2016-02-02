# Challenge (Walk Through): Fixed positioning

Let's continue from the previous exercise and explore fixed positioning. We will change the position of the header to fixed. 
Firstly we will setup the document. 

**1-**  Create more content (another sidebar & content) otherwise it will be difficult to see the effect of the fixed positioning as we need some scrolling to take place. 

![2-sidebars](img/2-sidebars.png)

**2-**  We need to tidy up our code a little here, we just copied and pasted divs which have ids. Id names must be unique or they will cause all sorts of problems down the line. Because there is now more that one sidebar and content let's make them classes rather than ids. That should solve the issue.

**3-**  Give the header border an id and change its position to fixed.
 
![fixed-header](img/fixed-header.png)

**4-**  This will cause some nasty layout problems! As the header is out of normal flow the divs will move up covering it.

**5-**  We can push the divs down to make room. Add a padding-top to the container to give space to the header.  

**6-**  There is one more issue. When we scroll the content divs move on top of the header. We want the header on top.
  
![fixed-header2](img/fixed-header2.png)

To do this we must change the order of the elements in the 3D space. We will not go into too much detail here but suffice is to say that the `z-index` controls that order.  

![xyz](img/xyz.png)

Let's give the header a high `z-index`, e.g. 100. 

```css
    z-index: 100; /* */
```
 
![header-front](img/header-front.png)

Save you work at this point. We will be continuing with this challenge in the next lesson.
