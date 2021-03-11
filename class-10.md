# summaraizing

## JS

### Error Handling and Debugging


#### Order of execution 
* To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.


#### Execution context
* The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.



#### The stack
* the javascript interpreter prcessess on line of code at a time. when a statement needs data from another functionm, it stacks (or piles) the new function on top if the current task.


#### EXECUTION CONTEXT and HOISTING
* Each time a script enters a new execution context, there are two phases of activity:
1. prepare
2. execute

#### UNDERSTANDING SCOPE
* In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.


#### UNDERSTANDING ERRORS
* If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.


#### ERROR OBJECTS
* Error objects can help you find where your mistakes are and browsers have tools to help you read them.


#### ERROR OBJECTS CONTINUED
1. syntax error
2. reference error
3. eval error
4. URIE error
5. type error
6. range error
7. error
8. NaN



#### How to deal with errors
* Now that you know what an error is and how the browser treats them, there are two things you can do with the errors.


#### A DEBUGGING WORKFLOW
* Debugging is about deduction: eliminating potential causes of an error. Here is a workflow for techniques you will meet over the next 20 pages. Try to narrow down where the problem might be, then look for clues.


#### BROWSER DEV TOOLS & JAVASCRIPT CONSOLE
* The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.


#### HOW TO LOOK AT ERRORS IN CHROME
1. The Console option is selected.
2. The type of error and the error message are shown in red.
3. The file name and the line number are shown on the right-hand side of the console.


#### HOW TO LOOK AT ERRORS IN FIREFOX
1. The Console option is selected. 
2. Only the JavaScript and Logging options need to be turned on. The Net, CSS, and Security options show other information. 
3. The type of error and the error message are shown on the left.
4. On the right-hand side of the console, you can see the name of the JavaScript file and the line number of the error.


###### You can also just type code into the console and it will show you a result.


#### WRITING FROM THE SCRIPT TO THE CONSOLE
* Browsers that have a console have a console object, which has several methods that your script can use to display data in the console. The object is documented in the Console API.



#### MORE CONSOLE METHODS
* To differentiate between the types of messages you write to the console, you can use three different methods:
1. console.info()
2. console.warn()
3. console.error()


#### WRITING TABULAR DATA
* In browsers that support it, the console. table () method lets you output a table showing:
* objects
* arrays that contain other objects or arrays


#### WRITING ON A CONDITION
* Using the console. assert() method, you can test if a condition is met, and write to the console only if the expression evaluates to false.


#### BREAKPOINTS
* You can pause the execution of a script on any line using breakpoints. Then you can check the va lues stored in variables at that point in time.


#### STEPPING THROUGH CODE
* If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur.


#### CONDITIONAL BREAKPOINTS
* You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.


#### DEBUGGER KEYWORD
* You can create a breakpoint in your code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.


#### HANDLING EXCEPTIONS
* If you know your code might fail, use try, catch, and finally. Each one is given its own code block.


#### THROWING ERRORS
* If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.


#### THROW ERROR FOR NaN
* If you try to use a string in a mathematical operation (other than in addition), you do not get an error, you get a special value called NaN (not a number).


#### DEBUGGING TIPS
* Here are a selection of practical tips that you can try to use when debugging your scripts.


#### COMMON ERRORS
* Here is a list of common errors you might find with your scripts:
1. Go back to basics
2. missed/extra characters
3. data type issues