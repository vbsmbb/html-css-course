# Web Design Rules and Framework

## Section Intro

1. This section focuses on Web Design not development
2. The goal of this section is not to become a graphic design artist, but rather a developer who can create a reasonably thoughtout web page
3. Jonas created a web design framework that we will be using to help us with website design

## Project Overview

1. We will not be building on our project from Section4
2. This section will work on a new project that is contained in the Starter -> Design folder
3. Copy the files to the working directory
4. The HTML for this project is complete and there is a skeleton CSS style sheet
5. The goal of this project will be to add to the CSS to enahnce the web page design and to learn some new CSS functionality

## Overview of Web Design and Website Personalities

1. Web designers create the overall look and feel of a website
2. Web developers implement the design using HTML, CSS, and Javascript code
3. In the early days of web design, the web designer would use a special software like PhotoShop to create the design and teh web developer would implement the design using HTML, CSS, and Javascript
4. The goal of this section is to help web developers become web site designers
5. Good Design:

	* Creates a lasting impression on the user/viewer of the brand or product
	* Makes the user trust the brand
	* Increases the perceived value of the brand or product
	* Gives users exactly waht they were looking for when coming to the site
	
6. Bad Design:

	* User might believe the brand does not really care for their product or service
	* Makes the user insecure about the brand
	* Makes the brand or product seem cheap
	* Leaves users confused and makes it hard for them to reach their goal
	
7. Build a solid web design is not about artistry, it is about following a framework or system to meet teh goals of the brand or product
8. Anyone can learn good web design, you don't have to be artistic or creative
9. There are nine different areas of design that we will learn to apply to any website that we are designing
10. Each of these areas of design contain a number of rules that will be applied depending upon the personality of the website
11. The areas of design of a well-designed website

	* Typography
	* Colors
	* Images/Illustrations
	* Icons
	* Shadows
	* Border-radius
	* White space
	* Visual hierarchy
	* User experience
	* Componants and layout
	
12. The rules applied to each area of design will be based on the website personality
13. Website personalities

	* Serious/elegant
	
		- Based on thin serif typefaces
		- Use golden or pastel colors
		- Use big, high-quality images
		
	* Minimalist/simple
	
		- Focuses on the essential text content
		- Uses small or medium sized sans-serif black text
		- Uses lines
		- Uses few images or icons
		
	* Plain/neutral
	
		- Used by large corporations sometimes
		- Uses neutral and small typefaces
		- Uses a very structured layout
		
	* Bold/confident
	
		- Makes an impact
		- Uses big and bold typography
		- Uses big and bright colors
		
	* Calm/peaceful
	
		- Use for products and services that CARE
		- Use calming pastel colors
		- Use soft serif headings
		- Use matching images/illustrations
		
	* Startup/Upbeat
	
		- Used a lot by startup companies
		- Use medium-sized sans-serif typefaces
		- Use light-gray text and backgrounds
		- Use rounded elements
		
	* Playful/Fun
	
		- Use colorful and round designs
		- Use handdrawn icons, illustrations,and animations
		- Use fun language
		
## Webdesign Rules #1: Typography

1. Typography is the most import web design area
2. Typography has more rules than any of the other design areas
3. What is typography?

	* Typography is the art of arranging type to make written language legible, readable, and appealing
	* Typography is about making text beautiful and easy to read
	
4. Serif versus sans-serif?

	* Serif typefaces
	
		- Have decorative lines at the bottom of the characters
		- Creates a more traditional/classic look and feel
		- Conveys trustworthiness
		- Good for long text
		
	* Sans-serif typefaces
	
		- Do not have the decorative lines at the bottom of the characters
		- They have a modern look and feel
		- They look clean and simple
		- Easier to choose for beginner design
		
5. The rules of typography

	* Use only good and popular typefaces, play it safe
	
		- Sans-serif
		
			+ Inter
			+ Open Sans
			+ Roboto
			+ Montserrat
			+ Work Sans
			+ Lato
			
		- Serif
		
			+ Merriweather
			+ Aleo
			+ Playfair Display
			+ Cormorant
			+ Cardo
			+ Lora

		- It is OK to use only one typeface per page, two at most
		- Choose the correct typeface depending upon your website personality
	* Use good fontsizes and weights
	
		+ Limit font-size choices
		+ Use a typescale tool or other predefined range
		+ Use a font size between 16px and 32px for normal text
		+ For long text (i.e. blog), use 20px or larger
		+ For headlines, you can use 50+px and 600+ boldness
		+ Do not use a font weight of less than 400 for any text
	* Create a good reading experience

		+ Use less than 75 characters per line
		+ For normal sized text, use a line height between 1.5 and 2.0
		+ Decrease letter spacings in headlines if they look unnatural
		+ Use All caps for short titles

			- Make them samll and bold
			- Increase letter spacing
			
		+ Do not justufy text
		+ Do not center long text blocks
		+ 
		
