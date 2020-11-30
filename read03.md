
# Read 3

## Reading and Writing Files in Python

-One of the most common tasks that you can do with Python is reading and writing files. Whether it’s writing to a simple text file, reading a complicated server log, or even analyzing raw byte data, all of these situations require reading or writing a file.

-A file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

-Files contain of:

Header: metadata about the contents of the file (file name, size, type, and so on)

Data: contents of the file as written by the creator or editor

End of file (EOF): special character that indicates the end of the file

-What this data represents depends on the format specification used, which is typically represented by an extension.

-When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)

File Name: the actual name of the file

Extension: the end of the file path pre-pended with a period (.) used to indicate the file type

-A common problem that you may face is the encoding of the byte data. An encoding is a translation from byte data to human readable characters. This is typically done by assigning a numerical value to represent a character. The two most common encodings are the ASCII and UNICODE Formats.

-When you want to work with a file, the first thing to do is to open it. This is done by invoking the `open()` built-in function. `open()` has a single required argument that is the path to the file. `open()` has a single return, the file object:

`file = open('dog_breeds.txt')`

-Warning: You should always make sure that an open file is properly closed.

Character	Meaning

'r' =>	Open for reading (default)

'w' =>	Open for writing, truncating (overwriting) the file first

'rb' or 'wb' =>	Open in binary mode (read/write using byte data)



-There are three different categories of file objects:

Text files

Buffered binary files

Raw binary files

-There are multiple methods that can be called on a file object to help you out:



`.read(size=-1)` =>	This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.

`.readline(size=-1)` =>	This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.

`.readlines()` =>  This reads the remaining lines from the file object and returns them as a list.

-As with reading files, file objects have multiple methods that are useful for writing to a file:

`.write(string)` =>	This writes the string to the file.

`.writelines(seq)` =>	This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).

-Sometimes, you may need to work with files using byte strings. This is done by adding the 'b' character to the mode argument. All of the same methods for the file object apply. However, each of the methods expect and return a bytes object instead.

## Python Exceptions: An Introduction

-A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception.

-Syntax errors occur when the parser detects an incorrect statement.

-Exception errors occur whenever syntactically correct Python code results in an error.

-The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

- when syntactically correct code runs into an error, Python will throw an exception error. This exception error will crash the program if it is unhandled. The except clause determines how your program responds to exceptions.


-`raise` allows you to throw an exception at any time.

-`assert` enables you to verify if a certain condition is met and throw an exception if it isn’t.

-In the `try` clause, all statements are executed until an exception is encountered.

-`except` is used to catch and handle the exception(s) that are encountered in the try clause.

-`else` lets you code sections that should run only when no exceptions are encountered in the try clause.

-`finally` enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

