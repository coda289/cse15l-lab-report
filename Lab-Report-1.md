# Lab Report 1
## `cd` examples
1. **no arguments**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ cd

   dakot@DESKTOP-2TDL2AN MINGW64 ~
   ```
   **absolute path:** `/c/Users/dakot/lecture1`

   Because I had no ements there was no output but the directory changed to my home directory.

   It is not an error because the code has no output and executed correctly

2. **path to directory**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~
   $ cd lecture1

   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   ```
   **absolute path:** `/c/Users/dakot/`

   With the argument `lecture 1` I got no argument but my directory changed to `lecture 1`

   This is not an error because this is the intended use of cd. To change from one directory to the other.

3. **file as argument**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
    $ cd Hello.java
    bash: cd: Hello.java: Not a directory
    ```
   **absolute path:**/c/Users/dakot/lecture1

   The output was a message informing me that the argument `Hello.java` was not a directory

   This is an error because cd is to change to a different directiry and it is expecting a directory and not a file. It provides the error message `bash: cd: Hello.java: Not a directory`

## `ls` examples
1. **no arguments**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ ls
   Hello.class  Hello.java  messages/  README
   ```
   **absolute path:** `/c/Users/dakot/lecture1`

   The output was a list of files and directories within the directory that I am currently in. 

   This is not an error because it properly displays the output, it lists the content of the directory I am in, `lecture1`

2. **path to directory**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ ls messages
   en-us.txt  es-mx.txt  zh-cn.txt
   ```
   **absolute path:** `/c/Users/dakot/lecture1`
   
   I got the output `en-us.txt  es-mx.txt  zh-cn.txt` becuase that is the list of files that are contained within the directory `messages`.

   It is not an error because it correctly displays the files that are within the directory. 
3. **path to file**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ ls Hello.java
   Hello.java
   ```
   **absolute path:** `/c/Users/dakot/lecture1`

   I got the output `Hello.java` because there are no files within `Hello.java` because it is not a directory but instead a file so it only contains itself.

   This is not an error because this is not a directory, but a file, so the output is only itself.

## `cat` Examples
1. **No arguements**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~
   $ cat

   ```
   **absolute path:** `/c/Users/dakot`

   I got no output and this makes sense because I gave no input so it had no files to read and therefore gave no outputs.

   This is an error because no only did it have no output, but it also broke my terminal and does noy let me type anymore. This makes sense because I told the terminal to print out a file and then provided no files.

2. **path to directory**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1 (main)
   $ cat messages
   cat: messages: Is a directory
   ```
   **absolute path:** `/c/Users/dakot/lecture1`

   I got an error message as an output stating what the error is.
   
   This is an error because cat expects a file and I gave a directory so in the error message it tells me `cat: messages: Is a directory` and clearly states the issue.

3. **path to file**
   ```
   dakot@DESKTOP-2TDL2AN MINGW64 ~/lecture1/messages (main)
   $ cat zh-cn.txt
   你好世界
   ```
   **absolute path:** `/c/Users/dakot/lecture1/messages`

   I got `你好世界` as an output becuase that is what is contained within the file `zh-cn.txt`

   This is not an error because it correctly displays what is contained in the file
