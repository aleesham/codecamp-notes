## Chapter Five: Functions Notes

1. Does a function have to have parameters?  
No. For example, we can have the following:
```
def hello_world()
    print("Hello, world!")
```

2. What happens if we call a function without providing a value for one or more input parameters?  
We get a type error message.

3. Does a function have to return a value?  
No. Consider the example in question one.

4. What happens if we have a function that doesn't return a value, but we try to store a return value in a variable?  
The code executes, but nothing is stored in the variable. If you print the type of the variable, you see `<class 'NoneType'>`.