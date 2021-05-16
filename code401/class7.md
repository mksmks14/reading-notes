# Read : 07

## Game of Greed 2

### Python Scope

- In programming, the scope of a name defines the area of a program in which you can unambiguously access that name, such as variables, functions, objects, and so on.

- A name will only be visible to and accessible by the code in its scope.

- Several programming languages take advantage of scope for avoiding name collisions and unpredictable behaviors.

- Most commonly, you’ll distinguish two general scopes:

    1. **Global scope:** The names that you define in this scope are available to all your code.

    2. **Local scope:** The names that you define in this scope are only available or visible to the code within the scope.

#### Using the LEGB Rule for Python Scope

- Python resolves names using the so-called LEGB rule, which is named after the Python scope for names.

- The letters in LEGB stand for *Local*, *Enclosing*, *Global*, and *Built-in*.

1. **Local** *(or function)* scope is the code block or body of any Python function or lambda expression.   
   - This Python scope contains the names that you define inside the function.
   - These names will only be visible from the code of the function.
   - It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls.
   - This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.  

2. **Enclosing** *(or nonlocal)* scope is a special scope that only exists for nested functions.   
    - If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function.   
    - This scope contains the names that you define in the enclosing function. 
    - The names in the enclosing scope are visible from the code of the inner and enclosing functions.  

3. **Global** *(or module)* scope is the top-most scope in a Python program, script, or module.   
   - This Python scope contains all of the names that you define at the top level of a program or a module.   
   - Names in this Python scope are visible from everywhere in your code.

4. **Built-in** scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session.   
    - This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python.   
    - Names in this Python scope are also available from everywhere in your code.   
    - It’s automatically loaded by Python when you run a program or script.  


##### [Go Back](code_401_reading_notes.md)