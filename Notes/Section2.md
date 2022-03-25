# HTML Fundamentals

## Introduction to HTML

HTML: Hyper Text Markup Language. It is one of the three core technologies used in frontend web development:

1. HTML: Hyper Text Markup Language
2. CSS: Cascading Style Sheets
3. JS: JavaScript

HTML is used to design the structure and content of the web page.
HTML consists of different types of elements to describe different types of content:

1. Headers
2. Paragraphs
3. Divisions
4. Links
5. Images
6. Video

Most HTML elements are made up of three parts:

1. Opening tag: _P_
2. Content: HTML is a markup language
3. Closing tag: _/P_

Some elements like the image element does not have a closing tag nor content.
Some elements may contain other elements. The nested elements are called child elements.

## HTML Document Structure

There are four basic elements to the structure of every web page:

1. The document type
2. The HTML container
3. The head section: child of HTML
4. The body section: Child of HTML

## Text Elements

Headings break up the text of the web page into logical sections.
Paragraphs separate large amounts of text into logical thoughts.
Use the STRONG element instead of the B element to make bold text.
Use the EM element instead of the I element to make italic text.

## More Text ELements: Lists

Ordered lists are numbered and the list items are children of an OL element.
Unordered lists are not numbered and the list items are children of a UL element.

## Images and Attributes

Image elements have no content or closing tag.
End the element with a slash before the closing bracket.
Use an attribute, _SRC_, to select the image to display.
Attributes are normally part of the opening tag.
A second attribute that should be added to all image elements is the _ALT_ attribute:

1. The _ALT_ attribute is used by search engines like Google or Bing to know what the image is
2. The _ALT_ attribute is also used by the blind to understand what the image displays

Another attribute to use for images is _WIDTH_. This attribute can resize the image if it is too big or too small.
Changing the width will also change the heighth to keep the aspect ratio of the image. However, the image height can be set manually as well with the _HEIGHT_ attribute.

An attribute that should be used in the **HTML** element is the _LANG_ attribute.
The _LANG_ attribute tells the search engines and web browsers which language in which the page is created.

In the **HEAD** element the attribute for the character set should be set. The _CHARACTERSET_ attribute is an attribute used with the **META** element. The **META** element is placed in the **HEAD** element. It is in the head because it describes an attribute of the web page itself. It is not content that can be displayed. The **META** element is another tag that has no content or closing tag. Close the element with a slash before the closing bracket just like the **IMG** element. Content of the web page always goes in the **BODY** element.

The characterset should usually be set to UTF-8. The UTF-8 characterset can display the web page in any known language.

## Hyperlinks

Hyperlinks or just links are what makes the World WIde Web work. Without hyperlinks the web could not function. Links can point to other pages on the same website or even at other locations on the same web page. Links can also point to pages on other websites. Linking to pages on other web sites is what makes teh web work. All of the different types of links use the same element to point to the other data. This is the anchor, **A** element. Depending upon which type of link you are making you may use different attributes, but it is still the same anhor link that makes the connection.

To connect to a web page outside the local website, you use the _HREF_ attribute with the URL to the web page to which you want to connect. To open a new tab when you connect to the link you need another attribute, _TARGET_. The value of the _TARGET_ attribute will be the value "\_blank" to create a new tab with to the web page to which you linked.

To create a link to another web page on the same web site, just add the path to the html file as the value of the _HREF_ attribute in the anchor.

If you wish to create a link that goes no where use the pound sign (hash tag) as the value for teh _HREF_ attribute of the anchor, **A**, element. Using the pound sign will just cause the link to connect to the top of teh current page. This anchor that goes no where can be a placeholder for a link for which you do not yet have the URL.

## Structuring the Page

The page as it is currently written has no structure. ALl of teh elements just flow one after teh other with no association to any other element or group of elements. This can be fixed by using container elements.

The links just under the **H1** element look like navigation links. They should be grouped to gether using the **NAV** element. This lets the browser know just exactly what they are.

The **H1** and the **NAV** elements are different from the renmainder of the elements on the web page. These two elements really are the header of the web page. Therefore, they should be contained in the **HEADER** element.

The remainder of the elements on the page after the **HEADER** element container are really the heart of teh blog post. Many blogs use the **ARTICLE** element for the meat of teh blog post. However, the **ARTICLE** element could also be used to enclose real-world elements like computers or houses. In this instance, though, it is simply used as the continer for the blog post. Now the **BODY** container contains only two parent elements: the **HEADER** and the **ARTICLE**. Every other element in the **BODY** is contained in one of these two containers.

The top part of the blog article contains a **H2** element, two **IMG** elements, and a **P** element. THis could be called the header of the article. THerefore, wrap these elements into a header container ,too. This second **HEADER** element is a bit subjective. Some may say it is not needed, but it gives a bit of structure to the article.

Lastly, the page needs a copyright statement. This is normally done in a separate container called a **FOOTER** element container. After the footer is added to the body, the **BODY** element now contains three parent elements. The copyright statement could be added in a paragraph or it could just be written as content in the **FOOTER** container. Since the copyright statement is all that is in the \*_FOOTER_ element container, it was added without a paragraph element. Had there been other content in teh footer, it may have amde sense to wrap the copyright statement in a paragraph.

## Semantic HTML

Semantic HTML code is HTML code that "says what it does". The HTML code uses HTML tages todescribe the purpose of the page elements. Semantic HTML codecommunictaes themeaning of its elements to computers and humans alike. This type of HTML coding helps web browsers, search engines, assistive technologies, and human developers understand the components of the web page. The article elemnt used for the body of the blog in the last lecture could just have easily used the **MAIN** element container. The grouping for this page would have worked just as well if the **MAIN** element was substituted for teh **ARTICLE** element container.

## Additional VS Code Extensions

### Image Preview

This extension displays images in the gutter of your editor while you are coding your page. At times you may need to know what a generic named image looks like while you are coding.

### Color Highlight

The color highlight extension becomes very useful while applying CSS to your web page.

### Auto Rename Tag

This is used to assistin renaming elements. If you change the opening tag of an element this extension will change the closing tag for you. THis could be very handy if renewing an older web site for semantic HTML coding.

### Live Server

The live server loads your web page into a web server on your local machine while you are coding. As you save changes to your HTML page, the server automaticlly restarts the web page so you see your changes instantaneously.

## HTML Challenge #1

Add the Related Posts Section to the web page. It is not part of the footer and it is not part of teh article. Create a new **ASIDE** element container and add the post links in that container. The **ASIDE** element is used to add content to the web page that is not part of the article itself.

1. Add the Related Posts in the **ASIDE** element container
2. Create the related posts in an unordered list
3. Each list element will contain:
   A. An image
   B. A link
   C. The name of the post's author

## HTML Challenge #2

1. Wrap all content in a **ARTICLE** element
2. Need to use an entity reference for the arrow: &rarr;
3. Link to image: https://i.ibb.co/Jr7Wh1d/challenges.jpg for codepen
4. Image size = 250 x 250
