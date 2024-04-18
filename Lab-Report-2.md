# Lab Report 2
## Part 1
### Code for ChatServer
<img width="464" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/78a2641c-af6f-4921-a041-8bd7c2de9ca1">
<img width="735" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/f4177859-7d19-4a2a-a564-0f0da326d62b">

### Example 1
<img width="635" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/9957886f-957f-4c0b-b22d-30cef47991ce">\
the method that is run is `handleRequest(URI url)` which also calls:
- `getPath()`
- `equals()`
- `format()`
- `getQuery`
- `split()`\
The argument is http://localhost:3030/add-message?s=Hello!%20What%20college%20do%20you%20go%20to&user=WistfulWillow as url
and the fields and local variables are
- String messages="WistfulWillow: Hello! What college do you go to"
- Strings[] news={"s=Hello! What college do you go to", "user=WistfulWillow"}
- Strings[] mess={"s","Hello! What college do you go to"}
- Strings[] user={"user","WistfulWillow"}
There is only one field, messagages, and the rest are local variables. SO the only thing that gets changes is the String messages and it gets updates to add a new message on a new line in the format  "<user>: <string>"

### Example 2
<img width="510" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/e3281916-70b7-479d-ae09-011276631188">\
the method that is run is `handleRequest(URI url)` which also calls:
- `getPath()`
- `equals()`
- `format()`
- `getQuery`
- `split()`\
The argument is http://localhost:3030/add-message?s=Hi%20I%20go%20to%20UCSD&user=ToweringTriton
and the fields and local variables are
- messages="WistfulWillow: Hello! What college do you go to '\n' ToweringTriton: Hi I go to UCSD"
- news={"s=Hi I go to UCSD","user=ToweringTriton"}
- mess={"s","Hi I go to UCSD"}
- user={"user","ToweringTriton"}
Similarly the only field that was changed not temporarily is messages now it includes my first message but it also includes a new message on the next line in the same format.  


## Part 2
### My computer
<img width="358" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/b6fea873-8bc6-4435-8ef4-0f7fd31fae7a">

### ieng6 machine
<img width="435" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/41d63a9b-cb0b-469d-bd5d-627f2fe41772">

### no password
<img width="651" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/019aea7f-91b7-4565-b55b-032e8041f3e5">


## Part 3
In labs 2 and 3 I learned a lot more about websites, inlcuding hosting them and url. Before this class I never realized you could write a program that can look at the url as an input and get different parameters to run in methods. I also learned that I can locally host a website on my computer and it will update when I give it a new path, or I could run it on the ieng6 machine and anyone on ucsd wifi can access it. 
