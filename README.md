# Simbly
  A new programming language

# Syntax

## Operators
### Mathematical Operators
  - `add`: Sum 2 numeric values
  - `sub`: Subtract 2 numeric values
  - `mul`: Multiplication 2 numeric values
  - `div`: Divide 2 numeric values
### Assignment Operators
  `is`  : For assign non-array data
  ```
  int x is 5
  char sex is 'F'
  char ref addrsex is deref sex
  ```
  `are` : For assign array data
  ```
  int myList are 1, 2, 3, 4, 5
  char name are "Kutay"
  ```
  `in`  : Accessing array elements
  ```
  char name are "Kutay"
  name[0] is 'G'
  // name = Gutay
  ```
### Comparison Operators
  - `g` : Greater '>'
  - `s` : Smaller '<'
  - `ge`: Greater or Equel '>='
  - `se`: Smaller or Equel '<='
  - `e` : Equel '='

## Variable Assignment
  General Rules:
  `<type> <ref?> <name> is/are <expression>`
  ```
  int myVariable is 5
  char ref message is "Im Using Simbly!"
  int myList are 0,1,2,3,4
  char myString are "Im using Simbly!"
  char ref users are "Kutay", "Ertug", "Ates"
  ```

## Accessing Array
  ```
  int mylist are 0,1,2,3,4
  print(2 in mylist)
  ```
  Accessing second element in array and print consolr

  ```
  2 in mylist is 5
  ```
  Changes the second element in the array

## Loops
### For Loop
  ```
  for int i is 0 and i to 6 by 2 do
    // code
  end
  ```
  It increases by 2 from 0 to 6.

### While Loop
  ```
  while i e 5 do
    // code
  end
  ```
  It continues looping until i is not equal to 5.

## Functions
### Without Parameters
  ```
  float func pi() do
    return 3.14
  end
  ```
### With Parameters and Overloading 
  ```
  int func sum(int a, int b) do
    return a add b
  end
  
  float func sum(float a, float b) do
    return a add b
  end
  ```
## Class
### Basic Class
  ```
  class Animal do
    public:
      int size
      Animal() do end
      -Animal() do end
      int func get_size() do
        return this.size
      end
  end
  ```
### Generic & Overloading Class
  ```
  generic T
  class Vector do
    public:
      T ptr array
      int size
      Vector() do end
      void append(T element) do
        index this.size in array is element
      T get(int ind) do
        return index ind in this.array
      end
      -Vector() do end
  ```

## Imports
### Include Library with `from`
  ```
  from <path-with-dot>.<namespaces> import <class-or-function>
  ```
  Example:
  ```
  from stdlib.io import print, input
  ```
### Include Library without `from`
  ```
  import <path-with-dot>.<namespaces>.<class-or-function>
  ```
  Example:
  ```
  from stdlib.io import print, input
  ```

> “A simple language that compiles to pure Assembly — Simbly brilliant.”
 
