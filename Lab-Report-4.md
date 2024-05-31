# Lab Repot 4
## Step 4
 <img width="416" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/12908f1d-de11-4d9c-b27b-8195792e1380"> \
 * `ssh <space> dbarnhardt@ieng6.ucsd.edu <enter>`
 * `ssh` is saying I want to log into a secure shell and after that is my username for the ieng6 machine. Then I hit <enter> to run the command and I do not need to type in a password because I delt with that in a previous lab.
## Step 5
 <img width="429" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/18434c82-07ab-4c09-8728-1e3045b8be54"> \
* `git <space> clone <space> crtlV`
* `git` is saying that it is a `git` command. `clone` is cloning a repository onto the ieng6 machine. And the url is the url of the repository I am cloning. I pasted the url to the repo with `ctrl v`.
## Step 6
<img width="499" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/86a6650b-fd5c-4407-8d66-084f1c969dfe"> \
* `cd <space> l <tab> <enter>`
   `bash <space> t <tab>`
* `cd` changes directories and `lab7` is the directory I want to change into then enter to change into it. Then `bash` runs a script so run multiple lines of code at once and `test.sh` is a script that compiles and runs and runs the junit tests. I used tab so I didnt have to type the whole name of the file/directory and instead let the computer complete it. 
## Step 7
<img width="402" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/929b6206-4de0-4404-b1d6-64273b275ca7"> \
* `vim <space> Li <tab> . <tab> <enter>` \
`<down>x44 w w <left>x2 r2 :wq <enter>` \
* `vim` with a file, here I typed the first letters and filled it in with tab, will open up a file in `vim` editor when I hit enter. Then I held the down arrow until I got to the line I wanted to change. Then I hit `w` twice to get to the start of the word after the one I wanted to chnage. Then I hit the left arrow to get to the character I wanted to change. Then I hit `r` for replace and 2 as the thing I wanted to replace it with. Then `:wq` after you hit enter saves and exits the `vim` editor. 
## Step 8
 <img width="342" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/920c25d5-4b66-4b04-aa25-fbe595519ef1"> \
* `<up>` `<up>` `<enter>` 
* Hitting the up arrow once brings you to the last command you ran. Hitting it again brings you to the one before that, for me that was the correct command. And after I reached the correct command I hit enter and it is the same file ran with `bash` to run the junit tests. 
## Step 9
<img width="410" alt="image" src="https://github.com/coda289/cse15l-lab-report/assets/148298382/248d73f3-470e-4ae2-b1a6-7526fecd856c"> \

* `git <space> add <space> . <enter>` 
* `git <space> com<tab> -m <space> "fix <space> index" <enter>` \
* `git <space> push <space> o<tab> m<tab> <enter>` \
* `git add .` this will add the files to the repository and the period serves as a wildcard \
   the next line it to commit your changes and lock them into place in addition to adding a message that wil go along with the changes. I chose fix index because that is what i did. \
   the next line pushes the actual changes onto git hub.
