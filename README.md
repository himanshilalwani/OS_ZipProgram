# OS Project 4

### Authors: Avani Tiwari, Himanshi Lalwani

Invoking the program:
- make
- ./adzip {-c|-a|-x|-m|-p} <archive-file> <file/directorylist> 	

Note that <file/directorylist> is a comma separated string of files and directories to be zipped.

Example Usage:
- make
- ./adzip {-c|-a|-x|-m|-p} adzip.ad text.txt,testDir,test.png

Overview:
The users can call the adzip program to archive files and directories which can be provided as a comma separated list in the <archive-file> provided. 
For extracting, printing the hierarchy, and printing the metadata we can just need the <archive-file> 			

-c store in the archive file <archive-file> (appropriately designated with postfix.ad), all files and/or directories provided by the list <file/directory-list>. If other files/directories exist within in <directory-list>, then all this content is recursively stored in the <archive-file>.			
-a append filesystem entities (files and directories) indicated in the <file/directory list> in the archived file <archive-file> that already exists. If additional files and directories exist in <file/directory list>, they are also recursively appended along with their content in the designated <archive-file>.				
-x extract all files and catalogs that have been archived in file <archive-file> by accurately recreating the original hierarchy in the current working directory. The folder in which the contents are extracted is called extract.			
-m print out the meta-data (owner, group, rights) for all files/directories that have been archived in <archive-file>.					
-p display the hierarchy(-ies) of the files and directories stored in the <archive-file>.
