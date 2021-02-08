# Programming Basics questions

## Computer science

### Data structures

#### What is the purpose of a list (array in some programming languages) data structure? Name some methods of it!
we use lists when we want to store objects in a way that we can access them.
#### What is the difference between a list/array and a set?
an array is an ordered pool of objects and the objects inside can be reffered by their index, or place in the list, a set is unordered and it's objects cannot be reffered to by indexing.
#### What is the purpose and methods of a dictionary/map data structure?
translation between input and interpretation by the computer
### Algorithms

#### Fibonacci sequences. Write a method (or pseudo code), that generates the Fibonacci sequences!
fibonachi = empty_list
for x in range limit:
    if x is 0:
        fibonachi.append 0
    elif x is 1:
        fibonachi.append 1
    else:
        fibonachi.append fibonachi[x-1] + fibonachi [x-2]

#### How do you find a max value in a list/array if you can’t use any built-in functions?
maxnum = 0
for number in list:
    if number > maxnum:
        maxnum = number
return maxnum

#### How do you find the average of values in a list/array if you can’t use any built-in functions?
sum = 0
for num in list:
    sum += num
avg = sum / len(list)
return avg
    
#### What do we call an *in-place* sort?
The in-place algorithms are those that don't need any auxiliary data structure in order to transform the input data.
#### Explain an algorithm which sorts a list!
It takes a value from a list and swaps it with another in the list based on parameters we gave it.
### Programming paradigms - procedural
the program executes itself in an orderly manner
#### What is the call stack?
it's a data structure that stores information about the active subroutines of a computer program.
#### What is “Stack overflow”?
A programmer's best friend (a website)
#### What are the main parts of a function?
the function name, the prerequisites, the algorithm

### Programming languages - Python

#### How do you use a dictionary in Python?
dict = {key:value}
dict[x] (gives back the value by default)
dict[x].key() (gives back the key)
#### What does it mean that an object is immutable in Python?
the object's state cannot be modified after declaring it
#### What is a conditional expression in Python?
if, elif, else
#### What are different types of arguments in Python?
keyword arguments, default arguments, variable length arguments, variable length keyword arguments
#### What is variable shadowing? (context: variable scope)
a variable declared within a certain scope has the same name as a variable declared in an outer scope
#### What can happen if you try to delete/drop/add an item from a List, while you are iterating over it in Python?
the program crashes
#### What is the "golden rule" of variable scoping in Python (context: LEGB)? What is the lifetime of variables?
the lifetime of variables are only in their own respective scopes, the same variable name can be used between two different definitions
#### If you need to access the iterator variable after a for loop, how would you do it in Python?
i'd define it outside the for loop first
#### What type of elements can a list contain in Python?
strings, integers, boolians and other lists
#### What is slice operator in Python and how to use?
#### What arithmetic operators (+,*,-,/) can be used on lists in Python? What do they do?
'+' adds to the value of the variable in the list element, '*' multiplies the value in the list element or multiplies the list itself, '-' substracts from the list element
#### What is the purpose of the in and not in membership operators in Python?
'in' checks if a value is inside a variable, 'not' checks if a value is different fron the control value.
#### What does the + operator mean when used with strings in Python?
the '+' operator is used to add characters or other strings at the end of strings
#### Explain f strings in Python?
f strings are strings that contain the value of a variable in them
#### Name 4 iterable types in Python!
strings, lists, sets, dictionaries
#### What is the difference between list/set/dictionary comprehension and a generator expression in Python?
lists, sets, dictionaries can be mentioned by themselves, generator expressiosn can only be reffered to in loops
#### Does the order of the function definitions matter in Python? Why?
Yes, if you want to use one function inside another.
#### What does unpacking mean in Python?
printing out variables
#### What happens when you try to assign the result of a function which has no return statement to a variable in Python?
you get NULL
## Software engineering

### Debugging

#### What techniques can you use while debugging a program in Python?
I can use debugger, or read between the code, or print out variables
#### What does step over, step into and step out mean while using the debugger?
step over steps over the next command, step into steps into definitions, step out does the opposite
#### How can you start to debug a program from a certain line using the debugger?
you can place break points

### Version control

#### What are the advantages of using a version control system?
You can easily backtrack if you break something in the code
#### What is the difference between the working directory, the staging area and the repository in git?
working directory is the current active directory that you modify, staging area contains the branches, the repository contains it all
#### What are remote repositories in git?
remote repositories are repositories that are not on your computer
#### Why does a merge conflict occur?
Your verion of the repository is outdated
#### Through what series of commands could you put a new file into a remote repository connected to your existing local repository?
git commit
git push
#### What does it mean atomic commits and descriptive commit messages?
atomic commit means a single large change in the file, descriptive commit messages are those that accurately describe the changes commited to the file
#### What’s the difference between git and GitHub?
git is a repository manager software where everyone has the repository locally, github is a website for monitoring git projects, commits, and branches

## Software design

### Clean code

#### What does clean code mean?
the code is efficientwith it's methodology and easily readable and modifiable
#### What steps do we usually do during a clean code refactoring?
we look for bloated bits of code or something that is used multiple times, then we write it to be more efficient for example, by writing a function to the code that is used multiple times.

### Error handling

#### What is exception handling?
Handling cases where the input is outside the acceptable ranges.
#### What are the basics of exception handling in Python?
try
#### In which case should we catch an exception? Why?
When it is prompt to break our program.
#### What can/should we do with an exception in the ‘except’ block?
either write an error message, or offer another input opportunity until it is within range
#### What does the else and finally statement do in a try-except block in Python?
else is called when nothing went wrong, finally is called once the try-except is finished

## Software Development Methodologies

#### What is the main goal of a retrospective meeting?
to reflect on what had happened so far in the team
## Programming environment

### Unix

#### What is UNIX and what is Linux?
UNIX is an operating system meant to be easier to handle for programmers than conventional operating systems in the 1970's, Linux is a freeware OS based on UNIX made by Linus Torvalds and currenty maintained and updated by the Linux community.
#### What do we call the shell in Linux?
A Shell is a command interpreter in Linux used mainly in the Linux Terminal, different shells have access to different commands in the OS.
#### What does root means in a Linux environment?
Root either means Root Directory, or in the case of privileges, it means administrator, or complete privilege with access to all commands in the OS.
#### How do you access your personal files in Linux?
in 'Files'
#### How can you install an application in Linux?
Either from the Linux store or from the Terminal, using repositories.
#### What is package management in Linux, what are repositories?
repositories are used to store multiple programs' adresses in them for them to be more easily downloadable.
#### How do you navigate in the filesystem with the command line?
Using 'cd' then space, then the desired directory. 'cd ..' is then used to go back one directory. 'cd /' is used to instantly go to the main directory.
#### What does the following commands do: mkdir, rm, cat, cp, touch?
Make Directory, Remove, Show and edit file content, Copy, Make a new empty file
#### How can you look up what does a command do in Linux if you have no internet connection?
using --help
#### What does the following commands do: head, tail, more, less?
by default, it displays the first 10 lines of a file, tail displays the last 10 lines of a file, the more command displays a percentage more of the file, the less command displays a percentage less of the file
#### How do you download a file from internet using the terminal?
Using the wget command then puting in the url or in case of multiple urls 