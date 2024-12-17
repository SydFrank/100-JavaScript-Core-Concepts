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

   | Operator |          Description           |       Example       |
   | :------: | :----------------------------: | :-----------------: |
   |    +     |            Addition            |     5 + 2 -> 7      |
   |    -     |          Subtraction           |      5- 2 -> 3      |
   |    *     |         Multiplication         |     5 * 2 -> 10     |
   |    /     |            Division            |    5 / 2 -> 2.5     |
   |    %     | Modulus(remainder of division) |     5 % 2 -> 1      |
   |    ++    |    Increment(increase by 1)    | let a = 5; a++ -> 6 |
   |    --    |    Decrement(decrease by 1)    | let a = 5; a-- -> 4 |

   

2. Assignment Operators: used to assign values to variables

   | Operator |     Description     |       Example       |
   | :------: | :-----------------: | :-----------------: |
   |    =     |     Assignment      |       x = 10        |
   |    +=    |   Add and assign    | x += 5 -> x = x + 5 |
   |    -=    | Subtract and assign | x -= 5 -> x = x - 5 |
   |    *=    | Multiply and assign | x *= 5 -> x = x * 5 |
   |    /+    |  Divide and assign  | x /= 5 -> x = x / 5 |
   |    %=    | Modulus and assign  | x %= 5 -> x = x % 5 |

   

3. Comparison Operators: used to compare two values and return a boolean (true or false)

   | Operator |           Description            |      Example       |
   | :------: | :------------------------------: | :----------------: |
   |    ==    |   Equal to (loose comparison)    |  5 == '5' -> true  |
   |   ===    |   Equal to (strict comparison)   | 5 === '5' -> false |
   |    !=    | Not equal to (loose comparison)  |  5 != '5' -> true  |
   |   !==    | Not equal to (strict comparison) | 5 !== '5' -> false |
   |    >     |            Great than            |   5 > 3 -> true    |
   |    <     |            Less than             |   5 < 3 -> false   |
   |    >=    |     Greater than or equal to     |   5 >= 5 -> true   |
   |    <=    |      Less than or equal to       |  5 <= 3 -> false   |

   

   > What is the difference between == and === ?

   |    Freture    |      == (Equality operator)       |      === (Strict equality operator)       |
   | :-----------: | :-------------------------------: | :---------------------------------------: |
   | Type Coercion |  Yes (performs type conversion)   |          No (no type comversion)          |
   |  Strictness   | Less strict, compares only values | More strict, compares both value and type |

   

4. Logical Operators: used to perform logical operations, typically with boolean values

   | Operator | Description |        Example         |
   | :------: | :---------: | :--------------------: |
   |    &&    | Logical AND | true && false -> false |
   |    !     | Logical NOT |     !true -> false     |

   

5. Conditional (Ternary) Operator: a shorthand for  if-else statement

   |         Operator          |                         Description                          |                   Example                    |
   | :-----------------------: | :----------------------------------------------------------: | :------------------------------------------: |
   | condition ? expr1 : expr2 | if condition is true, expr1 is returned, otherwise expr2 is returned | let result = (5 > 3) ? 'Yes' : 'No' -> 'Yes' |

   

6. Type Operators: used to check or change the type of a value

   |  Operator  |                  Description                  |           Example           |
   | :--------: | :-------------------------------------------: | :-------------------------: |
   |   typeof   |         return the type of a variable         |    typeof 5 -> 'number'     |
   | instanceof | checks if an object is an instance of a class | [] instanceof Array -> true |

   

7. Bitwise Operators: used to work on the binary representations of numbers

   | Operator | Description |   Example    |
   | :------: | :---------: | :----------: |
   |    &     | Bitwise AND |  5 & 3 -> 1  |
   |    <<    | Lest shift  | 5 << 1 -> 10 |

   

8. String Operators: used to manipulate strings

   | Operator |       Description        |                       Example                       |
   | :------: | :----------------------: | :-------------------------------------------------: |
   |    +     |      concatenation       |       "Hello" + " " + "World" → "Hello World"       |
   |    +=    | concatenation and assign | let str = "Hello"; str += " World"; → "Hello World" |

   

9. Spread and Rest Operators: used to handle collections of data

   | Operator |                  Description                   |                           Example                            |
   | :------: | :--------------------------------------------: | :----------------------------------------------------------: |
   |   ...    | spread (unpacks elements from array or object) |      let arr = [1, 2, 3]; let newArr = [...arr, 4, 5];       |
   |   ...    |      rest (collects remaining arguments)       | function sum(...numbers) { return numbers.reduce((a, b) => a + b);} |

   

10. Nullish Coalescing Operators: returns the right-hand operand if the left-hand operand is null or undefind

    | Operator |    Description     |                Example                 |
    | :------: | :----------------: | :------------------------------------: |
    |    ??    | Nullish Coalescing | let x = null ?? 'default'; → 'default' |

    

