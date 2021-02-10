# Programming Basics questions

## Computer science

### Data structures

#### What is the purpose of a list (array in some programming languages) data structure? Name some methods of it!
We use lists when we want to store objects in a way that we can access them.
A lists element can be accessed via the elements index number.
The index number starts from 0 so if we want to access the list's first element then we have to reffer to it as list[0].

#### What is the difference between a list/array and a set?
An array is an ordered pool of objects and the objects inside can be reffered by their index, or place in the list.
A set is unordered and it's objects cannot be reffered to by indexing.

#### What is the purpose and methods of a dictionary/map data structure?
The purpose of a dictionary is similar to a normal, language dictionary, translation between input and interpretation
When we create a dictionary we give a value (a key) that will be inputted and a value that the key should return
Creation of a dictionary: mydict = {'key1':'value1', 'key2':''value2}

### Algorithms

#### Fibonacci sequences. Write a method (or pseudo code), that generates the Fibonacci sequences!
def main():
    length = 8
    prev_num1 = 1
    prev_num2 = 1
    for x in range(length):
        next_num = prev_num1 + prev_num2
        print(f"{next_num} {prev_num1} {prev_num2}")
        prev_num1 = prev_num2
        prev_num2 = next_num


main()

#### How do you find a max value in a list/array if you can’t use any built-in functions?
def main():    
    maxnum = 0
    list = [666, 111, 999, 555, 888]
    for number in list:
        if number > maxnum:
            maxnum = number
    print(maxnum)


main()

#### How do you find the average of values in a list/array if you can’t use any built-in functions?
def main():    
    sum = 0
    list = [100, 900, 1000]
    for num in list:
        sum += num
    avg = sum / len(list)
    print(avg)


main()
    
#### What do we call an *in-place* sort?
An in-place sorting algorithm sorts values without the need of auxillary data structures.
This helps to keep memory usage at a minimum.

#### Explain an algorithm which sorts a list!
It takes a value from a list and swaps it with another in the same list based on parameters we gave it.

### Programming paradigms - procedural

#### What is the call stack?
It's a data structure that stores information about the active subroutines of a computer program.

#### What is “Stack overflow”?
A stack is a bank of memory that the program utilizes.
A stack overflow occurs when the programs demands exceeds the bank of memory that is available for it.
It's often the result of faulty programming and/or infinite loops.

#### What are the main parts of a function?
*The function name 
*The arguments 
*The algorithm itself

def 'function name'('the argument'):
    'the algorithm'
    'the algorithm'
    'the algorithm'
    'the algorithm'

### Programming languages - Python

#### How do you use a dictionary in Python?
Making a directory: dict = {key:value}
Referencing keys value in dictionary: dict[x] (gives back the value by default)
Referencing key in dictionary: dict[x].key() (gives back the key)

#### What does it mean that an object is immutable in Python?
The object's state cannot be modified after declaring it.
Strings and other concrete objects are typically expressed as immutable.

#### What is a conditional expression in Python?
Conditional expressions return different values based on the result of a boolean expression specified by the programmer.
The result of the boolian expression is either True or False.

#### What are different types of arguments in Python?
*Default arguments = argument has no value specified by default and requires another variable inside the program to get itself a value.
*Keyword arguments = has value by default, can only be specified after the default arguments and never before them.
*Variable length arguments = the ammount of arguments is not static.
*Variable length keyword arguments = the ammount of arguments is not static, but the value of the arguments is static.
*Command-line arguments = the arguments value is declared when starting the program in a command-line, like the linux terminal.

#### What is variable shadowing? (context: variable scope)
A variable declared within a certain scope has the same name as a variable declared in an other scope

#### What can happen if you try to delete/drop/add an item from a List, while you are iterating over it in Python?
Add: The iteration continues without an issue, albeit with different ammount of elements.
Delete/Drop: The program breaks with an index error.

#### What is the "golden rule" of variable scoping in Python (context: LEGB)? What is the lifetime of variables?
The lifetime of variables are only in their own respective scopes.
The same variable name can be used between two different definitions.

