# summaraizing

## Understanding The Problem Domain Is The Hardest Part Of Programming

#### What is the hardest thing about writing code?
* Learning a new technology
* Naming things
* Testing your code
* Debugging
* Fixing bugs
* Making software maintainable

#### Why problem domains are hard?
* Have you ever tried to put together a jigsaw puzzle that didn’t have any picture on it?  How about one like this one, that has a very similar pattern repeated on it and is double-sided?
![puzzel photo](https://spzone-simpleprogrammer.netdna-ssl.com/wp-content/uploads/2013/07/81zQGlKs9oS._SL1500_.jpg)


##### The reason why puzzles like this one are so hard, is because you can’t really see what you are trying to build very clearly.  Normally when you put together a jigsaw puzzle you follow steps that might look something like this:
1. Figure out what the major components of the picture are
2. Sort the pieces by color or component
3. Put together all the border pieces
4. Put together each component of the picture from the piles you created


##### Programming is easy if you understand the problem domain


####  the problem is the most critical piece to the equation. It is very difficult to solve a problem before you know the question.  It’s like buzzing in on Jeopardy before you hear the clue and shouting out random questions
* What can you do about it?
1. Make the problem domain easier
2. Get better at understanding the problem domain


##### You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.


## JS

#### object

##### whats is an object?
* Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

##### craeting an pbject: literal notation
* Literal notation is the easiest and most popular way to create objects (there are several ways to create objects).
* example: var hotel = {
*  name : 'Quay',
*  rooms : 40 ,
*  booked : 25 , 
*  checkAvailability: function() {
*  return this.room - this.booked;
* }
* };


##### Accessing an object and dot notation
* you access the properties or methods of an object using dot notation.
* you can also access properties using square brackets.
* var hotelName = hotel.name;
* var roomsFree = hotel.checkAvailability();



#### Document object model
* The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
* THE DOM TREE IS A MODEL OF A WEB PAGE


##### WORKING WITH THE DOM TREE
* Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.(ACCESS THE ELEMENTS)
2. Use its text content, child elements, and attributes.(WORK WITH THOSE ELEMENTS)


##### caching DOM queries
* methods that find elements in the DOM tree calles DOM queries, when you need to work with an element more than once, you should use a variable to store the result of this query.


##### ACCESSING ELEMENTS
* DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.


##### methods that select individual elements
* getElementById() and querySelector() can both swarch an entire document and return individual elements. both use a similar syntax.
* example : document.getElementById('one');



##### NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT
* When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element).


##### selecting an element from a nodelist
* there are two ways to select an element from nodelist:
* item() method and array ayntax.
* both reqire the index number of the element you want.


##### selecting elements using class attributes
* The get El ementsByCl ass Name() method allows you to select elements whose c 1 ass attribute contains a specific value.


##### SELECTING ELEMENTS BY TAG NAME
* The get El ementsByTagName () method allows you to select elements using their tag name


##### SELECTING ELEMENTS USING CSS SELECTORS
* querySe 1 ector() returns the first element node that matches the CSS-style selector. querySe 1ectorA11 () returns a Nodelist of all of the matches.


##### reoeating actions for an entire nodelist
* when you have a nodelist, you can loop through each mode in the collection and apply the same statement to each.


##### LOOPING THROUGH A NODELIST
* If you want to apply the same code to numerous elements, looping through a Nodelist is a powerful technique.


##### TRAVERSING THE DOM 
* When you have an element node, you can select another element in relation to it using these five properties. This is known as traversing the DOM.


##### WHITESPACE NODES
* Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements


##### PREVIOUS & NEXT SIBLING
* You have just seen that these properties can return inconsistent results in different browsers. However, it is safe to use them when there is no whitespace between elements.


##### FlRST & LAST CHILD
* These properties also return inconsistent resu lts if there is whitespace between elements. 


##### HOW TO GET/UPDATE ELEMENT CONTENT
* So far this chapter has focused on finding elements in the DOM tree. The rest of this chapter shows how to access/update element content. Your choice of techniques depends upon what the element contains.


##### ACCESS & UPDATE A TEXT NODE WITH NODEVALUE
* When you select a text node, you can retrieve or amend the content of it using the node Va 1 ue property.


##### ACCESSING & CHANGING A TEXT NODE
* To work with text in an element, first the element node is accessed and then its text node.


##### ACCESS & UPDATE TEXT WITH TEXTCONTENT (& INN ERTEXT) 
* The textCon tent property allows you to collect or update just the text that is in the containing element (and its children).


##### ACCESSING TEXT ONLY
* In order to demonstrate the difference between textContent and i nnerText, this example features a CSS rule to hide the contents of the (em) element



##### ACCESS & UPDATE TEXT & MARKUP WITH INNERHTML
* Using the i nnerHTML property, you can access and amend the contents of an element, including any child elements.



##### UPDATE TEXT & MARKUP
* This example starts by storing the first list item in a variable called fi rstltem.


##### ADDING ELEMENTS USING DOM MANIPULATION
* DOM manipulation offers another technique to add new content to a page (rather than i nnerHTML). It involves three steps:
1. CREATE THE ELEMENT
2. GIVE IT CONTENT 
3. ADD IT TO THE DOM


##### ADDING AN ELEMENT TO THE DOM TREE
* createEl ement () creates an element that can be added to the DOM tree, in this case an empty (li) element for the list.



##### REMOVING ELEMENTS VIA DOM MANIPULATION
* DOM manipulation can be used to remove elements from the DOM tree.


##### REMOVING AN ELEMENT FROM THE DOM TREE
* This example uses the removeCh i 1 d () method to remove the fourth item from the list (along with its contents).



##### COMPARING TECHNIQUES: UPDATING HTML CONTENT
* So far, you have seen three techniques for adding HTML to a web page. It's time to compare when you should use each one.


##### CROSS-SITE SCRIPTING (XSS) ATTACKS
* If you add HTML to a page using i nnerHTML (or several jQuery methods), you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise, an attacker could gain access to your users' accounts


##### DEFENDING AGAINST CROSS-SITE SCRIPTING
* VALIDATE INPUT GOING TO THE SERVER
1. Only let visitors input the kind of characters they need to when supplying information.
2. Double-check validation on the server before displaying user content/storing it in a database.
3. The database may safely contain markup and script from trusted sources (e.g., your content management system).


##### XSS: VALIDATION & TEMPLATES
* Make sure that your users can only input characters they need to use and limit where this content will be shown on the page.


##### XSS: ESCAPING & CONTROLLING MARKUP
* Any content generated by users that contain characters that are used in code should be escaped on the server. You must control any markup added to the page.


##### CHECK FOR AN ATTRIBUTE AND GET ITS VALUES
* Before you work with an attribute, it is good practice to check whether it exists. This will save resources if the attribute cannot be found.


##### CREATING ATTRIBUTES & CHANGING THEIR VALUES
* The cl assName property allows you to change the value of the cl ass attribute. If the attribute does not exist, it will be created and given the specified value.


##### REMOVING ATTRIBUTES
* To remove an attribute from an element, first select the element, then call removeAtt r i bute () . It has one parameter: the name of the attribute to remove.



