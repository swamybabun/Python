# Python

Python is high level programming language. Python is most wanted and widely used language now a days in every domains. Its good to learn such a cool language. I hope you will enjoy learning Python.

Let's begin the show..!

### Download & Installation
Get latest Python version from [Download Python](https://www.python.org/downloads/) as per your operating system type. 

### PATH Setup
Add the PATH of Python interpreter to the PATH variable in case of Windows. In case of Mac, Add the path of python interpreter to the BASH file.

### Ways of Executing Python Programs
There are mainly two different ways of coding python programs. 
 
 1) By Python Script using any of IDE's like MyEclipse, Sublime, Atom  and many Python editor softwares.
 2) By Interactive mode using IPython Notebook. (is recommended for beginners)
 
1) Install any text editor or python supported IDE. I prefer Atom or Sublime.
     Download [Atom](https://atom.io/) or [Sublime](https://www.sublimetext.com/) and install it.

2) By Interactive Mode :
 
To run Python programs in interactive mode, you need to have IPython to be installed. There are two ways of installing it. 

- By Anaconda distribution
- By PIP package installer

The popular recommended type is to install the Anaconda and run IPython. Download [Anaconda](https://www.anaconda.com/download/) as per your operating system and install it.

Anaconda: (For beginners): This Need more space as its a huge package around (2.5 GB).

    conda update conda
    conda update ipython
 
PIP type installation : (For experienced people)  : Make sure, PIP is already installed.
 
    pip3 install --upgrade pip
    pip install ipython

You can also download manually IPython from [GitHub](http://github.com/ipython/ipython/releases) or [PyPI](http://pypi.python.org/pypi/ipython) and to install one of these versions, unpack it and run the following from the top-level source directory using the Terminal:

    pip install .

After installation done, If you want to start interative python mode, please run below command
   
    jupyter notebook

If you want to have a look, how IPython looks like, please visit [IPython Sample](https://jupyter.org/try).

## Execution of Python programs

Python files has extension as **.py**.

Open IPython notebook or python IDE and create a new file named as first.py and then add below code to it.

      print "Hello World!"

save the file and run the file as below 
      
      python first.py

Great..! you see your first Python progam as "Hello Word!".

### Content

* [Data types](#data-types)
* [Functions](#functions)
* [Packages](#packages)


### Data types

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

    "I will eat " + str(3) + " bananas and " + str(2) + " apples"  => I will eat 3 bananas and 2 apples


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

list[startingIndex:endingIndex] => it gives us the values in list from given starting position to the endingIndex position. Remember, it doesn't include endingIndex element. It means, The start index will be included, while the end index is not.

      areas[2:8]  => This will give you values from second index position to 8th position.

      areas[:4] => this results values from 0th index to 4th index.

      areas[3:] => this results values from 3rd index to last index in list.

Look at below examples on how to read the range of values from lists.

      print(areas[0:3])  => will print ==> ['hallway', 11.25, 'kitchen']

      print(areas[3:6])  => will print ==> [18.0, 'living room', 20.0]

      print(areas[:3])  => will print ==> ['hallway', 11.25, 'kitchen']

      print(areas[3:])  => will print ==> [18.0, 'living room', 20.0, 'bedroom', 10.75, 'bathroom', 9.5]

Accessing Sublists in a list:

      house[-1][1]

      print(house[-1][1]) => 9.50

      print(house[1][1]) => 18.0

      print(house[3][1]) => 10.75

Manipulating List:

- Updating a specific position element :

      areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

- Updating 9th index and 4th index elements in this 'areas' list.

      areas[9]=10.50
      areas[4]="chill zone"

      print(areas) => ['hallway', 11.25, 'kitchen', 18.0, 'chill zone', 20.0, 'bedroom', 10.75, 'bathroom', 10.5]

- Add more elements to the existing list

      areas_1= areas + ["poolhouse", 24.5]

      areas_2 = areas_1 + ["garage" , 15.45]

- Delete elements from list:

      areas = ["hallway", 11.25, "kitchen", 18.0, "chill zone", 20.0, "bedroom", 10.75,"bathroom", 10.50, "poolhouse", 24.5, "garage", 15.45]

Now, we are removing "poolhouse", 24.5 elements from list

      del(areas[-4:-2]) or  del(areas[10:12]) will do same operation.

      print(areas)

      ['hallway', 11.25, 'kitchen', 18.0, 'chill zone', 20.0, 'bedroom', 10.75, 'bathroom', 10.5, 'garage', 15.45]


### Functions:
Functions are useful for reusing the code and maintaining the code properly. There are plenty of inbuilt functions that we can use for different purposes. For example, len() for calculating the length of arguement, type() useful for finding the data type of parameter, int(data) method to convert given data to integer type.

    # Create lists first and second
    first = [11.25, 18.0, 20.0]
    second = [10.75, 9.50]

    len(first)  => 2

    type(first) => list

    int(10.45) => 10

There are many functions like  sorted(), round()..etc

      # Paste together first and second: full
      full = first + second

      # Sort full in descending order: full_sorted
      full_sorted = sorted(full,reverse = True)

      # Print out full_sorted
      print(full_sorted)  ==> [20,0,18.0,11.25,10.75,9.50]

Reading index of arrays by inbuilt functions :

      # Create list areas
      areas = [11.25, 18.0, 20.0, 10.75, 9.50]

      # Print out the index of the element 20.0
      print(areas.index(20.0))  ===> 1

      # Print out how often 9.50 appears in areas
      print(areas.count(9.50))   ===> 1

### Packages:

Packages are useful to organising the related classes in to groups. There are different possible ways of importing a python packages.

If you want to include full package, then add import statement as below.
     # Import the math package
       import math
       
       call function as  ==>  math.pi() in code

If you want to include a specific function from a package, then add import statement as below.
      # Import radians function of math package
        from math import radians
        
        call function as  ==>  radians(value)

If you want to include a specific sub package from a package, then add import statement as below.
      
      # Import linang sub package from scipy  as my_inv
        from scipy.linalg import inv as my_inv
       
        call function as  ==>  my_inv([[1,2], [3,4]])

That's good enough to work on functions.

### References:

You can read more from https://docs.python.org/3/contents.html.


Thanks for your time.  Look out for updates on this page for more content.

Hope you enjoy this journey of mastering Python.
