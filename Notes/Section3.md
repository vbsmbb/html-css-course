# CSS Fundamentals

## Introduction to CSS

### CSS - Cascading Style Sheets

1. CSS is one of the three core technologies for frontend web development.
2. CSS describes the visual style and presentation of the content written in HTML.
3. CSS consists of properties that developers use to format the content
4. CSS code starts with a selector to which styles and properties are applied.
5. The properties(styles) are applied to the selector inside a pair of curly brackets.
6. The properties(styles) inside teh curly brackets make up the declaration block.
7. Each property in the declaration block must end with a semi-colon.
8. The selector with a declaration block create a CSS rule.

## Inline, Internal, and External CSS

1. There are three ways to style with CSS:
   A. _**Inline**_: Add a style to individual HTML elements
   I. Do not do this
   II. Putting the style in the HTML element violates the separation of concerns philosophy of Web Design
   B. _**Internal**_: Add a **STYLE** element in the **HEAD** element and put the properties there
   I. This is OK for small amounts of CSS
   II. However, a large CSS rule set could cause the page to load slowly and create performance issues
   C. _**External**_: Put the CSS rules in an external file (Best!)
2. When using the external style sheet, you need to associate the style sheet with the HTML file
3. Associate the two files using the **LINK** element in the **HEAD** element
   A. The parameter **HREF** in the **LINK** element points to the style sheet
   B. The parameter _REL_ in the **LINK** element describes the relationship of the linked file as a stylesheet.

## Styling Text with CSS

1. Any text property that can be described can be implemented with CSS
2. For example:
   A. Font families
   B. Font sizes
   C. Text case (upper, lower, mixed)
   D. Alignment of the text in its parent container
3. Any elements that are children of a parent element will inherit the parent's style if they are not directly styled themselves.
4. List items
   A. Only the list items are styled; not the **UL** or **OL** elements
   B. The default size of the list element is 16px.

## Combining Selectors

1. The same font-family was applied to all of teh rules in the stylesheet
   A. This is repetitive and not a Best Practice
   B. Can create a selector list to apply properties
2. Another selector is the descendant selector
   A. This occurs when you want to select a child element inside a parent element
   B. This selector is created with: **Parent child**
   C. Now only the child element inside the parent element will be styled even if the same element is styled differently as a parent element.
   D. This works even if you have to use a multiple descendant relationship like **Parent Child1 Child2**
   E. This is not BEst practice because now you are encoding the document structure in the CSS styles.
   F. Again, this violates the separation of concerns between the document structure and the document style

## Class and ID Selectors

1. IDs are unique selectors and can be used only once in an HTML page
2. Classes can be used on multiple elements throughout the page
3. Most FE developers try not to use IDs because the HTML can easily be chaanged and the and may become obsolete
4. Using classes allows for easier changes in the future

## Working with Colors

1. Theory of using colors in code
   A. Use the RGB model
   I. Every color can be represented by a combination of Red, Green, and Blue colors
   II. Each value of the model can be a value between 0 and 255
   B. Can use the rgb notation like: rgb(0, 255, 255) [Cyan]
   C. Can also use RGBA and that is RGB with transparency.
   I. The transparency value can range between 0 and 1.
   II. 1 is no transparency while 0 is complete transparency.
   D. Can also use the hexadecimal notation
   I. Ox = 0 and ffx = 255 Same range as RGB.
   II. Two digits for each color (RGB)
   III. Hexadecimal notation used unless transparency is required then the RGBA model is used.
2. When RGB are the same value you get a grey color.
   A. #000000: black
   B. #ffffff: White
   C. #444444: Dark grey
   D. #b7b7b7: Light Grey

## Pseudo Classes

1. A pseudo class is aclass that finds a prt of an element
2. For example the first line item in an ordered or unordered list
3. Any particular child element can be chosen using the _nth-child()_ pseudo class
4. There are a wide variety of selectors that allow for choosing a child element

## Styling Hyperlinks

1. Hyperlinks are styled using pseudo classes.
2. Using the element selector **A** styles all of teh anchors the same
3. This is not usually what you want
4. It is best to use pseudo classe3s to style the anchors so that each one or each group of anchors can be styled differently
5. The _LINK_ psuedo class would only target anchors with an _HREF_ parameter
6. The visited pseudo only styles links that have been visited
7. The hover pseudo class only styles links when you hover over them
8. The active pseudo class only styles the link when it is being selected
9. The anchor should always be styled with all four pseudo classes and should be styled in the order listed
   A. _LINK_
   B. _VISITED_
   C. _HOVER_
   D. _ACTIVE_