# 6. Template Literals (Template strings)

## 6.1 Concept

> Template literals are literals delimited with backtick (`) characters, allowing for multi-line strings, string interpolation with embedded expressions, and special constructs called tagged templates.

## 6.2 String Interpolation

```javascript
let name = "John";
let age = 30;
let greeting = `Hello, my name is ${name} and I am ${age} years old.`;
console.log(greeting);  // Output: Hello, my name is John and I am 30 years old.

```

## 6.3 Multi-line String

```javascript
let multiLineString = `This is the first line
This is the second line
And this is the third line`;

console.log(multiLineString);


Output:
This is the first line
This is the second line
And this is the third line
```

## 6.4 Tagged Templates

> Tags allows you to parse template literals with a function

> 1. first argument: an array of string values
> 2. remaining arguments: related to the expressions

```javascript
function tag(strings, ...values) {
    console.log(strings);  // The literal strings
    console.log(values);   // The interpolated values
    return "Finished";
}

let name = "Alice";
let age = 25;
let message = tag`Hello, my name is ${name} and I am ${age} years old.`;
console.log(message);  // Output: Finished


Output:
[ 'Hello, my name is ', ' and I am ', ' years old.' ]
[ 'Alice', 25 ]
Finished

```

# 7. Truthy and Falsy Values

## 7.1 Falsy Values

1. false
2. 0
3. -0 (minus zero)
4. 0n (BigInt zero)
5. '', "", `` (empty string)
6. null
7. undefined
8. NaN

## 7.2 Truthy Values

1. true
2. Any non-zero number
3. Non-empty string: any string that is not empty ("hello", " ").
4. Objects: all objects are truthy, even if they are empty ({} or []).
5. Functions: functions are truthy, even if they don't return anything.
6. BigInt values: any non-zero BigInt

# 8. Loops and iteration

1. for statement

   ```javascript
   for (initialization; condition; afterthought)
     statement
   
   ```

2. do...while statement

   ```javascript
   do
     statement
   while (condition);
   
   ```

3. while statement

   ```javascript
   while (condition)
     statement
   
   ```

4. labeled statement: lets you refer to it elsewhere in your program

   ```javascript
   label:
     statement
   
   ```

5. break statement

   ```javascript
   break;
   break label;
   
   1. The first form of the syntax terminates the innermost enclosing loop or switch.
   2. The second form of the syntax terminates the specified enclosing labeled statement.
   ```

   ```javascript
   let x = 0;
   let z = 0;
   labelCancelLoops: while (true) {
     console.log("Outer loops:", x);
     x += 1;
     z = 1;
     while (true) {
       console.log("Inner loops:", z);
       z += 1;
       if (z === 10 && x === 10) {
         break labelCancelLoops;
       } else if (z === 10) {
         break;
       }
     }
   }
   
   ```

6. continue statement

   ```javascript
   continue;
   continue label;
   
   ```

7. for...in statetment: iterates a specified variable over all the enumerable properties (keys) of an object.

   ```javascript
   for (variable in object)
     statement
   
   ```

   ```javascript
   let person = { name: "Alice", age: 30, city: "New York" };
   
   for (let key in person) {
       console.log(key, person[key]);
   }
   // Output:
   // name Alice
   // age 30
   // city New York
   ```

8. for...of statement: creates a loop iterating over iterable objects

   ```javascript
   for (variable of iterable)
     statement
   
   ```

   ```javascript
   let numbers = [10, 20, 30];
   
   for (let value of numbers) {
       console.log(value);
   }
   // Output:
   // 10
   // 20
   // 30
   ```



# 9. Function 



# 10. Working with Http Requests

## 10.1 Steps to Use XMLHttpRequest

1. Create an XMLHttpRequest Object
2. Call the open() method
3. Set Request Headers (Optional)
4. Register Callback Functions
5. Send the Request()

```javascript
const listElement = document.querySelector(".posts");
const postTemplate = document.getElementById("single-post");

// 1.Create an XMLHttpRequest Object
const xhr = new XMLHttpRequest();

// 2.Call the open() Method
xhr.open("GET", "https://jsonplaceholder.typicode.com/posts");

xhr.responseType = "json";

// 4.Register Callback Functions
xhr.onload = function () {
  // const listOfPosts = JSON.parse(xhr.response);
  const listOfPosts = xhr.response;
  for (const post of listOfPosts) {
    const postEl = document.importNode(postTemplate.content, true);
    postEl.querySelector("h2").textContent = post.title.toUpperCase();
    postEl.querySelector("p").textContent = post.body;
    listElement.append(postEl);
  }
};

// 5.Send the Request
xhr.send();

```

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Http</title>
    <link rel="stylesheet" href="assets/styles/app.css" />
    <script src="assets/scripts/app.js" defer></script>
  </head>
  <body>
    <template id="single-post">
      <li class="post-item">
        <h2></h2>
        <p></p>
        <button>DELETE</button>
      </li>
    </template>
    <section id="new-post">
      <form>
        <div class="form-control">
          <label for="title">Title</label>
          <input type="text" id="title" />
        </div>
        <div class="form-control">
          <label for="content">Content</label>
          <textarea rows="3" id="content"></textarea>
        </div>
        <button type="submit">ADD</button>
      </form>
    </section>
    <section id="available-posts">
      <button>FETCH POSTS</button>
      <ul class="posts"></ul>
    </section>
  </body>
</html>

```

## 10.2 JSON.parse(xhr.response) VS xhr.responseType = 'json'

|        Feature        |        JSON.parse(xhr.response)         |     xhr.responseType = 'json'     |
| :-------------------: | :-------------------------------------: | :-------------------------------: |
|    Parsing Method     |    Manual parsing using JOSN.parse()    |     Automatic parsing by XHR      |
|     Response Type     |  Working with the default 'text' type   |   Require responseType = "json"   |
|    Error Handling     |  Throws SyntaxError if JOSN is invalid  |   Returns null for invalid JSON   |
| Browser Compatibility |  Works in all browsers ( including IE)  | Supported only in modern browsers |
|       Use Case        | When handling raw JSON or mixed formats |  When expecting a JSON response   |

## 10.3 Promisifying Http Request (with XMLHttpRequest)

```javascript
const listElement = document.querySelector(".posts");
const postTemplate = document.getElementById("single-post");

function sendHttpRequest(method, url) {
  const promise = new Promise((resolve, reject) => {
    const xhr = new XMLHttpRequest();
    xhr.open(method, url);
    xhr.responseType = "json";

    xhr.onload = function () {
      resolve(xhr.response);
    };
    xhr.send();
  });
  return promise;
}

async function fetchPosts() {
  const responseData = await sendHttpRequest(
    "GET",
    "https://jsonplaceholder.typicode.com/posts"
  );

  const listOfPosts = responseData;
  for (const post of listOfPosts) {
    const postEl = document.importNode(postTemplate.content, true);
    postEl.querySelector("h2").textContent = post.title.toUpperCase();
    postEl.querySelector("p").textContent = post.body;
    listElement.append(postEl);
  }
}

fetchPosts();

```

##  10.4 Using the fetch() API

### 10.4.1 Concept

> fetch() is used to make HTTP requests aysnchronously and returns a Promise that resolves to a Response object.

### 10.4.2 Basic Syntax

``` javascript
fetch(url, options)
  .then(response => { 
    // Handle the response
  })
  .catch(error => { 
    // Handle errors
  });



url: the URL to which the request is sent.
options(optional): an object to customize the request(method, headers, body,etc.).
```

### 10.4.3 fetch() Returns a Promise

1. Resolved Promise: when the request completes successfully, the Promise resolves with the Response object.
2. Rejected Promise: if there's a network error or a failure in sending the request, the Promise is rejected, and the error is passed to the catch() method.

### 10.4.4 Response Object

```javascript
Response {
  body: ReadableStream,     // The body of the response as a byte stream
  bodyUsed: false,          // Whether the response body has been consumed
  headers: Headers,         // The Headers object containing the response headers
  ok: true,                 // Whether the response status code is in the 2xx range
  redirected: false,        // Whether the request was redirected
  status: 200,              // The HTTP status code
  statusText: "OK",         // The HTTP status text
  type: "cors",             // The type of the request (e.g., "cors", "basic")
  url: "https://jsonplaceholder.typicode.com/posts/1" // The URL of the request
}

```

### 10.4.5 Complete execution flowchart:

```javascript
fetch()  -> Returns a Promise
   |
   v
Resolves to a Response object (response)
   |
   v
Call response.json() -> Returns a Promise
   |
   v
Parse JSON data -> JavaScript object (data)
   |
   v
.then(data => ...) Callback
   |
   v
.catch(error => ...) Error handling

```

### 10.4.6 Example code

```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1')
  .then(response => {
    if (!response.ok) {  // Check if the response status is OK (2xx)
      throw new Error('Network response was not ok');
    }
    return response.json();  // Parse the response body as JSON
  })
  .then(data => {
    console.log('Fetched data:', data);  // Handle the parsed data
  })
  .catch(error => {
    console.error('There was a problem with the fetch operation:', error);  // Handle errors
  });

```



# 11. Webpack

## 11.1 Initial Setup

> 1. npm init -y
> 2. npm install webpack webpack-cli --save-dev
> 3. npx webpack
> 4. npx webpack --stats detailed  (optional)

## 11.2 Customize Webpack Configuration

### 11.2.1 Add **"build": "webpack"**

#### 11.2.1.1 Simplifies the Command

- Without the script, you would need to run:

  ```javascript
  npx webpack
  ```

- After adding it, you only need to run:

  ```javascript
  npm run build
  ```



































