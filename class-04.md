# summarizing

## HTML

#### Links
* Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

##### Writing Links 
* Links are created using the (a) element. Users can click on anything between the opening (a) tag and the closing (/a) tag. You specify which page you want to link to using the href attribute.


##### Linking to other sites
* Links are created using the (a) element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.


##### Linking to other pages on the same site
* When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL.


##### Directory stucture
* On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.


##### relative urls 
* Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.


##### relative link type 
1. same folder
2. child folder
3. grandchild folder
4. parent folder
5. grandparent folder


##### Email links
* mailto: To create a link that starts up the user's email program and addresses an email to a specified email address, you use the (a) element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to. 


##### opening links in a new window
* target: If you want a link to open in a new window, you can use the target attribute on the opening (a) tag. The value of this attribute should be _blank.


##### Link to a specific part of the same page
* At the top of a long page you might want to add a list of contents that links to the corresponding sections lower down. Or you might want to add a link from part way down the page back to the top of it to save users from having to scroll back to the top.


##### Linking to a specific part of another page
* If you want to link to a specific part of a different page (whether on your own site or a different website) you can use a similar technique.



## CSS


#### Layout


##### Building blocks
* CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
* Block-level elements: start on a new line.
* Inline elements: flow in between surrounding text.


##### containing elements
* If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.


##### controlling the position of elements
* CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS.


##### we can float elements using float property:
1. normal flow.
2. realtive positioning.
3. absolute positioning.


##### Box offset
* to indicate where a box should be positioned
* the values that we use for it:
1. fixed positioning 
2. floating positioning


##### z-index
* When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.



## Javascript


#### function-method-object
* complex scripts can run to hundreds (even thousands) of lines.


##### What is a function?
* Functions let you group a series of statements together to perform a specific task.


##### Declaring a function
* To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces.
* example: function sayHello() {
*    document.write('Hello!');
* }


##### calling a function  
* Having declared the function, you can then execute all of the statements between its curly braces with just one line code.
* sayHello();


##### Declaring functions that need information
* sometimes a function needs specfic information to perform its task.
* function getArea (width,height){
*    return width * height;
* }



##### calling functions that need information
* when you call a function that has parameters, you specify the values it should use in the parentheses that follow its name.
* Arguments as values : getArea(3,5);
* Arguments as variables : 
1. wallwidth = 3;
2. wallheight = 5;
3. getArea(wallWidth, wallHeight);


##### Anonymous functions and functions expressions
* Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression, (e.g., as an argument to a function), then it gets treated as an expression.



##### Immediately invoked function exoressions 
* This way of writing a function is used in several different situations. Often functions are used to ensure that the variable names do not conflict with each other (especially if the page uses more than one script).



##### Variable scope
* The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.
1. Local Variable 
2. Global Variable



##### How memory and variables work
* Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed.



#### 6 reasons for pair programming 

##### How does pair programming work?  
*  While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator.
1. the driver: it's the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. 
2. the navigator:  thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.


##### Why pair programming? 
* While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful.
* Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves. 



##### 1 Greater efficiency
* It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product).


##### 2 Engaged collaboration
1. When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone.
2. Another important aspect of learning to program is knowing when to ask for help.


##### 3 Learning from fellow students
* Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.


##### 4 Social skills
* Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities.



##### 5 Job interview readiness
* A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen.


##### 6 Work environment readiness
* Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.

