# Summarizing

## HTML

#### Lists
* There are lots of occasions when we need to use lists. HTML provides us with three different types


##### Ordered lists
* The ordered list is created with the (ol) element.
* Each item in the list is placed between an opening (li) tag and a closing (li) tag. (The li stands for list item.)


##### Unordred lists
* The unordered list is created with the (ul) element.
* Each item in the list is placed between an opening (li) tag and a closing (li) tag. (The li stands for list item.)


##### Definition lists 
* The definition list is created with the (dl) element and usually consists of a series of terms and their definitions.
* (dt) This is used to contain the term being defined (the definition term).
* (dd) This is used to contain the definition.


##### Nested lists
* You can put a second list inside an (li) element to create a sublist or nested list.



## CSS

#### Boxes


##### Box Dimensions
* for this we use the width and the height attributes


##### limiting width
* for this we use min-width and max-width attributes


##### limiting height
* for this we use min-height and max height attributes


##### Overflowing content
* for this we use overflow attribute and the values :
1. hidden
2. scroll


##### Border, Margin and Padding 
* Every box has three available properties that can be adjusted to control its appearance:

###### Border
* The border separates the edge of one box from another.

###### Margin
* Margins sit outside the edge of the border.

###### Padding
* Padding is the space between the border of a box and any content contained within it.



##### Changing Inline/Block
* for this we use Display and values of it:
1. inline
2. block
3. inline-block
4. none


##### Hidding Boxes 
* for this we use visibility and the values of it:
1. hidden
2. visible


##### Border images
* for this we use border-image and the main attribute for it is (url:and we give it the url of the image as a value).


##### Box Shadows
* for this we use box-shadow attribute.


##### rounded corners
* for this we use border-radius attribute.


##### Elliptical shapes
* for this we use border-radius attribute.



## Javascript


#### Arrays 
* An array is a special type of variable. It doesn't just store one value; it stores a list of values.


##### creating an array
* You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array).
* example: var color = ['white', 'black', 'custom'];


##### Values in arrays
* Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).


##### Accessing and Changing values in an array
* var color = ['red', 'yellow', 'blue'];
* var red = color[0];
* color [2] = 'green';


#### If statement
* The if statement evaluates (or checks) a condition, if the condition evaluates to ture, any statements in the subsequent code block are exuted.

##### IF Else Statement
* The if...else statement checks a condition if it resolve to true the first block is executed, if the condition resolves to false the second code block is run instead.


#### Switch Statement
* A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.
* example: var i = 2;
* switch (i){
* case 1 : i++;   breake;
* case 2 : i = i/2;  breake;
* defult : i = 0;  breake;
* }


##### Type coercion and weak typing
* If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error.


##### Truthy and Falsy values
* Due to type coercion, every value in JavaScript can be treated as if it were true or false; and this has some interesting side effects.


##### Checking Quality and Existence
* Because the presence of an object or array can be considered truthy, it is often used to check for the existence of an element within a page.


##### Short Circuit Vlaues
* Logical operators are processed left to right. They short-circuit (stop) as soon as they have a result - but they return the value that stopped the processing (not necessarily true or false).


#### loops
* loops check condition if it return true the code block will run then the condition will be checked again and if it still return true the code block will run again it repeats until the condition return false.

##### there are three common types of loops:
1. for.
2. while.
3. do while.

##### loop counters:
1. intialization : var i = 0;
2. condition : i < 10;
3. update : i++;

##### using for loop
* A for loop is often used to loop through the items in an array. 


##### using while loop
* This loop will continue to run for as long as the condition in the parentheses is true. That condition is a counter indicating that, as long as the variable i remains less than 10, the statements in the subsequent code block should run. 


##### using do while loop
* The key difference between a while loop and a do while loop is that the statements in the code block come before the condition. This means that those statements are run once whether or not the condition is met.

