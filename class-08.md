# summarizing

## Layout
* control where each element sits on a page



##### Building blocks
* CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
* Block-level elements: start on a new line.
* Inline elements: flow in between surrounding text.


##### containing elements
* If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.


##### controlling the position of elements
* CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS.


##### we can float elements using float property:
1. normal flow: postition:static.
2. realtive positioning: postition:relative .
3. absolute positioning: postition:absolute .
3. fixed positioning: postition:ficed .




##### Box offset
* to indicate where a box should be positioned
* the values that we use for it:
1. fixed positioning 
2. floating positioning


##### floating elements
* we can use this by this attribute : float

##### z-index
* When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.


##### using float to place elements side-by-side
* A lot of layouts place boxes next to each other. The float property is commonly used to achieve this.


##### clearing floats
* The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:
* to use it we use this attribute: clear
* and we use this values in it: left,right,both,none


##### parents of floated elements:problem
* If a containing element only contains floated elements, some browsers will treat it as if it is zero pixels tall.


##### parents of floated elements:solution
* Traditionally, developers got around this problem by adding an extra element after the last floated box (insid e thecontaining element).


##### creating multi-coulmn layouts with floats
* Many web pages use multiple columns in their design. This is achieved by using a (div) element to represent each column.
* we use these attributes in it: width,float,margin


##### screen size
* Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.


##### screen resolution
* Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.


##### page sizes
* Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).


##### fixed width layout
* Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.
* advantages:
1. Pixel values are accurate at controlling size and positioning of elements.
2. The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
3. You can control the lengths of lines of text regardless of the size of the user's window.
4. The size of an image will always remain the same relative to the rest of the page.
* disadvantages:
1. You can end up with big gaps around the edge of a page.
2. If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
3. If a user increases font sizes, text might not fit into the allotted spaces.
4. The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.
5. The page will often take up more vertical space than a liquid layout with the same content.


##### liquid layout
* Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.
* advantages:
1. Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.
2. If the user has a small window, the page can contract to fit it without the user having to scroll to the side.
3. The design is tolerant of users setting font sizes larger than the designer intended (because the page can stretch).
* disadvantages:
1. If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.
2. If the user has a wide window, lines of text can become very long, which makes them harder to read.
3. If the user has a very narrow window, words may be squashed and you can end up with few words on each line.
4. If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the window smaller) the image can overflow over the text.


##### a fixed width layout
* To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too).


##### a liquid layout
* The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen.


##### layout grid
* Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page. Many designers use a grid structure to help them position items on a page, and the same is true for web designers.


##### CSS framework
* CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.
* advantages:
1. They save you from repeatedly writing code for the same tasks.
2. They will have been tested across different browser versions (which helps avoid browser bugs).
* disadvanatges:
1. They often require that you use class names in your HTML code that only control the presentation of the page (rather than describe its content).
2. In order to satisfy a wide variety of needs, they often contain more code than you need for your particular web page (commonly referred to as code “bloat”).


##### multiple style sheets
* we use for it : @import and link
* Some web page authors split up their CSS style rules into separate style sheets. For example, they might use one style sheet to control the layout and another to control fonts, colors and so on.


