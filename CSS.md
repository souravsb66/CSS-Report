# Report on CSS Flexbox and Grid with Code Samples
  
## CSS Flexbox

The **Flexbox** also known as  Flexible Layout module is a layout model which helps us by providing a more efficient way to layout, align and distribute space among items in a container. The main principle at work is to give the container the ability to change it’s items width and height to best fit in the available space. Another important feature of Flexbox is that it is direction-agnostic as apposed to the regular layouts. It is most appropriate for the components of an application, and small-scale layouts.
  
The flexbox works with mainly 2 axes-
- **Main Axis**
- **Cross Axis**

The **Main Axis** by default works from left to right. The start of the Main Axis is called **Main Start**, the end is called **Main End**, and the distance between the start and the end is called the  **Main Length**. 
  
  
The **Cross Axis** by default is perpendicular to the main axis, working from top to bottom. The start of the Cross Axis is called **Cross Start**, the end is called **Cross End**, and the distance between the start and the end is called the  **Cross Length**. 
![flexbox-CSS-layout](https://user-images.githubusercontent.com/101306694/176899160-d5a1cbb7-8b9f-4fed-94b9-be6ebc2af462.png)


  
Now, lets talk about some of the properties of flexbox. Some, of these properties are meant to be set on the container which is also known as the parent element, or the **"flex container"**, while the others are meant to be set on the children element also known as the **”flex items”**. 
Some of the properties of the flex containers are as follows-
  

- **display** -  it defines a flex container depending on the given value
- **flex direction** - it establishes the main axis thus defining the flex container
- **justify content** - it defines the allignment along the main axis
  

Some of the properties of flex items are as follows-
- **order** - it specifies the order of the flexible item
- **flex** - it specifies the length of a flex item

Now, lets look at some examples-
  
### **3 x 3 Grid**
#### Source Code:
.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.item {
  flex: 0 32%;
  height: 100px;
  margin-bottom: 2%; /* (100-32*3)/2 */
}

#### Output:
![flexbox grid](https://user-images.githubusercontent.com/101306694/176900741-19568229-1da9-4927-9321-1a65c313db05.png)
  
  
## CSS GRID
  
CSS Grid also known as **Grid** is a two dimesnional grid based layout system, with rows and columns which separates the page into several sections which makes the process of designing web pages much more convenient without the use of positioning and floating.

To get started with using CSS Grid we have to define the container element as a grid with **display: grid**, set the column and row sizes with **grid-template-columns** and **grid-template-rows**, and then place the child elements into the grid with **grid-column** and **grid-row**.

Now, let’s talk about some of the important properties of CSS Grid with respect to the grid containers-
  
- **display** - defines the elements as a grid container and establishes a new grid format
- **grid-template** - defines the rows and columns of the grid
- **grid-gap** - specifies the size of gridlines
- **justify items** - align grid items along with inline items
  
  
Some important properties with respect to the grid items-
  

- **grid column/row** - justifies the location of an item within the grid
- **justify self** - alligns a grid item within the self
- **subgrid** - allows grid items to have a grid of their own
  
  
Now, lets look at some examples-
  
#### Source Code:
.wrapper {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
  grid-auto-rows: minmax(100px, auto);
}
.one {
  grid-column: 1 / 3;
  grid-row: 1;
}
.two {
  grid-column: 2 / 4;
  grid-row: 1 / 3;
}
.three {
  grid-column: 1;
  grid-row: 2 / 5;
}
.four {
  grid-column: 3;
  grid-row: 3;
}
.five {
  grid-column: 2;
  grid-row: 4;
}
.six {
  grid-column: 3;
  grid-row: 4;
}

#### Output:
![Grid](https://user-images.githubusercontent.com/101306694/176905893-b165f1bd-a5f9-4e07-832f-8ee2b327465f.png)

## Conclusion
CSS Grid helps us create outer layouts of webpages, we can build very complex and extremely interractive designs with this, whereas flexbox mostly comes in handy where we need to allign items and move blocks.
  
    
    
## References 
- https://www.youtube.com/watch?v=JJSoEo8JSnc
- https://www.youtube.com/watch?v=BNmxUzPRYdw
- https://www.geeksforgeeks.org/introduction-to-css-flexbox/
- https://www.javatpoint.com/css-flexbox
- https://www.w3schools.com/css/css_grid.asp
- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout
- https://smallseotools.com/plagiarism-checker/
