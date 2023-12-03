Real Hard Death Smack 
coded by RobotMonkeyHead in QBasic 4.5 in 1996-97

Remove the .txt part of the file names, so they're just .bas files.
Use Qbasic 4.5 to run them, if you wish.

In order to enable the custom fighter maker to work, you have to open
both .bas files and search for:

#THIS IS WHERE YOU EDIT THE CUSTOM CHARACTER'S FILE NAME

Directly below that, you'll find the variables TheDirectory$ and custom$
both followed by empty sets of quotation marks, which need to be filled in.
The directory variable should go from your root directory to the folder the 
character file is stored in.  Here is an example of how the program uses them:

delete file "C:\" + TheDirectory$ + Custom$ + ".max"

Custom$ is the name of the character file, and TheDirectory$ is the name of
the directory it's in.