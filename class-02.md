# summarizing

## HTML 
* When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.

#### Structural markup
* the elements that you can use to describe both headings and paragraphs.


#### Semantic markup
* which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on.


#### Headings 
1. (h1)
2. (h2)
3. (h3)
4. (h4)
5. (h5)
6. (h6)


#### Paragraphs
* (p)


#### Bold and Italic
1. for Bold we use (b)
2. for Italic we use (i)


#### Superscript and Subscript
1. for supscript we use (sup)
2. for subscript we use (sub)


#### white space
* When the browser comes across two or more spaces next to each other, it only displays one space. Similarly if it comes across a line break, it treats that as a single space too. This is known as white space collapsing.


#### Line Breaks and Horizantal Rules
1. for Line Breaks we use (br)
2. for Horizantal Rules we use (br)


#### Visual Editors & Their Code views
* Content management systems and HTML editors such as Dreamweaver usually have two views of the page you are creating: a visual editor and a code view.


#### Semantic Markup:
There are some text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages — they are known as semantic markup.


#### Strong and Emphasis
1. for strong we use (strong)
2. for emphasis we use (em)


#### Quotations 
1. (blockquote)
2. (q)


#### Abbreviations and Acronyms
* (abbr)


#### Citations and Definitions
1. for Citations we use (cite)
2. for Definitions we use (dfn)


#### Author Details
* (address)


#### Changes to Content
1. for inserted we use (ins)
* can be used to show content that has been inserted into a document.
2. for deleted we use (del)
* can show text that has been deleted from it.
3. (s)
* it indicates something that is no longer accurate or relevant (but that should not be deleted).



## CSS
* it make our web pages more attractive, controlling the design.


#### Understanding CSS: Thinking Insi de the Box
* The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element.


#### Block and Inline Elements
1. Block level elements 
* look like they start on a new line. Examples include the <h1>- <h6>, <p> and <div> elements.
2. Inline elements
* flow within the text and do not start on a new line. Examples include <b>, <i>, <img>, <em> and <span>.


#### CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.


#### CSS Associates Style rules with HTML elements.
* CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.


##### Selectors
* indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.


##### Declarations
* indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.


#### CSS Properties Affect How El ements Are Dis played 
* CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.


##### Properties
* indicate the aspects of the element you want to change. For example, color, font, width, height and border.


##### Values 
* specify the settings you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want the text in these elements to be.



#### Using External CSS
* we link the CSS sheet with the HTML page using <link> tag


##### <link>
* it includes 3 main attributes: 
1. href: This specifies the path to the CSS file (which is often placed in a folder called css or styles).
2. type: This attribute specifies the type of document being linked to. The value should be text/css.
3. rel: This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.


#### Using Internal CSS
* You can also include CSS rules within an HTML page by placing them inside a <style> element, which usually sits inside the <head> element of the page.
* The <style> element should use the type attribute to indicate that the styles are specified in CSS. The value should be text/ css.