6. Use Google Fonts and Fontsquirrel to get typefaces you need [Toolbox]

## Implementing Typography

1. Used Inter to change the typeface on the new HTML page
2. Changed the size and spacing on the different headers and paragraphs
3. Used different line heights depending upon the amount of writing in an area

## Webdesign Rules #2: Color

### Choose the Right Color

1. The color of the website has to match the website's personality
	* *Red* draw a lot of attention and symbolizes power, passion, and excitement
	* *Orange* is less aggressive and conveys happiness, cheerfulness, and creativity
	* *Yellow*: joy, brightness, and intelligence
	* *Green*: harmony, nature, growth, and health
	* *Blue*: peace, trustworthiness, and professionalism
	* *Purple*: wealth, wisdon, and magic
	* *Pink*: romance, care, and affection2. 
	* *Brown*: nature, durability, and comfort
	* *Black*: power, elegance, minimalism, grief, and sorrow
2. Use a good color tone
	* Do not use the CSS color name
	* Do not use a random tone
	* Use the Open color [Toolbox] color picker to collect the correct color tone
	* Also, tailwindcss [Toolbox] has beautiful colors associated with the framework
	* Some people use tailwindcss simply for teh colors
	* Some people use FLAT UI COLORS 2 [Toolbox] to select the main color for teh website
	
### Establish a Color System

1. At least two types of colors are required:
	* A main color
	* A gray color
2. To add complexity to the design, you can add an accent color
3. You will also need lighter and darker versions of teh colors in your color palette
	* Lighter versions are tints
	* Darker versions are shades
4. Tools to generate the accent color
	* Palleton [Toolbox]
	* Coolors [Toolbox]
5. Colors are used to draw attention to the most important element on the page
6. Do not make text too light
	* Use a tool like COOLORS to check the contrast between the text and background colors
	* Contrast ratio for normal text is 4.5:1
	* Contract ratio for large text should be 3:1
	
## Implementing Colors

1. Styled the button which was actually links
2. When styles were added to BTN only the large button in the header looked good, buth the ones at the bottom of the page were too big
3. Used the BTN--BIG and BTN--SAMLL classes to size the buttons individually
4. Made the background color of the buttons the main color of the page
5. Made the background color of the testimonial section the main web page color
6. Changed the text color to white for better contrast
7. Added some padding so you could see the backbrgound color around teh image

## Webdesign Rules #3: Images and Illustrations

1. Images are the MOST imprtant content of any webpage
2. Types of images to use:
	* Product photos
	* Storytelling photos
	* Illustrations
	* Patterns
3. Use images to support your websites message and story [Use only relevant images]
4. Use original images if possible
5. If not possible, then use high quality stock images
6. Sites with images that can be used:
	* Unsplash [Very good]
	* Pexels
	* DrawKit
	* unDraw

### Use Images Well

1. Try to use real people
2. If necessary, crop the images to fit your message
3. You can also combine photos, illustrations, and patterns to create interesting detail and effects

### Handling Text on Images

1. Darken or lighten image where the text is
2. Position text into a neutral image area
3. Put the text in a box

### Technical Details of Using Images

1. To account for High resolution screens: make image dimensions twice as big as their displayed size
2. Compress images for smaller file size and better performance
3. Use a tool like SQUOOSH [Toolbox] to compress images
4. Side by side images must have the same dimensions

## Webdesign Rules #4: Icons

1. Use good icon pack, niot just random icons found online
2. Free icon packs
	* Phosphor icons
	* ionicons
	* icons8
3. You can use emojis instead of iconpacks
4. Use ony ONE iconpack on any page
5. Use only SVG icons or icon fonts
6. Do not use JPG or PNG (bitmap type) icons. They do not scale well.
7. Icons should adjust to yoru website personality
	* Roundness, weight, and filling should match typography on webpage
	* Icons are often used with the text
	
### When to Use Icons

1. Use icons to provide visual assistance to text
2. Use icons to build product feature blocks
3. Use icons associated with actions, and label them
4. Use icons as bullet points

### How to Use Icons

1. To keep icons neutral, use same color as text. To draw more attention use different color.
2. Do not use icons which do not make sense or fit text or action
3. Do not maek icons larger than they were designed for

## Implementing Icons

