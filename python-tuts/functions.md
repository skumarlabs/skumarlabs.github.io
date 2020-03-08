First Class Object
1. can be passed to a function as an argument
2. can be returned from a function
3. can be assigned to a variable
4. can be stored in a data structure like list etc

High Order Functions
1. Take a function as an argument
2. Returns a function

* Docstrings are store in __doc__ property.
* Function annotations to document function parameters. Stored in __annotations__ property. Its a dictionary of parameter and their annotations.

def func1(a: "a string", b: "a positive integer") -> "a string":
    return a * b
    
Limitations of Lambda functions:
Single expression
No assignments
No annotations
__name__, __code__, __defaults__, __kwdefaults__

my_func.__code__.co_varnames

The inspect module

`import inspect`

ismethod(), isfunction(), isroutine()
An attribute that is callable is called a method.

inspect.getsource(my_func)
inspect.getmodule(my_func)
inspect.getcomments(my_func)
inspect.signature(my_func)

    
__new__(a, b) # object is created 

__init__(self, a, b) # object is initialized

__call__() makes a instance object callable

import functools

from functools import reduce

`l = [1, 2, 3, 4]` 

`reduce(lambda a, b: a if a < b else b, l)`

Built-in reducing functions:
min, max, sum, any, all
reduce() initializer

from functools import partial
f = partial(my_func, 10)
f(20, 30)

my_func(10, 20, 30)

Operator module:
itemgetter()
attrgetter()
methodcaller()












  
    