## Chapter Five: Functions Notes

1. Does a function have to have parameters?  
No. For example, we can have the following:

```
def hello_world()
    print("Hello, world!")
```

2. What happens if we call a function without providing a value for one or more input parameters?  
We get a `TypeError` message.

3. Does a function have to return a value?  
No. Consider the example in question one.

4. What happens if we have a function that doesn't return a value, but we try to store a return value in a variable?  
The code executes, but "nothing" is stored in the variable. Technically, the varible is set to the special value `None`. If you print the type of the variable, you see `<class 'NoneType'>`.

### Shadowing

A function can look at global variables, but a program cannot look at variables defined inside of a function UNLESS it is returned by that function. This then allows a program to have two variables of the same name: a global variable outside of the function and a local varaible of the same name defined within the function. However, the local varaible shawdows the global variable. The function does not change the global variable, it simply ignores it if it has its own.

Functions also cannot change global variables. Functions may only change local variables.