1. Used the icons from the HEROICONS website (SVG icons)
2. Not a large icon pack, but very easy to use
3. Added the SVG code to the index.html file
3. Added Icons to the feature block
4. Added icons to the chair features list

## Webdesign Rules #5: Shadows

1. Shadows create depth in the UI design. 
	* The more shadow, the farther away from the interface the element is
	* The farther away from the interface the element is, the larger the shadow on the interface
2. Shadows can be used on boxes and text

### Use Shadows Well
1. Only use shadows if they fit your website personality
2. Serious/elegant designs use less to no shadows at all
3. Shadows increase as we go down the scale toward more playful/fun websites
4. Always use shadows in small doses
5. Go light on shadows. Do not make them too dark.

### Use Shadows Correctly
1. Use small shadows for smaller elements to help them stand out (i.e. CTA buttons and small images)
2. Use medium-sized shadows for larger areas that should stand out from the page 
	* Make entire sections of a page float above the page
	* Make cards stand out from the interface
3. Use large shadows for elements that should really float above the interface
	* Navigations
	* Pop-up windows
4. Experiment with changing shadows on click and hover events
	* Normal - No shadow
	* Hover - Use medium shadow
	* Click - Use small shadow (Gives appearance of button movement)
5. Colored shadows can make the element appear to glow

## Implementing Shadows

1. Updated the CHAIR element to add a shadow to it
2. Made the Hprizontal size zero so that the shadow appears to come from the top
3. Left the vertical size at 20px
4. Changed the blur to 30px
5. Left the shadow color black, but made the transparency only 7%
6. This makes a very suttle shadow and creates a semblance of an edge around the chair cards

## Webdesign Rules #6: Border-Radius

1. Use border-radius to increase the playfulness and fun of the design [Makes it less serious]
2. Assure that border-radius matches the roundness of the typeface used on the page
3. Use border-radius on:
	* Buttons
	* Images
	* Around icons
	* Standout sections
	* Other elements
	
## Implementing Border-Radius

1. Used a small value of border-radius for the images and the testimonial section to match the text roundness
2. For a section, it should have the same amount of border-radius as the included images
3. Used a much larger value of border-radius for the buttons. This makes tem very round.
4. To make the buttons round make sure that the border-radius is larger than the element height
5. Using 50% border-radius will make an image round if it is a perfect square
6. If the image is a rectangle, the 50% value will create an oval instead of a circle 

## Webdesign Rules #7: Whitespace

1. It is one of the easiest and fastest ways to improve a page design
	* The correct amount of whitspace can make a page look clean, modern, and ploished
	* Makes the page easier for the user to understand
2. Whitespace communicates how different pieces of information are related to each other
3. Whitespace implies invisible relationships between the elements of a layout

### Where to Use Whitespace

1. Use lots of whitespace between sections
2. Use a lot of whitespace between groups of elements
	* Generally, more vertical whitespace is required than horizontal
3. Use whitespace between elements
4. Inside groups of elements, try to use whitespace instead of lines

### How much Whitespace to Use

1. The more some elements belong together, the closer they should be to each other [Law of Proximity]
2. Start with more whitespace than is needed and remove until the spacing looks natural
	* Too much whitespace looks detached
	* Too little whitespace looks cramed
3. Whitespace should match other design choices:
	* Big text or big icons require more whitespace
	* Smaller text or smaller icons require less whitespace
4. Use a multiple of 16px for all paddings and margins on the page (2, 4, 8, 16, 32, 64, 128...)

## Webdesign Rules #8: Visual Hierarchy

1. Visual hierarchy establishes which elements of a design are the most important
2. Visual hierarchy is about drawing attention to the most important elements on the page
3. Visual hierarchy defines a path for the users to guide them through the page
4. To establish a visual hierarchy use a combination of:
	* Position
	* Size
	* Colors
	* Spacing
	* Borders
	* Shadows

### Visual Hierarchy Fundamentals

1. Position important elements closer to the top of the page [Get most attention there]
	* The first CTA button should be near the top of the page
2. Use images carefully, they draw a lot of attention
	* Smaller images draw less attention
	* Larger images draw more attention
3. Use whitespace strategically to emphasize elements

### Visual Hierarchy for Text Elements

1. To convey importance use:
	* Font size
	* Font weight
	* Color (text and background)
	* Whitespace
2. What text elements should be emphasized?
	* Titles
	* Sub-titles
	* Links
	* Buttons
	* Data points
	* Icons
	* De-emphasize less important text:
		+ Labels
		+ Secondary/additional information

### Visual Hierarchy Between Components

