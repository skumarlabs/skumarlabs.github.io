## Interning
Reusing object on demand

At startup, Python(CPython), pre-loads a global list of integers in the range [-5, 256] <---- Singleton objects

Strings can also be interned using sys.intern("your string") :

#### Why?

1. Dealing with a large number of strings that could have high repetition e.g. tokenizing a NLP corpus
2. Lots of string comparisons
3. Memory optimization

## Peephole Optimizations

Constant Expressions
Short sequences length < 20

#### Membership Tests

`
    if e in [4, 3, 5]:
        pass
`

will become immutable version:

`
    if e in (4, 3, 5):

        pass
`

Extended Unpacking

a, *b = [1, 2, 3, 4]
The * operator can only be used once in LHS.

**operator: Key-value pair unpacking


*Single start scoops up positional arguments and stored as tuple and ** double start scoops up keyword arguments and stored as dictionary.

def func(*arg **kwargs):
    # arg = (1, 2)
    # kwargs = {'a': 10, 'b': 20}
    pass


func(1, 2, a=10, b=20)

Default parameters are calculated while import of function

Don't use mutable types in default parameters

















