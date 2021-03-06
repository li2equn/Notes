# PHP5

PHP is a server scripting language, and a powerful tool for making dynamic and interactive web pages

## PHP Syntax

### Basic PHP Syntax
A PHP scripts starts with <?php and ends with ?>
```php
<?php
//PHP code
?>
```
### Comments in PHP
```php
<?php
// This is a single-line comment

# This is also a single-line comment

/*
This is a multiple-lines comment block
that spans over multiple
lines
*/

// You can also use comments to leave out parts of a code line
$x = 5 /* + 15 */ + 5; //result = 10
echo $x;
?>
```

### PHP Case Sensitivity
- all keywords(eg. if, else, while, echo, etc.), classes, functions, and user-defined functions are **NOT** case-sensititive
- all variables names are case-sensitive 


## PHP Variables

### Creating(Declaring) PHP Variables

- A variable starts with the $ sign, followed by the name of the variable
- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive ($age and $AGE are two different variables)
- PHP automatically converts the variable to the correct data type, depending on its value.

## PHP Variable Scope:

- local
- global
- static

### Global and Local Scope
- A variable declared outside a function has a GLOBAL SCOPE and can only be accessed outside a function
- A variable declared within a function has a LOCAL SCOPE and can only be accessed within that function

### PHP The global Keyword
- The global keyword is used to access a global variable from within a function.
- To do this, use the global keyword before the variables (inside the function)

```php
<?php
$x = 5;
$y = 10;

function myTest() {
    global $x, $y;
    $y = $x + $y;
}

myTest();
echo $y; // outputs 15
?> 
```

PHP also stores all global variables in an array called $GLOBALS[index]. The index holds the name of the variable. This array is also accessible from within functions and can be used to update global variables directly.
```php
<?php
$x = 5;
$y = 10;

function myTest() {
    $GLOBALS['y'] = $GLOBALS['x'] + $GLOBALS['y'];
} 

myTest();
echo $y; // outputs 15
?>
```


### PHP the static Keyword

Normally, when a function is completed/executed, all of its variables are deleted. However, sometimes we want a local variable NOT to be deleted. We need it for a further job.
To do this, use the static keyword when you first declare the variable:

```php
<?php
function myTest() {
    static $x = 0;
    echo $x;
    $x++;
}

myTest();
myTest();
myTest();
?> 
```

## PHP Data Types
PHP supports the following data types
- string
- integer
- float
- boolean
- array
- object
- NULL
- resource

### PHP Integer
- An integer must have at least one digit
- An integer must **not** have a decimal point
- An integer can be either positive or negative
- Integers can be specified in three formats: decimal (10-based), hexadecimal (16-based - prefixed with 0x) or octal (8-based - prefixed with 0)

```php
<?php 
$x = 5985;
var_dump($x);// The PHP var_dump() function returns the data type and value:
?>
```

### PHP Array
```php
<?php 
$cars = array("Volvo","BMW","Toyota");
var_dump($cars);
?>
```

### PHP Object
An object is a data type which stores data and information on how to process that data.

In PHP, an object must be explicitly declared.

First we must declare a class of object. For this, we use the class keyword. A class is a structure that can contain properties and methods:

```php
<?php
class Car {
    function Car() {
        $this->model = "VW";
    }
}

// create an object
$herbie = new Car();

// show object properties
echo $herbie->model;
?>
```

### PHP NULL Value
Null is a special data type which can have only one value: NULL.

A variable of data type NULL is a variable that has no value assigned to it.

If a variable is created without a value, it is automatically assigned a value of NULL.

Variables can also be emptied by setting the value to NULL:

## PHP string functions
```php
<?php
//strlen() returns the length of a string
echo strlen("Hello world!"); // outputs 12

//str_word_count() counts the number of words in a string
echo str_word_count("Hello world!"); // outputs 2

// strrev() reverses a string
echo strrev("Hello world!"); // outputs !dlrow olleH

//strpos() searchs for a specific text within a string
// If match found, return the character position of the first match
//if no match found, it will return FALSE
echo strpos("Hello world!", "world"); // outputs 6

//str_replace() replaces some characters with some other characters in a string
echo str_replace("world", "Dolly", "Hello world!"); // outputs Hello Dolly!
?>



```

## PHP Constants

- Constants are like variables except that once they are defined they cannot be changed or undefined
- a constant is an identifier(name) for a simple value. The value cannot be changed during the script
- a valid constant name starts with a letter or underscore(no $ sign)
- constants are automatically global across the entire script

### Syntax create a PHP constant
define(name, value, case-insensitive)

- name: Specifies the name of the constant
- value: Specifies the value of the constant
- case-insensitive: Specifies whether the constant name should be case-insensitive. Default is false

```php
<?php
// case sensitive constant
define("GREETING", "Welcome to W3Schools.com!"); 
echo GREETING;// output 
// case-insensitive constant
define("GREETINGS", "Welcome to W3Schools.com!", true);
echo greetings;

function myTest1() {
    echo GREETING;
}

function myTest2() {
    echo greetings;
}
 
myTest1();
myTest2();
?>

```


## switch Statement
Use the switch statement to select one of many blocks of code to be executed.

This is how it works: 

First we have a single expression n (most often a variable), that is evaluated once. The value of the expression is then compared with the values for each case in the structure. 

If there is a match, the block of code associated with that case is executed. 

Use break to prevent the code from running into the next case automatically. 

The default statement is used if no match is found.

```php
<?php
$favcolor = "red";

switch ($favcolor) {
    case "red":
        echo "Your favorite color is red!";
        break;
    case "blue":
        echo "Your favorite color is blue!";
        break;
    case "green":
        echo "Your favorite color is green!";
        break;
    default:
        echo "Your favorite color is neither red, blue, nor green!";
}
?>
```

## PHP loops

- while - loops through a block of code as long as the specified condition is true
- do...while - loops through a block of code once, and then repeats the loop as long as the specified condition is true
- for - loops through a block of code a specified number of times
- foreach - loops through a block of code for each element in an array

### while loop
```php
<?php 
$x = 1; 

while($x <= 5) {
    echo "The number is: $x <br>";
    $x++;
} 
?>

output:
The number is: 1 
The number is: 2 
The number is: 3 
The number is: 4 
The number is: 5 
```

### do...while loop

```php
<?php 
$x = 6; 

do {
    echo "The number is: $x <br>";
    $x++;
} while ($x <= 5);
?>

output:
The number is: 6

```
### for loop
```php
<?php 
for ($x = 0; $x <= 10; $x++) {
    echo "The number is: $x <br>";
} 

output:
The number is: 0 
The number is: 1 
The number is: 2 
The number is: 3 
The number is: 4 
The number is: 5 
The number is: 6 
The number is: 7 
The number is: 8 
The number is: 9 
The number is: 10 
?>
```

### foreach loop

```php
<?php 
$colors = array("red", "green", "blue", "yellow"); 

foreach ($colors as $value) {
    echo "$value <br>";
}
output:
red 
green 
blue 
yellow 
?>
```

## Superglobals
Several predefined variables in PHP are "superglobals", which means that they are always accessible, regardless of scope - and you can access them from any function, class or file without having to do anything special.

The PHP superglobal variables are:

- $GLOBALS
- $_SERVER
- $_REQUEST
- $_POST
- $_GET
- $_FILES
- $_ENV
- $_COOKIE
- $_SESSION
