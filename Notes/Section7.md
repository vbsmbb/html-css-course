# Section 7: Omnifood Project - Setup and Desktop Version

## Seven Steps of the Development Process

1. Define
2. Plan
3. Sketch
4. Design and Build
5. Test and Optimize
6. Launch
7. Maintain and Update

### Define the Project
1. Define WHO is the website for
	* Yourself?
	* Client or Agency?
	* Freelancing business?
2. Define WHAT the website is for
	* Is the purpose to provide information?
	* Is the pusrpose to sell product?
	* Is the purpose to entertain the user?
3. Goals example
	* Business goal: To sell premium dogfood
	* User goal: Find high-quality dog food at a good price
4. Define a target audience (be really specific)
	* Example: Women, 20 - 40 years old, making $2000/mo, living in the mid-west
	* The more specific your target audience, the more information you will have to meet your business and user goals

### Plan the Project
1. Plan and gather website content
	* Text
	* Images
	* Videos
	* Etc.
2. This content is usually provided by the client
	* You can help them find some free images
	* If they want you to write copy, charge them for it
	* For larger sites, plan the sitemap [content hierarchy]
		+ What pages the site needs
		+ How they relate to each other
	* Plan what SECTIONS each page needs to convey the content's message and the order of the sections
	* The content should guide the design of the project 
3. Define the website personality

### Sketch Layout and Component Ideas
1. Think about the components you need and how you can use them in layout patterns
2. Get ideas out of your head
	* Sketch them with ppen and paper
	* Or use a layout software like Figma
3. The sketches should be simple, low-fidelity, without details
4. This is an iterative process
	* Experiment with differnt components and layouts
	* This process will allow you to arrive at a first good solution
5. Do not take too much time at this point
	* You don't need to try to sketch everything
	* Don't try to make it perfect
	* Just get the design juices flowing
	
### Design and Build Website
1. Use the information from the first three steps to design and build the website using HTML and CSS
2. You have the layouts and components from the previous steps so now you need to design the visual styles
3. Create the design based on the actual website personality
4. Use the client's branding if possiblefor design decisions (website should match client's branding)
	* Colors
	* Typography
	* Icons
	
### Test and Optimize
1. Make sure website works well in all major browsers
	* Chrome
	* Firefox
	* Safari
	* Edge
2. Test the website on actual mobile devices not just developer tools
3. Optimize all images in terms of dimensions and file size
	* Use the correct dimensions in pixels
	* Compress them so they load quicker
4. Fix simple accessibility issues
	* Color contrast issues
	* Maybe adding gradients where needed
5. Run the Lighthouse performance test in Chrome Developer Tools and fix reported issues
6. Think about Search Engine Optimization (SEO)

### Launch
1. Upload website files to a hosting platform
	* Netlify has a free hosting plan
	* Other platforms have a variety of hosting options at different costs
2. Choose a great domain name
	* One that represents the brand well
	* One that is memorable
	* One that is easy to write
	
### Maintain and Update the Website
1. Keep the website content updated over time
	* If working with a client, create a monthly maintenance contract (recurring income)
2. Install some type of analytics software
	* Google Analytics
	* Fathom
3. The analytics gives you information about how the users interact with your website
	* This may lead to changes in site structure and content
	* This can lead to updates that help the users make more action decisions
4. Each website should have a blog
	* It should be updated regularly
	* It is a good way to keep users coming back
	* It also aids SEO (?)
	
## Defining and Planning the Omnifood Project

### Define the Project
1. Define WHO the project is for: A client (Omnifood)
2. Define WHAT the website is for
	* Business goal: Sell a food subscription
	* User goal: Eat well effortlessly without spending a lot of time or money
3. Define target audience
	* Busy people who like technology
	* Are interested in eating healthy
	* Have a good-paying job
	
### Plan and gather website content
1. Plan the sitemap
	* No sitemap necessary
	* Omnifood will be a one-page marketing website
	* This is basically a landing page
2. Define the website personality
	* Use the startup/upbeat personality
		+ Technology company first
		+ Technology-centered target audience
	* Add some elements of the calm/peaceful personality
		+ Dealing with user well-being
		+ Concerned with user health

### Plan page sections
1. This should come from the content
2. Sections
	* Logo + Navigation
	* Hero (Include Summary and Headline)
	* Featured in
	* How it works
	* Meals and list of Diets
	* Testimonials + Gallery (side-by-side)
	* Pricing + Features
	* Call-To-Action (CTA)
	* Footer
	
## Sketching Initial Layout Ideas

## Responsive Design Principles

### Responsive Design
1. A design technique to make a webpage adjust its layout and visual style to any possible screen size
2. Responsive design makes all websites usable on all devices:
	* Desktop computers
	* Tablets
	* Mobile phones
3. Responsize webdesign is NOT a separate technology; it's just CSS

### Responsive Design Ingredients
1. Fluid layouts
	* Allows webpage to adapt to current viewport width
	* Use %, not px, for elements that should adapt to the viewport
	* Use max-width instead of width
2. Responsive Units
	* Use REM instead of PX for most lengths
	* This makes it easy to scale the entire unit up or down automatically
	* Use 1rem = 10px
3. Flexible Images
	* By default, images do not scale automatically as we change the viewport
	* Always use % for image dimensions together with the MAX-WIDTH property
4. Media queries
	* Bring responsive sites to life
	* Allow us to change CSS styles on certain viewport widths (called breakpoints)
	
### Desktop-First VS. Mobile-First Development
1. Desktop-First
	* Start writing CSS for desktop [large sreen]
	* Then, write media queries to shrink design to smaller screens
	* This method is thought to be the easiest to learn
2. Mobile-First
	* Start writing CSS for small screens
	* Then, write media queries to expand design for large screens
	* Forces us to reduce websites and apps to the absolute essentials
	
## How REM and MAX-WIDTH Work
1. Max-Width
	* Sets the maximum width of an element, but not the minimum
	* Using max-width allows an element to scale smaller, but can never be larger than the max-width set
2. REM
	* A rem is the size of the font of the root element
		+ The root element is the HTML element
		+ If no font size is set, it is the default font size of the browser
		+ Most browsers default font size is 16 pixels
		+ Therefore, unless the font size of the HTML element is set or the browser default font size has been changed, the size of 1rem = 16px.
		+ Normally 50rem = 800px.
	* For easier REM to PIXEL calculations, set the REM to 10 pixels
		+ You can set it directlysetting the font-size to 10 pixels in teh HTML (root) tag
		+ However, this may cause the user issues if they want to change the default pixel size in their browser
		+ Therefore, set the font-size to be 62.5%
		+ 10/16*100 = 62.5%
		+ Now if the user changes the default pixel settings on the web page will change accordingly

