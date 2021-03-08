# summaraizing
 
### Domain modeling 
* Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.


#### Model epic fails videos
* Imagine you've been tasked to build a program that models the popularity of epic fail videos. After months of painstaking research, you've determined that the two essential metrics for gauging popularity are an epic rating and whether or not the video has animals.


#### Define a constructor and initialize properties
To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.


#### Generate random numbers
* To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.


#### Calculate daily Likes
* Popularity of a video is measured in Likes. And the formula for calculating Likes is the number of viewers times the percentage of viewers who'll Like a video. In other words, viewers times percentage.


#### Calculate weekly Likes
* In addition to modeling the daily Likes, your boss has asked you to model the weekly Likes too. Little does your boss know how easy it is to add behaviors to your domain model.


##### Here's some tips to follow when building your own domain models.
1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside.




## HTML

### Tables


#### What's a Table?
* A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.

#### Basic Table St ructure
* (table)
* (tr)
* (tf)
* (th)


#### Spanning Rows
* You may also need entries in a table to stretch down across more than one row.


#### Long Tables
* There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).


#### Old Code: Width & Spacing
* There are some outdated attributes which you should not use on new websites. You may, however, come across some of them when looking at older code, so I will mention them here. All of these attributes have been replaced by the use of CSS.


#### Old Code: Border & Background
* The border attribute was used on both the (table) and (td) elements to indicate the width of the border in pixels.




## JS


### functions,methods, and objects

#### CREATING OBJECTS USING CONSTRUCTOR SYNTAX
* On the right, an empty object called hote 1 is created using the constructor function.


#### CREATE & ACCESS OBJECTS CONSTRUCTOR NOTATION
* To get a better idea of why you might want to create mult iple objects on the same page, here is an example that shows room availability in two hotels.


#### ADDING AND REMOVING PROPERTIES
* Once you have created an object (using literal or constructor notation), you can add new properties to it.


#### RECAP: WAYS TO CREATE OBJECTS
* CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS 
* CREATING AN OBJECT WITH PROPERTIES & METHODS


#### THIS (IT IS A KEYWORD)
* The keyword this is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.


#### RECAP: STORING DATA 
* In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.




#### WHAT ARE BUILT-IN OBJECTS? 
* Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.


#### THE BROWSER OBJECT MODEL: THE WINDOW OBJECT
* The window object represents the current browser window or tab. It is the topmost object in the Browser Object Model, and it contains other objects that tell you about the browser.


#### USING THE BROWSER OBJECT MODEL
* Here, data about the browser is col lected from the window object and its children, stored in the msg variable, and shown in the page. The+= operator adds data onto the end of the msg variable 


#### THE DOCUMENT OBJECT MODEL: THE DOCUMENT OBJECT
* The topmost object in the Document Object Model (or DOM) is the document object. It represents the web page loaded into the current browser window or tab. You meet its child objects in Chapter 5.


#### USING THE DOCUMENT OBJECT
1. The details about the page are collected from properties of the document object.
2. You have seen the document object's get El ementByid () method in several examples so far. It selects an element from the page using the value of its id attribute. You will see this method in more depth on p195



#### GLOBAL OBJECTS: STRING OBJECT
* Whenever you have a value that is a string, you can use the properties and methods of the String object on that valu e. This example stores the phrase "Home sweet home " in a variable.


#### WORKING WITH STRINGS


#### DATA TYPES REVISITED 
* In JavaScript there are six data types: Five of them are described as simple (or primitive) data types. The sixth is the object (and is referred to as a complex data type).


#### GLOBAL OBJECTS: NUMBER OBJECT
* Whenever you have a value that is a number, you can use the methods and properties of the Number object on it.


#### WORKING WITH DECIMAL NUMBERS
* As with the String object the properties and methods of the Number object can be used with with any va lue that is a number.


#### GLOBAL OBJECTS: MATH OBJECT
* The Math object has properties and methods for mathematical constants and functions.



#### MATH OBJECT TO CREATE RANDOM NUMBERS
* The Math object's random() method generates a random number between 0 and 1 (with many decimal places)


#### GLOBAL OBJECTS: DATE OBJECT (AND TIME)
* Once you have created a Date object, the following methods let you set and retrieve the time and date that it represents.