10. They should be styled in this order because this is the priority of the anchor pseudo classes.

## Chrome Dev Tools

1. Open Dev Tools in one of three ways:
   A. Select any point on web page and right click, then select the INSPECT menu item
   B. Using the view menu (Exists in Chrome not in MS Edge)
   C. CNtrl + Shift + I in MS Edge
2. This shows all of the style rules applied to every element on the web page
3. It also shows the actual HTML content that makes up the page
4. You can use this to see how different styles may change the page look and feel

## CSS Theory #1: Conflicts Between Selectors

1. If you have an element that has a class selector, an ID selector and an Element Selector, the ID selector has the highest priority and will override the other two barring any other cascading styles.
2. IF an element is styled by only a class or pseudo class selector and an element selector, then the class or pseudo class selector has priority.
3. The element selector only has the priority when there are no class or ID selectors for the particular element.
4. If there are multiple class or ID selectors on a particular element with priority, then the last ID or class selector will take the priority and style teh element.
5. Selections by priority
   A. Declarations marked !important (Should NOT be used)
   B. Inline style (Should NOT be used)
   B. ID
   B. Class
   C. ELement
   D. Universal Selector (lowest priority)
6. Multiple styles of the same priority selector will alwyas take the style of the last selector in the list.
7. Using the _**!important**_ declaration is just a hack and should not be used.
   A. If you have to use this then you have an issue with your CSS styles
   B. Your selections are too complex and should be simplified to a more basic set of rules
8. Do not use the inline style because with this you lose the separation of conserns which is teh basic web design philosophy.

## CSS Theory #2: Inheritance and the Universal Selector

1. Inheritance is where child elements get the style of their parent element when they have no more specific styles set directly on the element.
   A. Styles set in the **BODY** element are available to all of the elements in the body.
   B. Inherited styles are easily overwritten by any specific style rule that affects a child element.
   C. Inherited properties have the lowest priority of all styles affecting an element.
   D. Not all properties are inherited. It is mostly the properties relating to text that are inherited.
2. The Universal Selector selects every element on the page.
   A. This is useful if we want a certain property applied to all elements on a page that does not get inherited.
   B. This selector has the lowest priority and can be easily overridden.

## Challenge #1

1. Started a challenge in CodePen
2. Pinned the challenge so we can go back to it.
3. My implementation was different from JS so I updated mine to match his
4. Used classes for all CSS entries

## CSS Theory #3: The CSS Box Model

1. The box model defines how elements are displayed on the web page
2. Each and every element on the web page can bee seen as a rectangular box
3. Each of these boxes can have content, a border, and space inside and outside of it
4. The content of the element is the innermost box element
   A. The content can be text, images, a table, etc
   B. The content can contain width and height
5. The next box model element is the border
   A. The border is a line around the element
   B. The border is technically still inside the element
6. The next box model element is padding
   A. The padding comes between the content and the border
   B. It is invisible space around the content
   C. The padding is still considered to be inside the element
7. The next box model element is the margin
   A. The margin creates space around the element
   B. It is considered to be outside the element and between elements
8. The last box model element is the fill area
   A. This is the area that gets filled with background color or background image
   B. This area includes the content, padding, and border parts of teh element
9. The final element width consists of:
   A. The left border plus
   B. The left padding plus
   C. The width plus
   D. The right padding plus
   E. THe right border
10. The final element height consists of:
    A. The top border plus
    B. The top padding plus
    C. The height plus
    D. The bottom padding plus
    E. The bottom border

## Using Margins and Paddings

1. You can start with a clean slate by adding 0 margin and 0 padding to the universal selector
2. This will reset any default margins and paddings and allow you to set your own for the best look of your page
3. The universal selector has a priority of zero so any other more specific feature will override the universal settings
4. In setting horizontal margins and paddings use left and right
5. When setting vertical margins and paddings use bottom only

## Adding dimensions

1. If a width is already set on an element, it can be overridden
2. If you do so and the height is also set, you must set the height to auto in the new selector
3. Failure to set the height to auto will create a deformed image

## Centering our Page

1. To be able to center the whole page, you nust put everything on the page in a container (<div>)
2. THen you give the container a class name
3. Now you can style the container
4. Make the top and bottom margins 0 and the left and right margins auto
5. Making the left and right margins auto will allow the browser to calculate the margins and they will be the same on both sides

## Coding Challenge #2

