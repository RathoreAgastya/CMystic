
### Features of the language

# Declaring 

- `Declaring normal functions`

`use {name}({arguements})`

- an example

`use example(dec dig a)`

- use of curly bracket

`put code in curly brackets`

- example

```
use a(int dec a) {
    
}
```

# Declaring a variable

- `Real variables`

`dec {type} {variablename} = {content}`

- An example 

`dec dig my_var = 1`

- `Constants`

`immut {type} {variablename} = {content}`

- An example

`immut dig example = 252`

- `Characters`

`dec char {variablename} = {content}`

- An example

`dec char a = 'a'`

- `Integers`

`dec dig {variablename} = {content}`

- An example

`immut dig a = 2`

- `Strings`

`dec sentn {variable name} = {content}`

- An example

`dec sentn name = "Agastya"`

- Float (Decimal , duh)

`dec decm {variablename} = {content}`

- An example

`immut decm pi = 3.14`

# Comments 

- For creating a single-line comment

`~ {commentcontent}`

- Example
`~ This is a comment`

- For creating a multi-line comment

`~> {comment starts here} <~`

- Example

```
~>
This is a 
Multi-line comment!
<~
```

# Semicolons?

Put a semicolon at the end of every function or declaration

# Printing to the Console

`~ The most important thing, duh`

For printing something to the Console, use thet `out` function.

`out({text})`

- An example

`out("Hello, world!")` 

# OOP (Object Oriented Programming)

- For creating a class 

To create a class, use the keyword `cls`

```
cls {classname} {
    ~ Stuff in class
    ... 
}
```

- An example

```
cls my_class {
    ~ Put code in here
}
```

- Identity (self in Python)

- What is an identity? 

The identity parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class. 

- How to define one

Use the compiler recognized parameter `idt`

```
cls my_class() {
    use struct(idt, params, ...) {
        ~ Intialize params to idt
    }
}
```

- An example

```
cls my_class() {
    use struct(idt, dec dig num, dec immut decm pi) {
        idt.num = num
        idt.pi = pi
    }
} 
```

- To create a constructor

- First, what the hell is even a constructor?

A constructor is a set of parameters that is taken when intializing the class, it's kinda type of a *special method*.

- How to declare one?

First you need to create a class, then you need to add the compiler recognized function name `struct`

- An example

```
cls my_class {
    use struct(idt, params, ...) {
        ...
    }
}
```

- To create a method

- First, what is a method?

A method is a function of a class which you can access it through it's instance.

- How to declare one?

To create a method, you use the keyword `use clsmethod`

```
cls my_class() {
    use struct(idt, my_param) {
        idt.myParam = my_param
    }
    
    use clsmethod {name}(idt, params, ...) {
        ~ Code goes here
    }
}
```

- An example

```
cls my_class() {
    use struct(idt, dec dig a, ...) {
        idt.a = a
    }
    
    use clsmethod print_func(idt, dec decm a, ...) {
        out(a) 
    }
}
```

# Decorators

- First, what the hell is a Decorator?

A decorator is a design pattern that decs a user to add new functionality to an existing object without modifying its structure. 

# How to ignore identity?

Use the decorator `&stablemethod` for ignore using an identity

```
cls my_class() {
    use struct(idt, dec dig a, ...) {
        idt.a = a
    }
    
    &stablemethod 
    use clsmethod(dec decm a, ...) {
        put(a) 
    }
}
```

# Operators

- Arithmetic Operators

`+, -, /, //, *` are arithemtic operators, these are used to perform arithmetic expressions

- Examples

> `+`\

dec dig b = 4 + 5

> `-`\

dec dig a = 10 - 3

> `/`\

dec decm a = 12 / 5

> `//`\

dec dig n = 17 // 2

> `*`\

dec dig v = 2 * 7

- Assignment Operators

`=, +=, -=, *=, /=, ++, --, :` are assignment operators, these are used to give a constant/variable a value. 

- Examples

> `=`\

`dec sentn link = "example.com"`

> `+=`\

`dec dig a = 35`

`a += 5`

> `-=`\

`dec dig a = 35`

`a -= 5`

> `*=`\

`dec dig a = 10`

`a *= 2`

> `/=`\

`dec decm a = 6.45` 

`a /= 4`

> `++`\

this is incomplete

- Logical Operators

`|, &, >>, ==, ||, >, <` are logical operators, used to perform logical operations. 

# Conditionals

- What is conditionals?

A conditional statement as the name suggests itself, is used to handle conditions in your program.
what is this?
- on, elseon, other

# On

On means if the statement after the keyword `on` is true, it will execute the indented block on the next line

```
dec dig a = 1

on (a == )
```

# Elseon

Elseon means if the statement after the keyword `on` is not true and `elseon` is true, it will execute the indented block on the nextline

# Other

Other means if the statement after the keywords after `on` and `elseon` are not true, it will execute the idented block on the nextline