# File-Name-List-Project
Learned about basic file handling and put it to the test in C.


In this personal project, I wanted to relearn file handling on a basic level. The last time I worked with it was in C++, and more recently I started tackling C.
With that being said, it was refreshing to learn more about using the FILE* pointer, as well as the appending, reading, and writing modes: a (append), r (read), and w (write).
These modes are fairly self-explanatory in terms of what they accomplish in the code, but to demonstrate what I’ve learned, I’ve included an examples below.

Ex. FILE* fp = fopen("C:\..\..\..\NameList.txt", "a");

With this line, I am not only creating a file but also defining a file pointer named fp.
FILE* fp is a pointer that connects my program to the file I create.
Using fopen, I specify the file path and name (NameList.txt) and open it in append mode (a).

The append mode means that if the file does not exist, it will be created, and any new data written will be added to the end of the file rather than overwriting its contents.

When reading from the file, the process is similar, except I open it using read mode (r).
This allows me to access and display the data that was previously added.

Ex. fp = fopen("C:\..\..\..\NameList.txt", "r");

Notice how I do not write FILE* again. This is because I already declared the file pointer earlier in memory.
Here, I am simply reusing that same pointer to reference the file for reading.

With writing to the file its the exactly the same process as reading where im referencing the pointer, but this time giving the capability to delete from the file.

Ex. fp = fopen("C:\\..\\..\\..\\NameList.txt", "w");

*** NOTE ***
1. In this project there will be two lines for the File destination. Please put your file path in replacement of the place holder.
2. I'm still learning so I dont know how to make it automatic for whoever accesses this program.
3. I had to split up the viewing of the names between current session and the previous(The file's contents) betweem two different case statements, because I could not for the life of me figure it out.