1. Set the margin and padding to 0 for the universal container
2. The article is the container for the challenge
3. Update the width of the PRODUCT class and set the margins to 0 for top and bottom and auto for left and right
4. Actually it looks better to set the margins for the top and bottom to 50px for the container.
5. Try to be consistentwith setting margins
6. Mostly set the bottom margins
7. To set the margins for the individual items in the list use a descendant selector on the DETAILS-LIST class
8. Use padding for the content in the button to add space around it
9. Use a width of 100% for the button to make it fit across the page
10. Add a top border to the button the same as the article border

## CSS Theory #4: Types of Boxes

1. There are two types of boxes: inline and block level
2. An inline box only takes up the space that it needs for its element
3. A block level box takes as much sace as it can get
4. Block level boxes cannot be on the same line; they create line breaks
5. Inline boxes are within other elements and share space with its parent
6. A block level box is like a header
7. An inline box is like a URL link created in an anchor element, a string element, an emphasize element, button, etc.
8. Most of the HTML elements are block level elements
9. Heights and widths do not apply to inline elements
10. For inline boxes, paddings and margins are only applied horizontally
11. A block level element can be transformed into an inline element with the CSS property DISPLAY set to INLINE
12. An inline element can be transformed into a block level element with the CSS property DISPLAy set to block
13. The padding will be added to all sides of an inline element because the padding is inside the element not outside
14. The DISPLAY setting of INLINE-BLOCK has the best features of both block level and inline boxes
15. Images are naturally inline-block elements

## CSS Theory #5: Absolute Positioning

1. Normal flow versus absolute positioning
2. Normal Flow
   A. Default Positioning
   B. Elements ar laid out according to their order in the HTML code
   C. CSS property POSITION set to a value of RELATIVE
3. Absolute Positioning
   A. Element is removed from the normal flow of the layout
   B. Elemnt is anchored to a particular so=pot
   C. CSS property POSITION set to a value of ABSOLUTE
   D. This element loses any impact on surrounding elements
4. An absolutely positioned element must be positioned in a container that is relatively positioned

## Pseudo-elements

1. Pseudo-elements are not HTML elements, but they can still be selected and styled with CSS
2. Examples of pseudo-elements:
   A. First letter of a paragraph
   B. First line of a paragrap
3. Pseudo-elements are written with 2 colons while pseudo-classes are written with 1 colon
4. The adjacent sibling is the very next element after the element selected in the same parent container
5. The adjacent sibling selector is a plus sign '+'
6. The ::after and ::before pseudo elements are the most used pseudo-elements in CSS
7. The ::after pseudo-elemnts creates a pseudo-element that is the first child of the selected element
8. The first proprty of the ::after or ::before pseudo-elements is the CONTENT property
   A. This property can be empty (like "")
   B. Even if empty, it must be the first property
9. Absolute positioning requires that the parent element of the element to be absolutely positioned has to be positioned relatively
10. To position this pseudo-element absolutely the parent (h2) element must have the property (position: relative)
    A. Now the pseudo-element can be positioned absolutely with the property (position: absolute)
    B. Set the location with the top, bottom, left, and right selectors
    C. For this pseudo-element, use (top: -10px) and (right: -25px)
    D. The negative pixel values cause the pseudo-elemnt to move opposite to way positive values would move it
    E. In this instance it is moved slightly up and to the right of the end of the h2 element
11. This pseudo-element that was created does NOT exist in the HTML code!
    A. It only exists in the CSS code
    B. Ergo it is a pseudo-element and not a real element

## Developer Skill #1: Googling and Reading Documentation

1. Start yoursearch with the type of help you are looking for (i.e. css, html, javascript)
2. THen get more specific as you continue
3. If looking for properties, then the next search item would be property, then the type element
4. MSN (Mozilla Developer Network) is a graet resource for Web coding documentation

## Developer Skill #2: Debugging and Asking Questions

1. Most denugging can be done by going to the place just befoe the issue begins
2. This will find most missing ending labels
3. Use an HTML validator if you just can't find the issue
4. Often times, oneerror will create others so multiple errors can be fixed by finding and fixing the one
5. Always use a validator before going to production to find misspellings and other HTML issues
6. Use a diff checker to compare two code segments to find the differences between the two code segments
7. Keep your CSS selectors simple.
8. Creating complex selectors often leads to unintended design choices
9. Use developer tools! It can help you find and fix issues with CSS design
10. If asking for help, put your code in code pen and add the link to your code in the question
11.

## Challenge #3

1. Each elementcan havemore than one class
2. Use two classes for the color squares
   A. The first class determines the size and shape
   B. The second class determines the color
