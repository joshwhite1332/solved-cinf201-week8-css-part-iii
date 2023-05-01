Download Link: https://assignmentchef.com/product/solved-cinf201-week8-css-part-iii
<br>
Last week, we learned about how we can use the box model along with other properties such as float to position items on our page. This week, we will go over those concepts again and learn a little more about how we can position our items and give them plenty of white space. By the end of this week, students will be able to position elements on a page using the float or flexbox properties.




<strong>Previous Participation Questions/Responses </strong>These are the participation questions from last week:

<u>https://forms.gle/rMaLpfDhz1gT7UgJ7</u>




This link has the responses to the fun question from last week. Feel free to look over the responses from myself and your peers.  <u>https://docs.google.com/spreadsheets/d/1QLoQzbO-</u>

<u>Er7ARIECl0aPvY1lKUyZTdYeuwsn4g0XEAk/edit?usp=sharing</u>




<h2>Midterm</h2>

You don’t need to have perfectly placed or finalized content. However, your pages should be mostly put together. Major headings should be used to describe content. If you haven’t thought of text to use, feel free to Google “Lorem Ipsum” for place holder text. You can also use place holder images by Googling those as well. The most important thing is that you have some sort of content placed for your Midterm.

The basic-page-example.html file provided earlier in the semester is a good an example of an acceptable page. Feel free to use some of the CSS I’ve provided (row class, float items to the left, give them a width) to help style your pages. The overall structure should be original and your own work though.

For the Midterm submission, you’ll submit 3 links in total. Each link should point to a different page of your midterm. When I check your work, I should be able to go from page to page easily by using links on your pages.




<strong>What’s Due? </strong>

<ul>

 <li>Participation Proof</li>

 <li>CSS Positioning Exercise 2 (CW/HW)</li>

</ul>

<h1>More Positioning with CSS (Lecture/Class Activity)</h1>

<h2>Box Model Review</h2>

The Box Model in CSS consists of three properties which are padding, border, and margin. The padding and margin properties are the most important of the three since they control the space of the elements on your page. Borders can improve aesthetics but most items on a page don’t have one. However, they might have some sort of default margin or padding added to them.

Everything in HTML is a box and so you must learn to think about your content in terms of boxes/containers which hold other boxes.

The <u>padding</u> property handles the space between the content and the border around that content.

The <u>border</u> property handles borders which wraps around the padding and content.

The <u>margin</u> property handles space outside of the border and wraps up the border, padding, and content.




In the image above, I have used Google Chrome’s “Inspect Element” feature (F12 or right-click and select it) to view the HTML/CSS in a page. On the left side of the inspector, the HTML structure is viewable. On the right side, there is a multi-colored box which depicts the CSS box model in action.

The orange area represents the margin (16px default for paragraphs in Chrome). The border is depicted by the yellow area. Lastly, the green area is the padding which separates the content from the border.

Positioning with CSS

Last week, we covered how to position our elements on the page using CSS. We will review the concepts again and then you will complete a second positioning exercise.

<u>Float Property</u>

This property takes content and aligns it to either the left or right side of a container. The content is removed from the normal document flow, but text content and inline elements will wrap around it. Block level elements will appear on the next available line.

It was intended originally for having text wrap around images but has been used to manipulate the positioning of elements on a page. The problem is that if the total width of items being floated is under 100%, other items below your floated ones may move up in that space and wrap around your content.

To prevent unwanted wrapping of content, you would have to clear your floats. This means you use the clear property on the element which wraps your floated elements. Unwanted wrapping would look something like the screenshot below.




In the image above, I have 2 divs with 40% width each floated to the left. Currently, they don’t have the clearfix code implemented and 0 margin to space them out. Since there is 20% of the width still available, content below these divs will try to fill that space. If you use the clearfix method appropriately, the content can have whatever widths you’d like, and content won’t move to its side as shown in the next image.




There are many methods to clear floats but the best one I have found is here:  <u>https://css-tricks.com/snippets/css/clear-fix/</u>

