# Lab Report 3
## Part 1
```
interface StringChecker { boolean checkString(String s); }

class check implements StringChecker{
  public boolean checkString(String s){
    return s.contains("e");
  }
```
1. 
```
 @Test
    public void filterTest1(){
        List<String> input=List.of("hello","hi","enter");
        StringChecker e= new check();
        List<String> answer=List.of("hello","enter");
        assertEquals(answer ,ListExamples.filter(input,e) );
    }
```
2. 
```
 @Test
    public void filterTest2(){
        List<String> input=List.of("hello","ink","plow");
        StringChecker e= new check();
        List<String> answer=List.of("hello");
        assertEquals(answer ,ListExamples.filter(input,e) );
    }
```
3. 
<img width="917" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/c5f61195-ae24-44cb-b440-86cdbfc05b40"> \
4. Before
```
   static List<String> filter(List<String> list, StringChecker sc) {
    List<String> result = new ArrayList<>();
    for(String s: list) {
      if(sc.checkString(s)) {
        result.add(0, s);
      }
    }
    return result;
  }
```
After
```
 static List<String> filter(List<String> list, StringChecker sc) {
    List<String> result = new ArrayList<>();
    for(String s: list) {
      if(sc.checkString(s)) {
        result.add(s);
      }
    }
    return result;
  }
```
5. Before the code would check the list starting at element 0 and increasing, but it would add the elements to the front of the list resulting in an incorrect order. I changed it by using `.add()` with no index so it would add to the end of the list and stay in correct order.
## Part 2
`find` \
`-name` \
This will help you find the path of a specific file if you cant even remember what directory it is in. 
```
dakot@DESKTOP-2TDL2AN MINGW64 ~/Downloads/docsearch-main/technical   
$ find -name 5_Legal_Groups.txt
./government/Media/5_Legal_Groups.txt
```
It can also help you find the path of a directory too.
```
dakot@DESKTOP-2TDL2AN MINGW64 ~/Downloads/docsearch-main/technical
$ find -name plos
./plos
```
`-type` \
This helps you find all the directories within a directory. This can be helpful when you dont have a tool like vs code to help you look at them. 
```
$ find -type d
.
./911report
./biomed
./government
./government/About_LSC
./government/Alcohol_Problems
./government/Env_Prot_Agen
./government/Gen_Account_Office
./government/Media
./government/Post_Rate_Comm
./plos
```
It also works for files. You can list out every file in a certain directory so you can know the exact name if you want to cat the files
```
dakot@DESKTOP-2TDL2AN MINGW64 ~/Downloads/docsearch-main/technical   
$ find ./government/Alcohol_Problems/ -type f
./government/Alcohol_Problems/DraftRecom-PDF.txt
./government/Alcohol_Problems/Session2-PDF.txt
./government/Alcohol_Problems/Session3-PDF.txt
./government/Alcohol_Problems/Session4-PDF.txt
```
`-ls` \
If you want more information about the files you can use `-ls` this can help when theres files with similar names and you cant remember which one you just edited. 
```
dakot@DESKTOP-2TDL2AN MINGW64 ~/Downloads/docsearch-main/technical   
$ find -name "Session*" -ls
2533274790896081     36 -rw-r--r--   1 dakot    197609      35927 Apr 30 09:32 ./government/Alcohol_Problems/Session2-PDF.txt
5910974511424140     96 -rw-r--r--   1 dakot    197609      94212 Apr 30 09:32 ./government/Alcohol_Problems/Session3-PDF.txt
5348024558002878     80 -rw-r--r--   1 dakot    197609      80034 Apr 30 09:32 ./government/Alcohol_Problems/Session4-PDF.txt
```
You can also list informtion about files in a new text file for future reference
```
dakot@DESKTOP-2TDL2AN MINGW64 ~/Downloads/docsearch-main/technical   
$ find ./911report/ -name "*2.txt" -ls >> findexamples.txt
```
`-exec` \
This helps when I want to move multiple files at once. It would take a lot longer to do it one by one. 
```
dakot@DESKTOP-2TDL2AN MINGW64 ~/Downloads/docsearch-main/technical   
$ find ./911report/ -name "*2.txt" -ls >> findexamples.txt
```
This can help me run commands when I know the file name but do not know the path. I can also copy multiple files to the same file wusing this command. 
```
dakot@DESKTOP-2TDL2AN MINGW64 ~/Downloads/docsearch-main/technical
$ find -name 5_Legal_Groups.txt -exec cp {} ./copy.txt \;
```