1. Emphasize an important component by using:
	* Background color
	* Shadow
	* Border
2. Emphasize component A over component B by de-emphasizing component B
3. Which components should be emphasized?
	* Testimonials
	* Call-to-action sections
	* Highlight sections
	* Preview cards
	* Forms
	* Pricing tables
	* Important rows/columns in tables

## Implementing Whitespace and Visual Hierarchy

1. Added more space between the sections
2. Added more distance between the icons and the headers below them
3. Changed a couple of colors in the testimony to make the main text stand out more
4. Added more space in the chair feature cards between the features and the 'Add Chair' CTA button

## Webdesign Rules #9: User Experience

### What is User Experience (UX)

1. The User Interface (UI) is the digital presentation of any digital product
2. How the digital product looks and feels is the User Interface (UI)
	* The Layout
	* The Personality
	* The typography, colors, icons, etc.
3. How the digital product works is the User Experience (UX)
	* Does the application feel logical and well thought out?
	* Does the navigation work intuitively?
	* Are users reaching their goals?

### UI and UX Design

1. UI design is what makes an interface pleasing to the eye
2. UX design is what makes the interface useful and functional
3. UX design cannot exist without UI design

### UX Design Goals

1. A website exists for a reason
	* A user has a reason to visit the site
	* A business or owner has a reason for creating it
	* Users' goals
		- Use a product
		- Find information
		- Buy a product
	* Business' goals
		- Help a user find a product
		- Provide a user with information'
		- Present a product for the user to buy
2. UX design aligns the users' goals with the business' goals

### UX Rules for Usability

1. Do NOT design complicated layouts
	* Do not reinvent the wheel
	* Use patterns that users know
	* Familiarity with layout is more important than being original
2. Make your Call To Action (CTA) the most prominent element
	* Make the text descriptive
	* Make sure the CTA describes what will happen when the user selects it
3. Use blue text and underlined text for LINKS only!
4. Animations should have a purpose and be fast
	* 200 to 500 ms
	* Don't use animations just because you can
5. Align labels and fields in a single vertical line
	* It makes the form easier to scan
	* It looks more professional
6. Offer users good feedback for ALL actions
	* Form errors
	* Form success
	* Web apps
7. Place action buttons where they will create an effect
	* This is the law of locality
	* This is mostly for web apps
	* This does not apply to CTA buttons

### UX Rules for Website Content

1. Use a descriptive, key-word focused headline on your main page
	* Don't be vague or fancy
	* Get to the point
2. Only include relevant information
	* Cut out fluff
	* Make the content 100% clear
3. Use simple words
	* Avoid technical jargon
	* Avoid "smart sounding" words
4. Break up long text with:
	* Sub-headings
	* Images
	* Block quotes
	* Bullet points

## The Website-Personalities Framework

1. The nine website rules we learned should be applied according to the selected website personality
2. There are seven website personalities and they use each of the rules that we learned differently
3. The website personality is the feeling about the website that the web page tries to transmit to the user
4. Choosing the correct website personality makes the design easier for the developer
	* Once the personality is chosen there are fewer choices in each webdesign rule to consider
	* Each website personality has different traits and the design must fit the personality to transmit the correct vibe to the user

### Personality #1: Serious/Elegant

1. Overview:
	* Design for luxury and elegance
	* Based on thin serif typefaces
	* Use golden or pastel colors
	* Use big, high-quality images
2. Industries:
	* Real estate
	* High fashion
	* Jewelry
	* Luxury products or services
3. Webdesign ingredients:
	* Typography:
		+ Small serif typefaces
		+ Light font weight
		+ Small body font size
	* Colors:
		+ Gold or pastel colors
		+ Black
		+ Dark blue or grey
	* Images:
		+ Large, high-quality images
		+ Feature elegant
	* Icons:
		+ Usually no icons are used
		+ However, thin icons and lines may be used
	* Shadows: Usually none
	* Border-radius: Usually none
	* Layout
		+ Create and experimental layouts are common
		+ Special layout not required but often used

### Personality #2: Minimalist/Simple

1. Overview:
	* Focuses on the essential text content
	* Uses small to medium size sans-serif black text
	* Uses lines and few images or icons
2. Industries:
	* Fashion
	* Portfolios
	* Minimalism companies
	* Software startups
3. Webdesign ingredients:
	* Typography:
		+ Boxy/squared sans-serif typefaces
		+ Small body font sizes
	* Colors:
		+ Usually black or dark grey
		+ On pure white backgrounds
		+ Usually just once color throughout the design
	* Images:
		+ Usually few images
		+ Usually no illustrations
	* Icons: Usually none
	* Shadows: Usually none
	* Border-radius: Usually none
	* Layout:
		+ Simple layout
		+ Narrow, one-column layout is common

