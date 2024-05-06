# Lab Report 3
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
<img width="917" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/c5f61195-ae24-44cb-b440-86cdbfc05b40"> \n
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
