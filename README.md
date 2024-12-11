# 1. Variables

##  1.1 Concept:

> 1. A variable is a container used to store a value.
> 2. An identifier is the name used to refer to a variable.

 ```javascript
 let age = 25;  
 // 'age' is a variable that holds the value 25
 // 'age' is the identifier
 ```

## 1.2 Identifiers naming rules

1. Starts with a letter, underscore(__) , or dollar sign($).
2. Cannot start with a digit.
3. Subsequent characters can include letters, underscore(__), dollar sign($), or digits.
4. Case-sentitive.
5. Cannot be a reserved keyword.
6. Cannot contain spaces.
7. Can use Unicode characters.

# 2.Data Types

## 2.1 Primitive Data Types

1. Number: used for decimals and integers
2. String: used for text
3. Boolean: used for taking decisions
4. Undefined: a variable that has been declared but has not been assigned a value yet
5. Null: empty value
6. Symbol: value that is unique and immutable 
7. BigInt: used for numbers larger than 2^53 -1

## 2.2



# 3. Variable Declaring: const & let & var

|                |          const          |           let           |      var       |
| :------------: | :---------------------: | :---------------------: | :------------: |
|     Scope      |          Block          |          Block          |    Function    |
|  Reassignable  |           No            |           Yes           |      Yes       |
| Re-declaration |           No            |           No            |      Yes       |
|   Mutability   |    Immutable Binding    |         Mutable         |    Mutable     |
|    Hoisting    | Yes(Temporal Dead Zone) | Yes(Temporal Dead Zone) | Yes(undefined) |

> Q: What is hoisting ?
>
> Answer: Hoisting is JavaScript's  default behavior of moving declarations to the top.

# 4. Variable Scope

|   Scope Type   |                       Where it applies                       |                          Access                           |
| :------------: | :----------------------------------------------------------: | :-------------------------------------------------------: |
|  Global Scope  |  Variables/functions declared outside of any function/block  |           Accessible from anywhere in the code            |
| Function Scope |        Variables declared with var inside a function         |           Accessible only within that function            |
|  Block Scope   |     Variables declared with let or const inside a block      |             Accessible only within that block             |
| Lexical Scope  | Refers to the functions's ability to access variables from its outer(enclosing) functions | Inner functions can access variables from outer functions |



# 5.Operators

1. Arithmetic Operators:  used to perform mathematical operations
   1. 
   2. -
   3. /
   4. *
   5. %
   6. ++
   7. --
2. Assignment Operators
   1. 
3. 