#### If you need to access the iterator variable after a for loop, how would you do it in Python?
I'd define it outside the for loop first, then iterate it inside the for loop.
By doing this I make the object operate on a larger scope than the for loop.
This object then can be used outside that for loop.

#### What type of elements can a list contain in Python?
*Strings
*Characters 
*Integers 
*Boolians
*Other lists, dictionaries, or sets

#### What is slice operator in Python and how to use?
':' is the slice operator.
The slice operator returns a slice of a list/set/dictionary.
a[0:2] = returns the first and second element of the 'a' list. (the second argument is the uppermost limit and is not included in the return value)
a[0:-1] = returns all elements except the last one of the 'a' list.
a[::-1] = returns a reversed list.
a[::2] = skips every second element of the list

#### What arithmetic operators (+,*,-,/) can be used on lists in Python? What do they do?
'+' adds to the value of the variable in the list element or joins two lists together or adds a string into a list character by character or by itself.
'*' multiplies the value in the list element or multiplies the number of list elements themselves or multiplies the ammount of list elements.
'-' substracts from the list elements value.
'/' divides the list elements value.

#### What is the purpose of the in and not in membership operators in Python?
'in' checks if a value is inside a list/set/dictionary. 
'not' is a negation statement, and it checks if the value is NOT equal to the control value.

#### What does the + operator mean when used with strings in Python?
The '+' operator is used to add characters or other strings at the end of strings or to join multiple strings together.

#### Explain f strings in Python?
f-strings are strings that contain the value of a variable in them and thus making them dynamic.
game = Pokemon GO!
example: f"I play {game} every day!\nI play {game}!"
f-strings are easier to make dynamic texts with than with using the traditional '+' operator.

#### Name 4 iterable types in Python!
*Strings 
*Lists 
*Sets 
*Dictionaries

#### What is the difference between list/set/dictionary comprehension and a generator expression in Python?
Lists, sets and dictionaries can be mentioned by themselves. (printed out) 
Generator expressions can only be reffered to in loops. (printed out)

#### Does the order of the function definitions matter in Python? Why?
Yes, it matters if you want to use one function inside another.
Then the inner function must be defined before the outer definition.

#### What does unpacking mean in Python?
Unpacking is a way in wich arguments can be given to a function from a list/set/dictionary.
Unpacking is done via the '**' operator.
example:
    def asd(a, b, c):
        print(a, b, c)
    
    d = {'a':2, 'b':4, 'c':10}
    
    asd(**d) <------this means the arguments from left to right are equal to the 'd' dictionaries elements from left to right.
    
output = 2 4 10
Unpacking too many arguments result in an argument overflow.

#### What happens when you try to assign the result of a function which has no return statement to a variable in Python?
The resulting variables value will become NULL (empty)

## Software engineering

### Debugging

#### What techniques can you use while debugging a program in Python?
Use the built in debugger from the IDE.
Read between the code and try to figure out the problem on my own.
Print out the variables (this is similar to using the IDEs debugger).
#### What does step over, step into and step out mean while using the debugger?
Step over steps over the next line or loop in the code.
Step into steps into definitions or loops.
Step out does the opposite that step into does.
#### How can you start to debug a program from a certain line using the debugger?
You can place break points in the IDE at the line you want to start debugging at.
Breakpoints stop the running of the code while using the built in debugger tool.

### Version control

#### What are the advantages of using a version control system?
You can easily backtrack if you break something in the code that you don't necessarily know the solution for.
#### What is the difference between the working directory, the staging area and the repository in git?
Working directory is the current active directory that you modify.
Staging area contains the branches that you work on.
The repository contains all the branches including the staging area and the working directory.
#### What are remote repositories in git?
Remote repositories are repositories that are not on the computer you are working on.
#### Why does a merge conflict occur?
When your instance of the repository is outdated.
To fix merge conflicts you must update your instance using the git pull command, then handle the conflicts in the IDE.
#### Through what series of commands could you put a new file into a remote repository connected to your existing local repository?
git add 'file.extension'
git commit -m 'commit message'
git push
#### What does it mean atomic commits and descriptive commit messages?
Atomic commit means a set of distinct changes as a single operation.
If the changes are applied, then the atomic commit is successful.
If there's an error while the changes are applying, then all of the atomic commits changes are reversed.
Descriptive commit messages are those that accurately describe the changes commited to the file.

