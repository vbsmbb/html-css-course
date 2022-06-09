# Layouts: Floats, Flexbox, and CSS Grid

## Section Intro

## The Three Ways of Building Layouts

1. Layout is the way that text, images, and other content are arranged on the web page
2. The layout gives the page a visual structure into which content is placed
3. Building a layout means to arrange page elements into a visual structure instead of having the elements palced one after the other in normal flow
4. Page layout vs. Component layout

   A. Components also need layout
   
   B. It would not make sense to create a page layout and then let components get placed in a normal flow.
   
   C. You also need to layout components within the page layout

5. The three ways of building layouts in CSS

   A. Floats
   
   - This is an old way of building layouts
   - It uses the FLOAT property
   - This technology is being replaced by Flexbox and CSS Grids

   B. Flexbox
   
   - This is a modern way of laying out components in a one dimensional direction without using floats
   - The flexboxis perfect for component layouts
   
   C. CSS Grid
   
   - This is a two-dimenaional way of laying out components on a web page
   - It also works well with complex components
   
 
## Using Floats

1. When an element is floted, it is removed from the normal flow of the web page
2. Unlike absolute positioning, text and inline elements will wrap around the floated element
3. The container element will not adjust its height due to the floated element
4. If all child elements of a container are floated, the height of the container will collapse (return to 0)

## Clearing Floats

1. You can clear the floats by adding a block element (<div>) with no content to the container with the floated children
2. Then add the clear property to the block element with no content and the floated properties are added back to the container
3. This can get cumbersome and also add numerous empty elements to the HTML code which is not a best practice
4. The clearfix hack is a better way to fix this issue caused by floating all of the children of the container.

	* First add another class to the container where the children were floated
	* Call it "clearfix"
	* Now create a pseudo-element in the clearfix class named after (.clearfix::after)
	* This will create a pseudo element as the last element in the container
	* The pseudo-element must have content so add an empty text content to the element
	* Use the clear: both; property
	* Remember psuedo-elements are inline elements
	* However, the clearfix element must be a blcok element for the clearfix hack to work
	* Add the property, display: block;
	* Now, the floated elements are part of their container again
	
## Building a Simple Float Layout

1. The main header has already been floated so it does not need any further changes
2. However, the article, aside and foother containers need to be layed out to meet the new specs
3. Before the layout is formatted, it makes sense to make the container wider since we are laying out containers side by side
4. Therefore change the width of the container from 800px to 1200px.
5. Float the article container to the left
6. Float the aside container to teh right
7. Notice now that the footer is floated under the aside container
8. Since the footer is its own container, all we need do is add the (clear: both) property to the footer and it will display at the bottom of the page
9. This simple layout is complete

## Box-Sizing: Border-Box

1. If right and left padding is added to our aside then the aside is no longer at the top of teh page, but moves to teh bottom
2. This happens because of the calculation of teh width of the aside container using the standard box model
3. When the left and right padding was added, then the aside container became 380 pixels wide and no longer fit beside the article container
4. A quick fix for this issue is to add the box-sizing property to the aside container and set it to border-box
5. Now, the aside container is back beside the article container where it should be
6. The reason this happened is that the box model sizing was changed due to the border-box property.
7. The aside container will always be it's set width and height regardless of margin and padding.
8. This is such an issue that most CSS developers set the box-sizing property with the broder-box value in the universal selector.
9. Now, the box-sizing is set to border-box for all elements.
10. Our universal selector now has three properties that are applied to every element on teh page:

	* margin: 0;
	* padding: 0;
	* box-sizing: border-box;

## Challenge #1

## Introduction to Flexbox

1. Flexbox is designed to work with a set of children in a container
2. by setting the display proerty to FLEX in the container, the child elements are automatically aligned horizontally across teh web page
3. ALl of the children take the height of the tallest element in the container
4. To center items in the flexbox, add the property align-items to the container with teh value od CENTER
5. To center the items horizontallly across the web page, add the property justify-content to the container with the value of CENTER
6. To add space between the items change the value of the justify-content property to space-between
7. STRETCH is teh default value of teh align-items property

## A Flexbox Overview

1. Flexbox is a set of CSS properties to build a one-dimensional layout
2. The main idea of Flexbox is that empty space inside a container element can be equally divided by its child elements
3. Flexbox makes it easy to align items to one another inside a parent container both horizontally and vertically
4. Flexbox solves common problems such as vertical centering and equal-height columns
5. Flexbox replaces the Floats display mechanism allowing cleaner and fewer HTML and CSS code

### Flexbox Terminology

1. The element upon which flexbox is used is called the flex container
2. To use flexbox on a container, set its display property to the value FLEX
3. The main flow of the itmes in the flex container is called the main axis
4. The perpendicular axis is called the cross axis

### Main Properties of the Flex Container

   1. Gap - space between items (length) [default: 0]
   2. Justify-Content: How to place items along the main axis
   
      * flex-start [default]
      * flex end
      * center
      * space-between
      * space-around
      * space-evenly
      
   3. Align-Items: How to place items along the cross axis
   
      * flex-start [default]
      * flex-end
      * center
      * baseline

   4. Flex-Direction
   
      * row
      * row-reverse
      * column
      * column-reverse
      
   5. Flex-Wrap
   
   	  * nowrap
   	  * wrap
   	  * wrap-reverse
   	  
   6. Align-content
   
      * stretch
      * flex-start
      * flex-end
      * center
      * space-between
      * space-around
      
### Properties of Flex Items

1. Align-Self: Used to override align-items for individual items

   * auto
   * stretch
   * flex-start
   * flex-end
   * center
   * baseline
   
