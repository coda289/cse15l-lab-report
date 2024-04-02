# Lab Report 1
## `cd` examples
1. **no arguements**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ cd

   dakot@DESKTOP-2TDL2AN MINGW64 ~
   ```
   **absolute path:** `/c/Users/dakot/lecture1`

   Because I had no arguements there was no output but the directory changed to my directory.

   It is not an error because the code has no output and executed correctly

2. **path to directory**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~
   $ cd lecture1

   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   ```
   **absolute path:** `/c/Users/dakot/`

   With the argument `lecture 1` I got no arguement but my directory changed to `lecture 1`

   This is not an error because this is the intended use of cd. To change from one directory to the other.

3. **file as arguement**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
    $ cd Hello.java
    bash: cd: Hello.java: Not a directory
    ```
   **absolute path:**/c/Users/dakot/lecture1

   The output was a message informing me that the arguement `Hello.java` was not a directory

   This is an error because cd is to change to a different directiry and it is expecting a directory and not a file. It provides the erroe message `bash: cd: Hello.java: Not a directory`

##`ls` examples
1. **no arguements**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ ls
   Hello.class  Hello.java  messages/  README
   ```
   **absolute path:** `/c/Users/dakot/lecture1`

   The output was a list of files that and directories withen the directory that I am currently in

   This is not an error because it properly displays the output, it lists the connect on the directory I am in `lecture1`

2. **path to directory**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ ls messages
   en-us.txt  es-mx.txt  zh-cn.txt
   ```
   **absolute path:** `/c/Users/dakot/lecture1`

   
