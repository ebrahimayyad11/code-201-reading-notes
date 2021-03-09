# Summaraizing

## HTML

#### Forms
* Traditionally, the term 'form' has referred to a printed document that contains spaces for you to fill in information.


##### Why forms
* The best known form on the web is probably the search box that sits right in the middle of Google's homepage.


##### Form controls
* There are several types of form controls that you can use to collect information from visitors to your site.


##### Adding text:
* Text input: used for a single line of text such as email addressess and names.
* Password input: like a single line text bot but it masks the characters entered.
* Text area(multi line): for longer of text, such as messages and comments.


##### Making choices:
* Radio buttons: for use when must sekect one of a number of options.
* Checkboxes: when a user select and unselect one ot more options.
* Drop-down boxes: when a user must pick one of number of options from list.



##### Submiting forms:
* Submit buttons: to submit data from your form to another web page.
* Images buttons: similar to submit buttons but they allow you to use an image.


##### Uploading files:
* file upload: allows you to upload files (eg:images) to a website.


##### How forms work
* A user fills in a form and then presses a button to submit the information to the server.


##### Form structure 
* we use this for is : (form).
* it has two main attributes: 1. action 2. method



##### Test input 
* we use for it : (input).
* it has two main attributes : 1. type 2. name


###### Password input
* we use for it (input) with attribut (type="password").


###### Text area
* we use for it (textarea).


###### Radio buttons
* we use for it (input) with attribut (type="radio") and (value="the name that will apear for the radio").


###### Checkbox
* we use for it (input) with attribut (type="checkbox") and (value="the name that will apear for the checkbox").



###### Drop down list box
* we use for it (select) and we use an elememt inside the select element called (option) and it has an attribute value and selected.



###### File input cox
* we use for it (input) with attribut (type="file"). 


###### Image button
* we use for it (input) with attribut (type="image").

###### button and hidden controls
* button: The (button) element was introduced to allow users more control over how their buttons appear, and to allow other elements to appear inside the button.
* type="hidden" This example also shows a hidden form control.


###### Labelling Form Controls
* (label) When introducing form controls, the code was kept simple by indicating the purpose of each one in text next to it.
* (for): The for attribute states which form control  the label belongs to.Note how the radio buttons usethe id attribute.


###### Grouping Form Elements
* (fieldset) You can group related form controls together inside the (fieldset) element.
* (legend) The (legend) element can come directly after the opening (fieldset) tag and contains a caption which helps identify the purpose of that group of form controls.


##### HTML 5: Form Validation
* You have probably seen forms on the web that give users messages if the form control has not been filled in correctly; this is known as form validation.


##### HTML 5: Date Input
* we use for it (input) with attribut (type="date").


##### HTML 5: Email & URL Input
* email: we use for it (input) with attribut (type="email").
* URL: we use for it (input) with attribut (type="url").


##### HTML 5: Search Input
* we use for it (input) with attribut (type="search").


###### Placeholder
* On any text input, you can also use an attribute called placeholder whose value is text that will be shown in the text box until the user clicks in that area. Older browsers simply ignore this attribute.



## CSS


### Lists Tables and Forms


##### Bullet point styles
* The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker).


##### Images for Bullets
* You can specify an image to act as a bullet point using the list-style-image property.


##### Positioning the Marker
* Lists are indented into the page by default and the list-styleposition property indicates whether the marker should appear on the inside or the outside of the box containing the main points.
* and it has two values: 1. outside  2. inside


##### List shorthand
* As with several of the other CSS properties, there is a property that acts as a shorthand for list styles. It is called list-style, and it allows you to express the markers' style, image and position properties in any order.


#### Tables properties
* You have already met several properties that are commonly used with tables. Here we will put them together in a single example using the following:
1. width.
2. padding.
3. text-trasform.
4. letter-spacing, fornt size.
5. border-top, border-bottom.
6. text-align.
7. background-color.
8. :hover.


##### Border on empty cells
* If you have empty cells in your table, then you can use the empty-cells property to specify whether or not their borders should be shown.
* it has 3 values: 1. show 2. hide. 3. inhirit.


##### Gaps between cells
* The border-spacing property allows you to control the distance between adjacent cells. By default, browsers often leave a small gap between each table cell, so if you want to increase or decrease this space then the border-spacing property allows you to control the gap.
* it has 2 values: 1. collapse 2. separate


#### Styling Forms

##### the most common to style:
* text inputs and text areas.
* submit buttons.
* labels om forms, to get the form control to align nicely.


##### Styling text input we can use to style it :
* font size.
* color.
* background-color.
* border.
* border-radius.
* :focus.
* :hover.
* bacground-image.