To use the clear fix in the link above, you need to wrap all floated elements in a parent container (div usually). Then you target that parent container’s before/after pseudo property and apply the styles as depicted. The before/after pseudo selectors allow us to add extra content to our HTML without using anything extra in the HTML markup. However, in our case, we don’t display any content (that’s why it has empty quotation marks). We display it like a table and clear both sides of it.




<u>Flexbox</u>

Flexbox is an awesome property which allows you to create layouts without using floats or positioning. Like floats, it requires the usage of a parent container which has other items/containers inside of it. Unlike floats, you don’t need to worry about clearing anything and it’s easier to implement. If we used the same HTML code as we did previously to create a 3column layout, the CSS would look like this instead:

Rather than using the row class for clearing, just simply give it a display of flex and a width of 100%. From there, we apply all the same styles to the children containers (one-third-column) with the exception of floating it. The final result would look pretty much the same, but with less effort as far as clearing floats and choosing float directions:

As a quick recap, for flexbox, you need a flex container and flex items. The flex container is just the parent container which wraps the elements you want to move around on the page. The flex items are the elements inside of the container which will be displayed horizontally or some other way.

For comparison purposes, I’ve provided a screenshot of the CSS we would use for the same layout, but by using float instead of flexbox. The underlying HTML is still the same.




Flexbox                                                                Float







The reason you would use float over flexbox is because float is more universally implemented by browsers. Some older browsers don’t support the flexbox property, and then your styles wouldn’t work as expected. It’s important to understand your audience and the types of devices/browsers they are using. For the purposes of this class, flexbox and floats are acceptable for assignments and the final project.




There are many other properties for the flex containers/items, so make sure to review them to fully understand the possibilities with flexbox. My example above is useful for creating quick multi-column layouts.




<u>Online Resources (Not required, but can be helpful for guidance)</u>

<ul>

 <li><u>https://css-tricks.com/almanac/properties/p/position/</u> (Position)</li>

 <li><u>https://developer.mozilla.org/en-US/docs/Web/CSS/float</u> (Float)</li>

 <li><u>https://css-tricks.com/all-about-floats/</u> (Float)</li>

 <li><u>https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox</u> (Flexbox)</li>

 <li><u>https://css-tricks.com/snippets/css/a-guide-to-flexbox/</u> (Flexbox)</li>

 <li><u>https://css-tricks.com/snippets/css/complete-guide-grid/</u> (Grid)</li>

 <li><u>https://www.w3schools.com/css/css_grid.asp</u> (Grid)</li>

</ul>




<h1>CSS Positioning Exercise 2 (CW/HW)</h1>

Download the “CSS-Positioning-Exercise-2.zip” folder from Blackboard under today’s Lecture Notes or the Assignment folder. Extract everything from inside of this zip folder to some place where you will be able to find them easily. This week, there will be an HTML file and an image with an example of a finished assignment. The HTML file contains &lt;style&gt;&lt;/style&gt; tags for you to use so you don’t have to place your CSS externally.




Based on the image provided, add CSS to the style tags so that the web page looks as close as possible to mine. You can change where it says “Your Name Here” to whatever name you want. In the image provided, it says “Chris Velez” in the header and “Christopher Velez” in the footer, but you can alter that to show your name.




It is also okay to change colors if the text contrast is high enough for the text to be readable.

However, the items should be styled similarly in terms of their placement, individual styles (borders, padding, margins, underlines, etc.)




<u>General Tips</u>

<ul>

 <li>If you use floats, float everything in one direction (I personally always use left)</li>

 <li>To center an image, use “display: block;” and “margin: 0 auto;” (images are always inline so when we display them with block, we can add width/height, margins, etc.)</li>

 <li>Padding/Margin will help with spacing (sometimes needs to be set to 0) o Use px or em (em is a relative unit and generally, 1em = one times whatever the default body font size is – sometimes 16px – 2em would then equal 32px)</li>

</ul>

o Margin: 0 auto also centers divs and other containers that have widths