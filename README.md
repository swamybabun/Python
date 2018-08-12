# Python

Python is high level programming language. Python is most wanted and widely used language now a days in every domains. Its good to learn such a cool language. I hope you will enjoy learning Python.

Let's begin the show..!

# Data types

1) **int**    -> Data type to store integer values
2) **float**  -> Data type to store floating point numbers
3) **str**    -> Data type to store text values
3) **bool**   -> Data type to store True or false

- Creating and initialising different data type variables

      age = 20
      salary = 20345
      pi = 3.4
      name = "test name"
      firstname = 'initial name'
      isValid = True

- To know the type of variable, you can user type() function.Few examples.

      type(age)         => int
      type(salary)      => int
      type(pi)          => float
      type(name)        => str
      type(firstname)   => str
      type(isValid)     => bool

- To print the value of a variable, you need to user print() function.

      area = 20
      print(area) => 20

      area = "Netherlands"
      print(area) => Netherlands

      area = True
      print(area) => True

Let us see on how to work with operators in Python.

- Operators :

There are different types of operators as usual as to other programming languages.

**Addition**  : + is addition operator  => Useful for calculating the addition of a number with another.

You can concatenate two strings using + operator.

    1 + 4 = 5

    1.4 + 5.9 = 7.3

    "firstname" + "lastname" => firstnamelastname

    "firstname" + 3 => gives you error as "Can't convert 'int' object to str implicitly"

**Subtraction**  : - is Subtraction operator  => Useful for calculating the subtracting a number from another.

    1 - 4 = -3

    5.9 - 4.3 = 1.6

    "firstname" - "lastname" => gives you error as "unsupported operand type(s) for -: 'str' and 'str'"

**Multiplication**  : * is multiplication operator => Useful for calculating the multipling a number with another.

    1 * 2 => 2

**Factorial** : **  =>  Useful for calculating the factorial of a number

    2 ** 3 = 8 => This means 2 * 2 * 2 which results in 8.

If you want to concatenate another data type with string, then you need to use str() function to convert non-string to string type and then you can concatenate two strings. This is useful in case of concatenating different type of data types in messages.

    "firstname" + 3 => This gives you error as you seen in above examples.

Let's convert 3 to string type and then try to concatenate.

    "firstname" + str(3) => firstname3

    "I will eat " + str(3) + " bananas and " + str(2) + " apples"  => I will eat 3 bananas 2 apples


Cool right... Keep going..

As of now, we have seen different data types which can hold a single value. But what to do, when we need to store multiple values in a single variable...?

The answer is **List**. Let us see how list works.

- **List**    

A list is a python data type. A list can contain any Python type. Although it's not really common, a list can also contain a mix of Python types including strings, floats, booleans, etc.

It's true; A python list can contain different data types in a single a list variable.

    Ex : sampleList =["12", 12.4, 1200, 'This is test', '1']

    [1, 3, 4, 2]

A list also can contain another lists.

    matrix = [[1, 2, 3], [4, 5, 7]]

    house = [["hallway Area", 120.67], ["kitchen Area", 12000], ["living room Area", 10.45]]

You can also have internal expressions in a list.

    temp_list = [1 + 2, "a" * 5, 3]

You can use **print()** and **type()** functions on a list too.

    house = [["hallway Area", 120.67], ["kitchen Area", 12000], ["living room Area", 10.45]]

    print(house) => [['hallway Area', 120.67], ['kitchen Area', 12000], ['living room Area', 10.45]]

When you print a type of list, it prints as below.

    print(type(house)) => list

List operations:

You can retrieve the required element from its position by their index position. Index starts from '0'.

  areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

      print(areas[0])  => will print ==> hallway
      print(areas[3])  => will print ==> 18.0

Accessing ranges in list: You can retrieve values in list by their ranges.

list[startingIndex:endingIndex] => it gives us the values in list from given starting position to the endingIndex position. Remember, it doesn't include endingIndex element.

      areas[2:8]  => This will give you values from second index position to 8th position.
  
      areas[:4] => this results values from 0th index to 4th index.

      areas[3:] => this results values from 3rd index to last index in list.

Look at below examples on how to read the range of values from lists.

      print(areas[0:3])  => will print ==> ['hallway', 11.25, 'kitchen']

      print(areas[3:6])  => will print ==> [18.0, 'living room', 20.0]

      print(areas[:3])  => will print ==> ['hallway', 11.25, 'kitchen']
      
      print(areas[3:])  => will print ==> [18.0, 'living room', 20.0, 'bedroom', 10.75, 'bathroom', 9.5]