#### What’s the difference between git and GitHub?
Git is a repository manager software where everyone has the repository stored locally at the same time.
Github is a website for monitoring git projects, commits, and branches inside the repository

## Software design

### Clean code

#### What does clean code mean?
The code is efficient with it's methodology when executed.
The code is easily readable and modifiable by the programmer.
Repeating parts of the code are defined separately as functions.

#### What steps do we usually do during a clean code refactoring?
We look for bloated bits of code or something that is used multiple times, then we write it to be more efficient for example, by writing a function to the code that is used multiple times.
Bloated code is code that is unnecessarily complicated, hard to read, has repeating sequences or is generally not efficient when executed.
We separate what we can in different functions.(when said part of the code is repeatedly used)

### Error handling

#### What is exception handling?
Exception handling is the process of responding to the occurrence of exceptions. (Anomalous or exceptional conditions requiring special processing)

#### What are the basics of exception handling in Python?
Understanding the origin of the error the exception caused. (The error code is usually written out by the IDE uppon error, but you still have to understand what it means.)
Knowing where the exception may have occured. (This is also usually written out by the IDE uppon error)
Knowing how to handle the exception. (Knowing what process to write to when addressing the exception)

#### In which case should we catch an exception? Why?
When it is prompt to break our program.

#### What can/should we do with an exception in the ‘except’ block?
Write an error message on what part of the program had had an unhandled exception
Offer another input opportunity uppon error.

#### What does the else and finally statement do in a try-except block in Python?
Else is called when nothing went wrong. 
Finally is called once the try-except is finished.

## Software Development Methodologies

#### What is the main goal of a retrospective meeting?
To reflect on what had happened so far in the team.
To consult with team members about their experiences working.
To reflect on the parts that needs to be worked on on a team member.

## Programming environment

### Unix

#### What is UNIX and what is Linux?
UNIX is an operating system meant to be easier to handle for programmers than conventional operating systems in the 1970's.
Linux is a freeware OS based on UNIX made by Linus Torvalds and currenty maintained and updated by the Linux community.

#### What do we call the shell in Linux?
A Shell is a command interpreter in Linux used mainly in the Linux Terminal. 
Different shells have access to different commands in the OS.

#### What does root means in a Linux environment?
Root either means Root Directory, or in the case of privileges, it means administrator, or complete privilege with access to all commands in the OS.

#### How do you access your personal files in Linux?
Via the file browser or by the Terminal with the ls command.

#### How can you install an application in Linux?
Either from the Linux store or via the Terminal, using repositories.

#### What is package management in Linux, what are repositories?
Repositories are used to store multiple programs' addresses in them for them to be more easily downloadable.
You can install linux programs from repositories with the 'apt-get' or 'apt install' commands.
A file in a repository can either be open-source or closed-source.
Open source programs are those that are made by the linux community.
Closed-source programs are proprietary programs, for example: Drivers

#### How do you navigate in the filesystem with the command line?
*Using 'cd' then space, then the desired directory. 
*'cd ..' is then used to go back one directory. 
*'cd /' is used to instantly go to the main directory.

#### What does the following commands do: mkdir, rm, cat, cp, touch?
*mkdir = Make Directory (to make a directory)
*rm = Remove (either a file or a directory)
*cat = Show and edit file content (mostly used for text files)
*cp = Copy (either a file or a directory)
*touch = Make a new empty file (a txt file by default)

#### How can you look up what does a command do in Linux if you have no internet connection?
By using --help in Terminal after a command.
--help can be used to print helping instructions on the Terminal

#### What does the following commands do: head, tail, more, less?
By default, it displays the first 10 lines of a file
Tail displays the last 10 lines of a file
The more command displays a percentage more of the file
The less command displays a percentage less of the file

#### How do you download a file from internet using the terminal?
Using the wget command then puting in the url
In the case of multiple simoltanious downloads, wget can be used on text files with multiple links in them.