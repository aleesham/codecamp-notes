# Exam 1 Review

## Data and Variables
* Explain what a value is: a value is an object that a program manipulates. A value is a specific piece of data.

* Explain what a data type is: a data type is a class that a value can be such as integer, float, string, list, boolean.

* Give examples of the three data types int, float, and string:
    * `int` examples: `7`,`-1`
    * `float` examples: `5.0`, `3.1415`
    * `str` examples: `"Hello world"`, `"a"`

* Use the type conversion functions `int`, `float`, and `str`:
    * `int("14")`
    * `float("15.333333")`
    * `str(1245.34234)`

* Explain what a variable is: a variable is a box that holds one value

* Assign values to a variable: `a=5`, `name = "Aleesa"`

* Calculate the value of expressions using order of operations: PEMDAS

 
## Debugging 
* Describe how to debug programs using print and comments:
* Explain the three common error types (in all of computer programming): syntax error, runtime error, semantic (logical) error
    * Syntax: misusing :,0, or other symbols.
    * Runtime: these errors occur when the code is running. Runtime errors generally happen when a user is using it. 
    * Semantic: forgetting something logically; there is no syntax error, but it gives the wrong answer. These errors are genearlly the hardest to find.
* Give examples of each of the three common error types:
* Explain some best practices to avoid errors and debugging:
* Explain how each of the following (Python) errors may occur, with examples: `TypeError`, `ParseError`, `NameError`:
    * `TypeError`: mixing data types, such as adding a string and an int. This is usually a runtime error.
    * `NameError`: have not defined a variable that your using, usually means that you misspelled it. This is closest to a syntax errors. 


## Modules
* Explain the keyword import and what it is used for:
* Explain what a module is: a module is a file or set of files containing Python definitions and statements that someone else wrote.
* Explain the two steps needed to use a module: You need to install the module onto your machine (this is only necessary once). We then need to import the module into our script. Note that we have to use the dot notation to use something inside the module.
<!--- Ask about this --->
* Explain the difference between a function that is part of module and a function that is part of Python (such as print):
* List the three modules introduced in "Think Python" and describe what each might be used for:
* Explain where you might go to find information about a module:


## Loops
* Explain how to use for loop syntax with lists:`for list_item in list1`
* Explain the role of a loop iterator variable:
* Write a for loop that uses a list literal, such as [1, 2, 3, 4]:
* Write a for loop that uses the iterator variable in the loop body:
* Write a for loop that uses a list variable:
* Use the range function to generate lists of integers: 
    * `range(5)` is the list `[0,1,2,3,4]`
    * `range(2,15,3)` is the list `[2,5,8,11,14]`
    * `range(10,4,-2)` is the list `[10,8,6]`
* Use the range function within a list definition:
* Create turtle objects:
* Use common turtle methods including left, forward:


## Functions
* Explain what is a function: a function is a named sequence of statements that belong together. They are used to organize problems into chunks that match how we think about the solution to the problem. 

* Write a function with many parameters:
```
def compute_hypervolume_4Dcube(length , width, height, fourth_dimension):
    hypervolume = length*width*height*fourth_dimension
    return hypervolume
```

* Explain what a return statement does: it causes the function to return a value and also returns the flow of control back to the place in the program where the function was made.

* Describe what is scope and explain it with an example:
* Explain what is shadowing:

* Implement a problem that requires the accumulator style, such as adding up a list of numbers:
```
    def sumTo(n):
        accumulated_total=0
        for i in range(n+1):
            accumulated_total += i
        return accumulate_total
```

* Write a program that solves a problem using multiple functions:

* Explain why programming style is important:
* Explain why we use functions: 


## Conditionals
* Describe what is a boolean: A boolean is a data type. A boolean value can only take on two values: `True` or `False`. Booleans are used in logical statements or boolean arithmetic.
* Describe what are logical operators: There are three logical operators: `and`,`or`, and `not`. These have the same meanings as in the English language. For example, 
    * `x>0 and x<10` is equivalent to saying that "x is greather than zero and x is less than ten." 
* Describe the order of precedence with logical operators:
    PEMDAS-NAR
* Write an if statement with an else clause:
* Write a (nested) if statement with an elif clause:

<!--- Ask about this--->
* Reduce a boolean function to a boolean expression: