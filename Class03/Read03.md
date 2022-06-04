# What is Python File Handling?
File handling is basically the management of the files on a file system. Every operating system has its own way to store files.

Python File handling is useful to work with files in our programs. We don’t have to worry about the underlying operating system and its file system rules and operations.

[Operations ](File-operations.png.webp)

1. open() function
The open() function is used to open a file in a particular mode.
It basically creates a file object which can be used for further manipulations.

Syntax:


  open(file_name, mode) 
  Different modes for opening a file:

r: Read
w: Write
a: Append
r+: Read and Write
Initially, we need to create a file and place it in the same directory as of the script.

Demo.txt

 Welcome to the programming world!
 Execute_file.py


 demo_file = open('Demo.txt', 'r')
## This statement will print every line in the file
for x in demo_file:
    print (x)
 
## close the file, very important
demo_file.close()
Output:

Welcome to the programming world!
Here, the Execute_file.py script opens the Demo.txt file and prints the entire content line-by-line.


2. read() function                         used to read the  contents of the file. To  achieve the same,  we need to open a file  in the read mode.
   demo_file = open("Demo.txt", "r")
    print(demo_file.read())
    demo_file.close()
   Output:
   Welcome to the programming world!
3. write() function
The write() function is used to write to a
 file and make changes to it.

  demo_file = open('Demo.txt','w')

    demo_file.write("Hello Everyone!.\n")
    demo_file.write("Engineering  Discipline.")
    demo_file.close()
    Output: When we open the Demo.txt file, we can see the changes reflected here.
    Hello Everyone!.
    Engineering Discipline.


4. append() function
   
 demo_file = open('Demo.txt','a')
 
    demo_file.write("\nStatement added to the  end of the file..")
    demo_file.close()
     Output:

     Hello Everyone!.
     Engineering Discipline.
    Statement added to the end of the file..
5. split() function
The split() function is used to split lines within a file. It splits up as soon  as it encounters space in the script.

    Demo.txt
     Hello Everyone!.
      Engineering Discipline.
      Statement added to the end of the file..
 Execute_file.py


with open("Demo.txt", "r") as demo_file:

    demo_data = demo_file.readlines()
    for line in demo_data:
        result = line.split()
        print(result)
     Output:
     ['Hello', 'Everyone!.']
     ['Engineering', 'Discipline.']
     ['Statement', 'added', 'to', 'the', 'end', 'of', 'the', 'file..']
6. close() function
The close() function is used to close a particular file post manipulations on it.

After writing to a file, if we do not call the close() method, all the data written to the file will not be saved in it.

It’s always a good idea to close the file after we are done with it to release the resources.

Syntax:

file-name.close()

7. rename() function
The os module provides the rename() method to change the name of the particular file.
Syntax:
os.rename(current_name,new_name)

8. remove() method
The os module provides the remove() method to delete the file given as input.

import os
os.remove('Demo.txt')
Before executing the remove() method..

Delete A File
Before remove()
Output: After executing the remove() method


After Remove
After remove()
Conclusion
Thus, in this article, we have understood the File operations in Python.


