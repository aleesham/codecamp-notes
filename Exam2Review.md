# Exam 2 Learning Objectives

## Conditionals
- Describe what is a boolean.  
A boolean is a data type that stores either `True` or `False`. 

- Describe what are logical operators.  
Logical operators include `and`, `or`, and `not`. There are also six comparision operators: `<`, `<=`, `>`, `>=`, `==`, `!=`. These are less than, less than or equal to, greater than, greater than or equal to, equal to, and not equal to, respectively. 

- Describe the order of precedence with logical operators.  
First, we do any mathematics necessary using the ordinary order of operations. Then we do comparisons. And finally logical operators. 

- Write an if statement with an else clause.  
```{p}
if number % 2 == 0:
    print("The number", number, "is even.")
else:
    print("The number", number, "is odd.")
```

- Write a (nested) if statement with an elif clause.  
```{p}
if number % 2 == 0:
    print("The number", number, "is even.")
    if number < 0:
        print("The number", number, "is negative.")
    elif number > 0:
        print("The number", number, "is positive.")
    else:
        print("The number", number, "is zero.")
else:
    print("The number", number, "is odd.")
    if number < 0:
        print("The number", number, "is negative.")
    else:
        print("The number", number, "is positive.")
```

- Reduce a boolean function to a boolean expression.  
[Examples](https://runestone.launchcode.org/runestone/static/thinkcspy/Selection/BooleanFunctions.html)

## More About Iteration
- Write a for loop.
```
# nums is some list of numbers
total = 0
for num in nums:
    total += num
avg = total/len(nums)
```

- Write a while loop.
```
a_string = ""
while( a_string != "exit"):
    a_string = input("What do you want me to print? If you want to exit, type 'exit'.\n")
    print(a_string)
```    

- Explain what is an infinite loop.  
An infinite loop can only occur in a while loop. It occurs when the condition of the while loop always evaluates to true. For example, the following example is an infinite loop that continuously prints Hello.   
```
while True:
    print("Hello.")
```

- Explain how an image is stored digitally.  
We store an image digitally by using a matrix of colors, or 2-dimensional sheet containing pixels where each pixel has its own specific color. 

- Explain how color is modeled on a computer.  
We model color on a computer using the RGB Color Model. The specific color of a pixel depends on a formula that mixes various amounts of three basic colors: red, green, and blue. The amount of each color, sometimes called the intensity of the color, allows us to have very fine control over the resulting color.


- Write a program that processes an image.  
[Examples](https://runestone.launchcode.org/runestone/static/thinkcspy/MoreAboutIteration/2DimensionalIterationImageProcessing.html)
## Strings
- Explain what is a collection data type and why a string is an example.   
A collection data type is a data type that is composed of smaller pieces of data. A string is considered to be a collection data type because it can be considered a sequential collection of one-character strings.

- Explain what is a string concatenation and how to perform it in Python.   
String concatenation is taking two (or more) strings and adding them together. We concatenate the first string to the second string by simply creating another string that starts with the entirety of the first string and "pastes" the second string to the end of the first. In Python, we do this by using the `+` operator with two strings. For example, `print("Hello" + "World")` would print HelloWorld.

- Explain what is string repetition and how to perform it in Python.
String repetition is repeating a string over and over again. It is basically concatenating a string with itself some given number of times. We can perform it in Python using the `*` operator. For example, `3*"Hello` is equivalent to `"Hello"+"Hello"+"Hello"`. Both of these are equivalent to the concatednated string `"HelloHelloHello"`.

- Explain how to index into a string.  
Use bracket notation to index a string. For example, if `a_str="Hello"`, then we can use `a_str[i]` to access the letter in the ith postion. Some examples include: `a_str[0] == "H"`, `a_str[3] == "l"`, and `a_str[-4] == "e"`. Note if i is out of range, Python will give an error. The index i can be between `-len(a_str)` and `len(a_str)-1` (inclusively).

- Describe some of the methods we can perform on strings.  
[String Methods](https://runestone.launchcode.org/runestone/static/thinkcspy/Strings/StringMethods.html)

- Explain how the len function works.  
The `len` function returns the length of the string. It is worth noting that the length is NOT a usable index as we start indexing from 0.

- Explain how the slice operator works.  
The slice operator uses bracket notation. For example, `print(a_str[n:m])` would print the string `a_str` from its nth position up to but not including the character in its mth position. A more concrete example is as follows `print("Hello"[2:4])` would print the string 'll'. Note that we can also use the notation `a_str[:m]` to print the beginning of the string, up to but not including the character in the mth postion or we can use the notation `a_str[n:]` to print the end of the string starting from and including the character in the nth position.

- Explain what are ordinal values in strings. (How does this apply to Lexicographical Order?)  
Each length one string is assigned a unique integer, called its ordinal value. This is how computers can distinguish lowercase and uppercase letter. Lexicographical order is similar to alphabetical order; however, capitalization matters. It turns out that all capital letters come before lowercase letters in lexigraphical order. Therefore `"D" > "z"` would evaluate to `False` since `"D"` is capitalized.

- Explain what it means for strings to be immutable.  
You cannot change a part of a string without creating a new string variable or reassigning the current variable. For example, the reassignment `a_str[0] = "a"` would produce an error, but we could get around this by using the following assignment: `a_str = "a" + a_str[1:]`.