##### Styling submit buttons we can use to style it:
* color.
* text-shadow.
* border-bottom.
* background-color.
* :hover.


##### Styling firldsets and legends we use to style it:
* width.
* color.
* backgournd-color.
* border.
* border-radius.
* padding.



##### aligning form controls: problem
* Labels for form elements are often different lengths, which  means that the form controls will not appear in a straight line. This is demonstrated in the example on the right (without CSS applied to the form controls).


##### aligning form controls: solution
* Each row of the form has a title telling users what they need to enter. For the text inputs, the title is in the (label) element. For the radio buttons, the title is in a (span) element. Both have a class attribute with a value of title.


##### Cu rsor Styles
* The cursor property allows you to control the type of mouse cursor that should be displayed to users.
* the values for it:
1. auto.
2. crossshair.
3. pointer.
4. move.
5. text.
6. wait.
7. help.
8. url("curser.gif");


##### Web developer toolbar
* This helpful extension for Firefox and Chrome provides tools to show you the CSS styles that apply to an element when you hover over it, along with the structure of the HTML.



## JS

### Events


#### Events types
* UI Events.
* Keyboard Events.
* Mouse Events.
* Focus Events.
* Form Events.
* Mutation Events.


#### How Events Trigger Jacascript Code?
* When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.
1. Select t he element node(s) you want the script to respond to.
2. Indicate which event on the selected node(s) will trigger the response.
3. State the code you want to run when the event occurs.



#### THREE WAYS TO BIND AN EVENT TO AN ELEM ENT:
* Event handlers let you indicate which event you are waiting for on any particular element. There are three types of event handlers.
1. HTML EVENT HANDLERS
2. TRADITIONAL DOM EVENT HANDLERS
3. DOM LEVEL 2 EVENTLISTENERS 


#### TRADITIONAL DOM EVENT HANDLERS
* All modern browsers understand this way of creating an event handler, but you can only attach one function to each event handler.


#### USING DOM EVENT HANDLERS
1. If you use a named function when the event fires on your chosen DOM node, write that function first. (You could also use an anonymous function.)
2. The DOM element node is stored in a variable. Here the text input (whose id attribute has a va lue of username) is placed into a variable called e 1 Username.


#### Event listers
* Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.


#### USING EVENT LISTENERS
1. If you use a named function when the event fi res on your chosen DOM node, write that function first. (You could also use an anonymous function.)
2. The DOM element node(s) is stored in a variable. Here the text input (whose id attribute has a value of username) is placed into a variable called el Username.


#### USING PARAMETERS WITH EVENT HANDLERS & LISTENERS
* Because you cannot have parentheses after the funct ion names in event handlers or listeners,passing arguments requires a workaround.


#### USING PARAMETERS WITH EVENT LISTENERS
* The first line of this example shows the updated checkUsername() function. The mi nlength parameter specifies the minimum number of characters that the username should be. JAVASCRIPT
* The value that is passed into the checkUsername() function is used in the conditional statement to check if the name is long enough, and provide feedback if the username name is too short.
c06/ js/ event-li st ener -with-parameters.js
var elUsername = document .getElementByid('username') ;
var elMsg = document .getElementByid('feedback') ;
II Get username i nput
II Get feedback element
function checkUsername(mi nleng t h) { II Declare function
if (elUsername.val ue.length < minlength) II If username too short
II Set the error message
elMsg . textContent = 'Username must be ' + minlength + ' characters or more';
} else { II Otherwi se
elMsg . innerHTML
}
I I ,• II Clear msg
elUsername. addEventListener( 'bl ur ' , function() {
checkUsername (S);
II When it loses focus
II Pass arguments here
}, false) ; 


#### SUPPORTING OLDER VERSIONS OF IE 
* IES-8 had a different event model and did not support addEventL i stener() but you can provide fallback code to make event listeners work with older versions of IE.


#### FALLBACK FOR USINGEVENT LISTENERS IN I E8 
* The event handling code builds on the last example, but it is a lot longer this time because it contains the fal lback for Internet Explorer 5-8.


#### Event flow
* HTML elements nest inside other elements. if you hover or click on a link, you will also be hovering or clicking on its parent elements.


##### Why flow matters?
* The flow of events only really matters when your code has event handlers on an element and one of its ancestor or descendant elements.


#### THE EVENT OBJECT
* When an event occurs, the event object tells you information about the event, and the element it happened upon.


#### THE EVENT OBJECT IN IES-8
* Below you can see how you get the event object in IES-8. It is not passed automatically to event handler/listener functions; but it is available as a child of the window object.


#### USING EVENT LISTENERS WITH THE EVENT OBJECT
* Here is the example that has been used throughout
the chapter so far with some modifications:
1. The function is called check Length() rather than
checkUsername (). It can be used on any text input.
2. The event object is passed to the event listener.
The code includes fallbacks for IES-8(Chapter13
demonstrates using helper functions to do this).
3. In order to determine which element the user
was interacting with, the function uses the event
object's target property (and for IES-8 it uses the
equivalent s rcEl ement property).
JAVASCRIPT
function checklength(e, minlength) {
var el , elMsg ;
if (le) {
e = window.event;
}
el = e .target II e.srcElement;
elMsg =el .nextSibling;
if (el . va l ue .length< minlength)
elMsg . innerHTML 'Username must be '
else {
elMsg . innerHTML ' ';
* This function is now far more flexible than the
previous code you have seen in this chapter because:
1. It can be used to check the length of any text
input so long as that input is directly followed by an
empty element that can hold a feedback message
for the user. (There should not be space or carriage
returns between the two elements; otherwise, some
browsers might return a whitespace node.)
2. The code will work with IES-8 because it tests
whether the browser supports the latest features (or
whether it needs to fall back to use older techniques).
c06/ js/ event-1istener-with-event-object.js
II Declare function
II Declare variables
II If event object doesn't exist
II Use IE fallback
II Get target of event
II Get its next sibling
II If length is too short set msg
c + minlength + ' cha racters or more';
II Otherwise
II Clear message
var el Username = document .getEl ementByid('username ' );ll Get username input
if (el Username .addEventlistener) { II If event listener supported
elUsername.addEventlistener ('b l ur ', function(e) { II On blur event
checkUsername(e, 5); II Call checkUsername()
}, false); II Capture in bubble phase
else { II Otherwise
elUsername . attachEvent('onblur', function(e){ II IE fallback onblur
checkUsername(e, 5); II Call checkUsername()
} ) ;



#### EVENT DELEGATION
* Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.


#### CHANGING DEFAULT BEHAVIOR
* The event object has methods that change: the default behavior of an element and how the element's ancestors respond to the event.


#### WHICH ELEMENT DID AN EVENT OCCUR ON?
* When calling a function, the event object's target property is the best way to determine which element the event occurred on. But you may see the approach below used; it relies on the this keyword.


#### DIFFERENT TYPES OF EVENTS
* In the rest of the chapter, you learn about the different types of events you can respond to.

##### Events are defined in:
1. The W3C DOM specification
2. The HTMLS specification
3. In Browser Object Models


#### USER INTERFACE EVENTS 
* User interface CUI) events occur as a result of interaction with the browser window rather than the HTML page contained within it, e.g., a page having loaded or the browser window being resized.


##### events triggers:
1. load.
2. unload.
3. error.
4. resize.
5. scroll.


##### load
* The load event is commonly used to trigger scripts that access the contents of the page.


##### focus and blur events
* The focus and b 1 ur events are most commonly used on forms. They can be particularly helpful when:
* You want to show tips or feedback to users as they interact with an individual element within a form (the tips are usually shown in other elements and not the one they are interacting with) 
* You need to trigger form validation as a user moves from one control to the next (rather than waiting for them to submit the entire form first)




#### mouse events
* The mouse events are fired when the mouse is moved and also when its buttons are clicked.
* there is some events that we can use it for the mouse:
1. click
2. dbclick
3. mousedown
4. mouseup
5. mouseover
6. mouseout
7. mousemove


#### Where events occur
* The event object can tell you where the cursor was positioned when an event was triggered.


#### Keyboard events
* The keyboard events are fired when a user interacts with the keyboard (they fire on any kind of device with a keyboard).
* there is some events that we can use it for the keyboard:
1. input
2. keydown
3. keypress
4. keyup


#### Form events
* There are two events that are commonly used with forms. In particular you are likely to see submit used in form validation.
* there is some events that we can use it for the Forms:
1. submit
2. change
3. input


#### Mutation events and observers
* Whenever elements are added to or removed from the DOM, its structure changes. This change triggers a mutation event.
* there is some events that we can use it for the mutation:
1. DOMNodelnserted
2. DOMNodeRemoved
3. DOMSubtreeModified
4. DOMNodelnsertedlntoDocument
5. DOMNodeRemovedFromDocument


#### HTML5 events
* Here are three page-level events that have been included in versions of the HTMLS spec that have become popular very quickly.
* there is some events that we can use it for the HTML5:
1. DOMContentLoaded
2. hashchange
3. beforeun load
