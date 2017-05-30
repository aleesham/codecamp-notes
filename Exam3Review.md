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
[Documentation on references.](https://runestone.launchcode.org/runestone/static/thinkcspy/Lists/ObjectsandReferences.html)

- Explain what is aliasing.  
[Documentation on aliasing.](https://runestone.launchcode.org/runestone/static/thinkcspy/Lists/Aliasing.html)  
Aliasing can be considered as having different names for the same object. For example, we can alias in the following way:
```
a = [1,2,3]
b = a
# b is an alias for a.
a = [1,2,3]
b = [1,2,3]
# a and b are different instances of the list [1,2,3]. a is not an alias for b, and b is not an alias for a. 
```

- Explain how to clone a list.  
The easiest way to clone a list is to use slicing. However, you can clone a list using a list comprehension. For example:
```
a = [1,2,3]
# the following creates a new list rather than a reference to a.
b = a[:]
# the following also clones a list
c = [x for x in a]
```

- Name some of the list methods. Particularly, these would be good to remember: `append`, `insert`.  
[Examples of list methods.](https://runestone.launchcode.org/runestone/static/thinkcspy/Lists/ListMethods.html)

- Traverse though a list with a loop.  
You can traverse through a list using the code: `for item in lst.` 

- Explain how lists are sent as arguments. (That is, passing by reference versus passing by value.)  
Lists are passed by reference, and hence a function can mutate the original list.

- Explain what is a pure function.  
A pure function does not change any of its arguments.

- Implement a function that produces a list of items (using the accumulator style).  
```
def double_list(lst):
    double_lst = []
    for i in lst:
        double_lst += [2*i]
    return double_lst
```

- Explain what is a list comprehension.  
A list comprehension is basically a way to create a new list based on an old list with some new condition. For example, if we want to double everything in a list and store it into a new list, the following code would work
```
a = [1,2,3]
double_a1 = [2*x for x in a]

# the following is equivalent
double_a2 = []
for i in a:
    double_a2.append(2*i)

# the following only doubles odds
double_odds_a1 = [2*x for x in a if x%2]
```

- Implement an example of how to access an element from nested lists.  
```
lst_of_lsts = [[0,1,2], [1,2,3], [2,3,4]]
# lst_of_lsts[1] == [1,2,3]
# lst_of_lsts[1][2] == 3
```

- Explain how the string split method works.  
`str.split()` splits a string at spaces (`" "`) and return a list of string. You can also pass in a string argument to split elsewhere. For example:
```
# the following returns the list ["Hello","World"]
"Hello World".split()
# the following returns the list ["US", "500, JP", "600"]
"US$500, JP$600".split("$") 
```

- Explain what is a tuple and how they differ from lists.  
A tuple is a non-primitive immutable data type that can hold different types of data in each index. They are very similar to lists except for the fact that they are immutable.

- Explain how tuple assignment works.  
```
# T.F.A.E.
u,v = (4,5)
(u,v) = (4,5)
u,v = 4,5
```

- Implement a function that produces a tuple.  

```
def coorPoint(x,y):
    return (x,y)
```

## Dictionaries
- Explain what a dictionary is.  
A key must be an immutable data type. 

- Create dictionaries with entries.  
```
a_dct = {}
a_dct['Actor'] = 'Tom Hanks'
a_dct['Movie'] = 'Toy Story'
a_dct['Year'] = 1996
```

- Explain what it means to say that "dictionaries are mutable."  
Given a key, we can change the value at that particular key using just the assignment operator. Using the example above, we can change the value for the 'Movie' key as follows:

```
a_dct['Movie'] = 'Forest Gump'
```

- Access individual elements of a dictionary.  
You can use bracket notation or the `.get(k)` method. Note that we can add a second parameter to be returned should the key k not exis in the given dictionary.

- Modify individual elements of a dictionary.  
Consider the above bullet on mutability.

- Loop through the elements of a dictionary.  
There are several ways to loop through a dictionary. If you want to loop through the keys and values simultaneously, you can use: `for k,v in a_dct.items():`. However, you can just as well use `for k in a_dct:` or `for k in a_dct.keys():` and access its respective value using bracket notation (`a_dct[k]`). Further, if you just need the values, you can loop using `for value in a_dct.values():`.

- Use dictionary methods such as `keys()`, `values()`, and `get()`.  
Note the above bullet points using these methods.


## Objects
- Explain what an object is. In particular, what does an object contain?  
An object is something created from a specific class. 

- Write your own user defined class.  
    - Explain what is an initializer method.  
    The initilizer method initializes attributes that the programmer gives to the class. An example is offered below.

```
class Rectangle:

    def __init__(self, length, width):
        self.length = length
        self.width = width

    def get_perimeter(self):
        return 2*(self.width+self.length)

    def get_area(self):
        return self.width*self.length

    def __str__(self):
        return "Length: " + str(self.length) + ", Width: " + str(self.width)
```

- Explain what is a class versus an instance.  
An object is an instance of a class; the class definition gives a blueprint for an instance of a class.

- Explain how objects are passed as arguments.  
Objects are passed by reference, and hence a function can mutate the original list.

- Explain how to convert an object to a string.  
To convert an object to a string, you must include a `__str__` method. For example, refer to the above code for the Rectangle class.there

## Inheritance
- Explain how equality/sameness is in objects.  
The idea of sameness in objects (that is, using the `is` operator) is the same as the idea of sameness in lists. If b is an alias of a, then they refer to the same object. However, if a and b are different instances of the "same" object, they are not the same.

- Explain what is inheritance.  
Inheritance allows us to build a subclass for an already existing class. For example, building off of our Rectangle class above, we can build a square class as follows:

```
class Square(Rectangle):

    def __init__(self, side):
        Rectangle.__init__(self, side, side)
        
    def __str__(self):
        return "Side: " + str(self.length)
```

- Implement a super-sub class relationship.  
Refer to the above example. Note that the `__str__ ` method in the Square class overrides the `__str__` method in the Rectangle class for Square objects.