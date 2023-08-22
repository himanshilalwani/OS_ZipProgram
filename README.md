# adzip - Archive and Extract Utility in C

### Authors: Avani Tiwari, Himanshi Lalwani

### Overview
The adzip utility is a powerful C program designed to provide archiving and extraction capabilities for files and directories. Users can conveniently invoke this program through the command line interface. Here's a concise guide on using adzip.

### Invocation
To utilize the adzip program, follow these steps:
1. Open a terminal and navigate to the src folder within project directory using the cd command.
2. Compile the program using `make`.
3. Execute the program with one of the following options and a comma-separated list of files and directories: `./adzip {-c|-a|-x|-m|-p} <archive-file> <file/directorylist>`.

### Example Usage
As an illustration, consider the following usage scenario:<br>
`make`<br>
`./adzip {-c|-a|-x|-m|-p} adzip.ad text.txt,testDir,test.png`

### Features
The users can call the adzip program to archive files and directories which can be provided as a comma separated list in the <archive-file> provided. 
For extracting, printing the hierarchy, and printing the metadata we just need the <archive-file> arg.

The adzip program encompasses several key functionalities:
- `-c`: Store Operation
  - Archive the specified files and directories into an archive file, appropriately designated with the '.ad' postfix.
  - Recursively include all content within the provided directories.   
- `-a`: Append Operation
  - Append filesystem entities indicated in the <file/directory list> to an existing archive file.
  - Additional files and directories existing within the <directory-list> are also recursively appended to the designated archive file.
- `-x`: Extract Operation
  - Extract all archived files and directories from the archive file, meticulously recreating the original hierarchy.
  - Extraction is done in the 'extract' folder within the current working directory.
- `-m`: Metadata Printing
  - Display the meta-data (owner, group, rights) for all files/directories archived in the designated archive file. 
- `-p`: Hierarchy Display
  - Print the hierarchies of files and directories stored within the archive file.

In summary, the adzip utility serves as a versatile tool for archiving and extracting files and directories, enhancing your file management capabilities with efficiency and ease.
