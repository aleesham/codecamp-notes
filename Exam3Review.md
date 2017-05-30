# Exam 3 Learning Objectives

## Lists
- Explain what is a list in Python.  
A list is a non-primative, mutable data type. 

- Example how can you find the length of a list.  
You can use the function `len()` to find the length of a list.

- Explain how to access elements in a list.  
You can use bracket notations (`[]`) to access elements in a list.

- Explain how can you check if an item is in the list.  
You can set a varaible equal to the expression `item in a_list` to check if an item is in the list. This expression evaluates to `True` if the item is in the list and `False` if the item is not in the list.

- Explain how to concatenate a list.  
To concatenate lists, you can use the `+` operator. 

- Explain how you repeat a list.  
To repeat a list, you can use the `*` operator. 

- Explain how to slice a list.  
To slice a list, you can use the `[:]` operator. 

- Explain what it means for lists to be mutable. 
If a data type is mutable, pieces of it can be changed using bracket notation rather than having to reassign the whole thing. For example, if `a_lst =[1,2,3]` and we make the assignment `a_lst[0]`, then `a_lst is [0,2,3]` evaluates to `True`.

- Explain how to delete items from the list.  
You can use the `lst.remove(item)` or `lst.pop(position = -1)` methods to remove items from a list. The `remove()` method removes the first occurence of the item it is passed. The `pop()` method removes the item at the position it is passed and returns that value. Both of these methods are mutators; that is, they change the lists; they do not return updated lists.

- Explain how references work. (An example may help here.)
<!--- Explain this in better detail. --->  

- Explain what is aliasing.
<!--- Explain this in better detail. --->    

- Explain how to clone a list.  
<!--- Explain this in better detail. --->  

- Name some of the list methods. Particularly, these would be good to remember: `append`, `insert`.  

- Traverse though a list with a loop. 
You can traverse through a list using the code: `for item in lst.` 

- Explain how lists are sent as arguments. (That is, passing by reference versus passing by value.)  

- Explain what is a pure function.  

- Implement a function that produces a list of items (using the accumulator style).

- Explain what is a list comprehension.  

- Implement an example of how to access an element from nested lists.  

- Explain how the string split method works.  

- Explain what is a tuple and how they differ from lists.  
A tuple is a non-primitive immutable data type that can hold different types of data in each index. They are very similar to lists except for the fact that they are immutable.

- Explain how tuple assignment works.  

- Implement a function that produces a tuple.  

```
def coorPoint(x,y):
    return (x,y)
```

## Dictionaries
- Explain what a dictionary is.  
A key must be an immutable data type. 

- Create dictionaries with entries.  

- Explain what it means to say that "dictionaries are mutable."  

- Access individual elements of a dictionary.  
You can use bracket notation or the `.get()` method.

- Modify individual elements of a dictionary.  

- Loop through the elements of a dictionary.  

- Use dictionary methods such as `keys()`, `values()`, and `get()`.  


## Objects
- Explain what an object is. In particular, what does an object contain?  
An object is something created from a specific class. 

- Write your own user defined class.  
    - Explain what is an initializer method.  

- Explain what is a class versus an instance.  
An object is an instance of a class.

- Explain how objects are passed as arguments.

- Explain how to convert an object to a string.  

## Inheritance
- Explain how equality/sameness is in objects.  

- Explain what is inheritance.  

- Implement a super-sub class relationship.  