2. Flex-grow: length [default: 0]
3. Flex-shrink: length [default: 1]
4. Flex-basis: auto (define an items width)
5. Flex: shorthand for grow,shrink,basis [default: 0 1 auto]
6. Order: integer (Change order of item w/o changing the HTML code)

## Spacing and Aligning Flex Items

1. Items can be individually by using the Flex Items properties
2. The most used item property is align-self
3. Order can be used to reorder the items in teh flex container

   * An order number less than all of the other items will move the selected item to flex-start
   * An order number larger than all of the other items will move the selected item to flex-end
   
4. Easily add space between the flex items with the GAP property on the flex container

## The Flex Property

1. This item property is actually used to size flex items
2. This property is a shorthand property for the item properties

   * flex-grow
   * flex-shrink
   * flex basis
   
3. Never use the individual properties of the flex shorthand
4. Always use the flex shorthand property
5. Setting flex-grow to 1 (0 is default) will allow the flex items to grow to fill the container
6. Setting flex-shrink to 0, keeps the flex items from shrinking so that they do not overflow teh container

## Adding Flexbox to Our Project

1. In order to get the layouts you want you may need to add some more containers around elements
2. Use a div container to group elements
3. Put a div around the image and link to get them into the correct orientation
4. Use the gap property on the flex container to add space between the flex items
5. Add other margins as required to create the required layout

## Building a Simple Flex Layout

1. You need to group the article and teh aside into another container
2. Add the display property with the FLEX value to teh new container
3. Set the flex shorthand property to allow the items to grow and the width to be 825px for the article and 300px for the aside
4. There should also be a gap of 75px between teh flex items in the new flex container
5. Be sure to set the align-items property
6. The default value for align-items is STRETCH
7. This causes the ASIDE to stretch alll teh way to the end of the article
8. Set the align-items property on the flex container to the value FLEX_START and the aside is now it's normal height

## Challenge #2

## Introduction to CSS-Grid

1. Use display: grid; to create a grid layout
2. The containers are GRID containers
3. The items are GRID items
4. Create the number of columns wanted using the grid-template-columns property
5. Each column will be the size that has been specied in the property
6. Specify the number of rows with the property grid-template-rows
7. Each row will be the size that has been specified in the property
8. Gaps can be cretaed between the rows and columns using the GAP property
9. If you want to be more specific you can use the column-gap and row-gap properties
10. This may be the easiest layout tool yet

## CSS-Grid Overview

1. CSS-Grid is a set of CSS properties that are used for building two-dimensional layouts
2. A CSS-Grid layout can be divided into rows and columns and filled with it's child elements
3. CSS-Grid allows to to write less nested HTML elements and easier to read CSS
4. CSS-Grid is not meant to replace flexbox, but is meant to work with flexbox

### CSS-Grid Terminology

1. Create a grid container by setting its display property to GRID
2. The child elements of the grid container will be the grid items
3. Grid has a row axis and a column axis and the direction of these cannot be changed
4. Grid lines divide up the grid into rows and columns
5. The areas where grid items can be placed are called teh grid cells
6. Gaps can be cretaed between columns and rows. The gaps are called gutters.
7. A grid track can be either a grid row or a grid column
8. Grid container properties

	* Grid-Template-Rows: <track size>
	* Grid-Template-Columns: <track size>
	* Gap: <size>
	* Row-Gap: <size>
	* Column-Gap: <size>
	* Justify-Items
	
		- Stretch <default>
		- Start
		- Center
		- End
	
	* Align-Items
	
		- Stretch <default>
		- Start
		- Center
		- End
		
	* Justify-Content [only used if container larger than grid]
	
		- Start
		- Center
		- End
	
	* Align-Content	[only used if container larger than grid]
	
		- Start
		- Center
		- End
		
9. Grid Item Properties

	* Grid-Column: Start column / End column or Span
	* Grid-Row: Start row / End row or Span
	* Justify-Self	[Horizontal Alignment]
	
		- Stretch
		- Start
		- Center
		- End
	
	* Align-Self [Vertical Alignment]
	
		- Stretch
		- Start
		- Center
		- End
		

## Sizing Grid Columns and Rows

1. Using pixels for column and row sizing is a rigid standard that will not flow well and may not display properly on some displays
2. Use the fractional (fr) unit to allow the columns and rows to resize depending upon the disply size
3. Most of the time it is ok just to specify columns and let the rows automatically adjust
4. The fractional unit is more useful with columns

## Placing and Spanning Grid Items

1. Items can be individually placed into any given cell
2. Use the properties GRID_COLUMN and GRID-ROW to place the indivisual cells
3. An item can spane multiple columns or rows by setting the value of GRID-COLUMN or GRID-ROW to span more than one row or column
4. You can use the SPAN property with the number of cells to span as the second value of teh GRID-COLUMN or GRID_ROW property

## Aligning Grid Items and Tracks

1. Align tracks within the grid container with

	* Justify-Content (Horizontally)
	* Align-Content (Vertically)
	
2. Align items within cells

	* Justify-Items (Horizontally)
	* Align-Items: (Vertically)
	
3. You can align the tracks only when the container is larger than teh content

## Building a Simple CSS-Grid Layout

1. Updated the index.html file from Flexbox layout to grid layout
2. Left the flexbox foprmats for 1-dimensional layouts
3. Removed the flexbox layouts for the actual 2-dimenaional page layout
4. Removed the container that we added for the flexbox page layout
5. For the grid layout, we used two columns
6. The main header was set to span across the whole page
7. The footer was set to span across the whole page
8. The template columns were set to 1fr and 300px because 300px was teh size of the Aside
9. A column gap of 75px was set
10. A row gap of 60px was set
11. THe margin-bottom was removed from the product container and the main header

## Challenge #3