### Personality #3: Plain/Neutral

1. Overview:
	* Uses design that gets out of the way
	* Uses very neutral and small typefaces
	* Uses a boxy, structured, and condensed layout
2. Industries:
	* Well-established corporations
	* Companies that do not want to make an impact through design
3. Webdesign ingredients:
	* Typography:
		+ Uses sans-serif typefaces
		+ Text is small with little visual impact
	* Colors:
		+ Safe colors employed
		+ Nothing too bright or washed-out
		+ Blues and blacks are common
	* Images: 
		+ Frequently used
		+ Small-format images are used
	* Icons: Usually no icons
	* Shadows: Usually no shadows
	* Border-radius: Usually no border-radius
	* Layout:
		+ Structured and condensed
		+ Lots of boxes and rows

### Personality #4: Bold/Confident

1. Overview:
	* Design that makes an impact
	* Features big and bold typography
	* Paired with confident use of bold colored blocks
2. Industries:
	* Digital agencies
	* Software startups
	* Travel 
	* "Strong" companies
3. Webdesign ingredients:
	* Typography:
		+ Boxy/squared sans-serif typefaces
		+ Big and bold typography (especially headings)
		+ Uppercase headings are common
	* Colors:
		+ Usually multiple bright colors
		+ Big/color block sections used to grab attention
	* Images: Lots of big images
	* Icons: Usually none
	* Shadows: Usually none
	* Border-radius: Usually none
	* Layout:
		+ All kinds of layouts used
		+ No particular tendencies used

### Personality #5: Calm/Peaceful

1. Overview:
	* For products and services that care about the consumer
	* This vibe transmitted through
		+ Pastel colors
		+ Soft serif headings
2. Industries:
	* Healthcare
	* Products with customer well-being in mind
3. Webdesign ingredients:
	* Typography:
		+ Soft serif typefaces frequently used for headings
		+ Sans-serif headings could be used (Software products)
	* Colors:
		+ Pastel/washed-out colors
		+ Light oranges, yellows, browns, greens, blues
	* Images:
		+ Usually used
		+ They should match teh color palette
	* Icons: Frequently used
	* Shadows:
		+ Usually no shadows
		+ Could be used sparingly
	* Border-radius: Some is usual
	* Layout:
		+ All kinds used
		+ No particular tendencies

### Personality #6: Startup/Upbeat

1. Overview:
	* Widely used in startup companies
	* Features medium-sized, sans-serif typefaces
	* Uses light-grey backgrounds
	* Uses rounded elements
2. Industries:
	* Software startups
	* Modern-looking companies
3. Webdesign ingredients:
	* Typography:
		+ Medium-sized headings (not too large)
		+ Usually one sans-serif typeface
		+ Tendency for lighter text colors
	* Colors:
		+ Blues, greens, and purples are widely used
		+ Lots of light backgrounds (mostly grey)
		+ Gradients are common
	* Images:
		+ Images or illustrations are always used
		+ 3D illustrations are modern
		+ Sometmes patterns and shapes add visual details
	* Icons: Used frequently
	* Shadows: 
		+ Subtle shadows are frequent
		+ Glows are becoming common in modern designs
	* Border-radius: Used very commonly
	* Layout:
		+ Rows of cards and Z-patterns are common
		+ Animations are common
		
### Personality #7: Playful/Fun

1. Overview:
	* Use colorful and round designs
	* Fueled by creative elements:
		+ Hand-drawn icons or illustrations
		+ Animations
		+ Fun language
2. Industries:
	* Child products
	* Animal products
	* Food
3. Webdesign ingredients:
	* Typography:
		+ Round and creative (handwritten)
		+ Uses sans-serif typefaces
		+ Centered text is common
	* Colors:
		+ Multiple colors are frequently used
		+ Colorful layouts are common
		+ Backgrounds and text can have multiple colors
	* Images:
		+ Frequently used
		+ Hand-drawn (3D) illustrations are common
		+ Geometric shapes and patterns are used
	* Icons:
		+ Frequently used
		+ Often hand-drawn
	* Shadows:
		+ Subtle shadows are common
		+ However,they are not always used
	* Border-radius: Very common
	* Layout:
		+ All kindsare used
		+ No particular tendencies
		
## The Missing Piece: Steal Like an Artist

1. Do not completely copy a design
	* Get inspired by websites you cisit
	* Take things you like and adapt them to your needs
2. Sources of inspiration
	* landbook.com
	* onepage