#### CSS Selectors
* There are many different types of CSS selector that allow you to target rules to specific elements in an HTML document.
1. Universal Selector: Applies to all elements in the document, example:( * {} ).
2. Type Selector: Matches element names, example:( h1, h2, h3 {} ).
3. Class Selector: Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol, example: ( .note {} , p.note {} ).
4. ID Selector: Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol, example: ( #introduction {} ).
5. Child Selector: Matches an element that is a direct child of another, example: ( li>a {} ).
6. Descendant Selector: Matches an element that is a descendent of another specified element (not just a direct child of that element), example: ( p a {} ).
7. Adjacent Sibling Selector: Matches an element that is the
next sibling of another, example ( h1+p {} ).
8. General Sibling Selector: Matches an element that is a sibling of another, although it does not have to be the directly preceding element, example: ( h1-p {} ).



#### How CSS rules CASCADE
1. Last rule: If the two selectors are identical, the latter of the two will take precedence.
2. SPECIFICITY: If one selector is more specific than the others, the more specific rule will take precedence over more general ones.
3. Important: You can add !important after any property value to indicate that it should be considered more important than other rules that apply to the same element.



#### Why use External Style Sheets?
* When building a website there are several advantages to placing your CSS rules in a separate style sheet.
1. All of your web pages can share the same style sheet. This is achieved by using the <link> element on each HTML page of your site to link to the same CSS document.
2. once the user has downloaded the CSS stylesheet, the rest of the site will load faster.
3. The HTML code will be easier to read and edit because it does not have lots of CSS rules in the same document.



#### Different Versions od CSS and Browser Quirks
* CSS1 was released in 1996 and CSS2 followed two years later. Work on CSS3 has been ongoing but the major browsers have already started to implement it.



## JAVASCRIPT

#### statments 
* A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.


#### comments 
* You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.
* There is to type of comments:
1. one line comment and we is this to write is //
2. multiple line comment and we start it with <!-- and close is with -->


#### What is a variable
* A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.


#### How to declare variables
* example: var quantity;
* var is the variable keyword.
* quantity is the variable name.


#### How to assign variables a value
* example: quantity = 3;
* quantity is the variable name.
* 3 is the variable value.


#### The data types
1. Numeric data type: it contains numbers.
2. String data type: it contains letters and other characters.
3. Boolean data type: it contains True and Flase.


#### When want to declare a numbaric variable we just put a number after the equals sign but when we want to declare a String variable we should put the letter or the character that we want in a double quotes or a single quotes and when we want to declare a boolean variable we just put true or false.



#### changing the value of a variable 
* Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script.
* Once the variable has been created, you do not need to use the var keyword to assign it a new value. You just use the variable name, the equals sign (also known as the assignment operator), and the new va lue for that attribute.



#### Rules for naming variables
1. The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number. 
2. The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name.
3. You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something. For example, var is a keyword used to declare a variable. Reserved words are ones that may be used in a future version of JavaScript.
4. All variables are case sensitive, so score and Score would be different variable names, but it is bad practice to create two variables that have the same name using different cases.
5. Use a name that describes the kind of information that the variable stores. For example, fi rstName might be used to store a person's first name, l astNarne for their last name, and age for their age.
6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.


#### Arrays
* An array is a special type of variable. It doesn't just store one value; it stores a list of values.

##### values in array 
* Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).


#### Operators
* Expressions rely on things called operators; they allow programmers to create a single value from one or more values.


##### ARITHMETIC OPERATORS
* JavaScript contains the following mathematical operators, which you can use with numbers. You may remember some from math class.
1. Addition (+).
2. Subtraction (-).
3. Division (/).
4. Multiplication (*).
5. Increment (++).
6. Decrement (--).
7. Modulus (%).


##### String operators
* There is just one string operator: the+ symbol. It is used to join the strings on either side of it.



#### Decision making
* There are often several places in a script where decision are made that determine which lines of code should be run next.


##### Evaluating conditions and conditional statements
* There are two components to desision:
1. an expression is evaluated, which returns a value.
2. a conditional statement says what to do in a given situation.


##### comparison operators: evaluating conditions
1. (==)  : is eqal to .
2. (!=)  : is not eqal to .
3. (===) : strict eqal to .
4. (!==) : strict not eqal to.
5. (>)   : greater than.
6. (<)   : less than.
7. (>=)  : greater than or equal to.
8. (<=)  : less than or equal to.


##### Structuring comparsion operators
* (score >= pass)


##### USING COMPARISON OPERATORS
* At the most basic level, you can evaluate two variables using a comparison operator to return a true or fal se value. 
* example: ((5 > 2) && (2 >= 3))


##### Logical operators
1. (AND) we can write it like this (&&).
2. (OR) we can write it like this (||).
3. (NOT) we can write it like this (!).


##### IF STATEMENTS
* The if statement evaluates (or checks) a condition, if the condition evaluates to ture, any statements in the subsequent code block are exuted.


##### IF Else Statement
* The if...else statement checks a condition if it resolve to true the first block is executed, if the condition resolves to false the second code block is run instead.

