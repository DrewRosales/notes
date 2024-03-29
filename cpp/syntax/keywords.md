# keywords
Description and examples of keywords within C++

## default
Added to a function declaration to declare that a function is explicitly defaulted. Needs to be a special member function of the class. Using 'default' is a more efficient implementation than declaring an empty function {}.

**C++ 11 feature**
```
class foo {
  //constructor is generated by the compiler
  foo() = default;
};
```

## operator
Allows for the customization of how an object of a given class can be modified and interacted with
```
class foo {
  // deletes the parentheses assignment operator for the class
  operator() = delete;
};
```
<!-- TODO: Add a move semantics section that allows pairs with the operator keyword
## Move Semantics
-->

## friend
The friend keyword is used as a modifier for a class or function. A friend class or function allows the friend class or function to access the private and protected methods and variables of the parent class. 

```
class Node{
  // LinkedList can access the members of Node
  friend class LinkedList;
public:
  Node *parent;
  Node *child;
};
```

## function
Store, copy, and invoke callable targets such as functions, lambda expressions, bind, or function object

Parameters:
* R - return type
* args - input arguments

```
void print_num(int i) {
  std::cout << i << '\n'
}

std::function<void(int)> f_display = print_num;
```

In the example above, `f_display` has the return type of `void` and a single input of type 'int'

## Using
Keyword that allows for a couple of functions:
* namespaces
* aliasing
* directives

aliasing:
```
using ll = long long;

ll longValue;
```
directives:
```
using std::cout;
using std::endl;

cout << "Aliasing!" << endl;
```

