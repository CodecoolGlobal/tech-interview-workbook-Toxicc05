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
#### How do you find a max value in a list/array if you can’t use any built-in functions?
#### How do you find the average of values in a list/array if you can’t use any built-in functions?
#### What do we call an *in-place* sort?
#### Explain an algorithm which sorts a list!

### Programming paradigms - procedural

#### What is the call stack?
#### What is “Stack overflow”?
#### What are the main parts of a function?

### Programming languages - Python  
#### How do you use a dictionary in Python?
#### What does it mean that an object is immutable in Python?
#### What is conditional expression in Python?
#### What are different types of arguments in Python?
#### What is variable shadowing? (context: variable scope)
#### What can happen if you try to delete/drop/add an item from a List, while you are iterating over it in Python?
#### What is the "golden rule" of variable scoping in Python (context: LEGB)? What is the lifetime of variables?
#### If you need to access the iterator variable after a for loop, how would you do it in Python?
#### What type of elements can a list contain in Python?
#### What is slice operator in Python and how to use?
#### What arithmetic operators (+,*,-,/) can be used on lists in Python? What do they do?
#### What is the purpose of the in and not in membership operators in Python?
#### What does the + operator mean when used with strings in Python?
#### Explain f strings in Python?
#### Name 4 iterable types in Python!
#### What is the difference between list/set/dictionary comprehension and a generator expression in Python?
#### Does the order of the function definitions matter in Python? Why?
#### What does unpacking mean in Python?
#### What happens when you try to assign the result of a function which has no return statement to a variable in Python?

## Software engineering

### Debugging

#### What techniques can you use while debugging a program in Python?
#### What does step over, step into and step out mean while using the debugger?
#### How can you start to debug a program from a certain line using the debugger?

### Version control

#### What are the advantages of using a version control system?
#### What is the difference between the working directory, the staging area and the repository in git?
#### What are remote repositories in git?
#### Why does a merge conflict occur?
#### Through what series of commands could you put a new file into a remote repository connected to your existing local repository?
#### What does it mean atomic commits and descriptive commit messages?
#### What’s the difference between git and GitHub?

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
Make Directory, Remove, Show file content, Copy, Make a new empty file
#### How can you look up what does a command do in Linux if you have no internet connection?
using --help
#### What does the following commands do: head, tail, more, less?
by default, it displays the first 10 lines of a file, tail displays the last 10 lines of a file, the more command displays a percentage more of the file, the less command displays a percentage less of the file
#### How do you download a file from internet using the terminal?
Using the wget command then puting in the url or in case of multiple urls 