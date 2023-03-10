# **Week 7 Lab Report - Skyler Nguyen**

## Challenge Task

## Setup

1. I logged into the ieng6 server by typing *ssh cs15lwi23aiz@ieng6.ucsd.edu* into the terminal and pressed *< Enter >*.

2. Typed *ls* into the terminal and checked if lab7 was in the ieng6 directory.

3. If lab7 was in the directory:
   1. Typed *rm -r lab7* into the terminal and pressed *< Enter >*.
   2. Four questions popped up (one after the other), for each one, I typed *yes* into the terminal and pressed *< Enter >*. It looked like this:

![image](https://user-images.githubusercontent.com/122576334/221089808-74b13f13-82d8-4800-acfb-e08a6d541819.png)

4.  To unfork the lab7 repository, I logged into github on the website, clicked my profile picture on the topright corner, clicked 'Your repositories', clicked on 'lab7', clicked on settings, scrolled all the way down, clicked 'Delete this repository', typed skn0012/lab7, and clicked 'I understand the consequences, delete this repository'. The page before deleting the repository looked like this:

<img width="599" alt="image" src="https://user-images.githubusercontent.com/122576334/221090923-44aea006-2801-418f-90ff-1d22a09fa570.png">

5. To fork the lab7 repository, I went to [this](https://github.com/ucsd-cse15l-w23/lab7) repository, clicked 'Fork', and 'Create fork'.

## Challenge

1. I logged into the ieng6 server by typing *ssh cs15lwi23aiz@ieng6.ucsd.edu* into the terminal and pressing *< Enter >*.

2. To clone the repository:
   1. I went to the forked repository page done in **Setup**, clicked 'Code', clicked 'SSH', then copied the key. The page looked like this and the string circled in red is what I copied: <img width="674" alt="image" src="https://user-images.githubusercontent.com/122576334/221092172-6b79fa99-be30-4519-827c-ea25c851c353.png">
   2. Going back to VSCode, I typed 'git clone ', pressed *< Ctrl + V >* to paste the copied key, and then pressed *< Enter >*. The terminal looked like this: 
   
   <img width="562" alt="image" src="https://user-images.githubusercontent.com/122576334/221092863-85d4a7d1-4644-4be2-8896-76035cabf5af.png">

3. To run the test:
   1. I typed *cd lab7* and pressed *< Enter >* to change the directory to lab7.
   2. I copied and pasted 'javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java' from the Week 3 Lab page and pressed *< Enter >* to compile all the java files.
   3. Afterward, I copied and pasted 'java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore' from the same Lab page, then typed 'ListExamplesTests', and pressed *< Enter >* to run the test. This is what it looks like: 
   
   <img width="761" alt="image" src="https://user-images.githubusercontent.com/122576334/221099000-282cd64d-2bd3-4bad-b0d2-26015114926f.png">

4. To edit the file to fix the failing test:
   1. I typed *nano ListExamples.java* into the terminal then pressed *< Enter >* which opens up the ListExamples file using the nano text editor.
   2. I then held the *< Down >* key, pressed the *< Up >* key 7 times, pressed the *< Right >* key 12 times, pressed the *< Backspace >* key 1 time, and typed '2'. This fixes the failing test which was a typo in which the line is supposed to be '**index2 += 1;**' and not '**index1 += 1;**'. 
   
   * *Before:* 
   
   <img width="180" alt="image" src="https://user-images.githubusercontent.com/122576334/221100781-d436743b-74ba-4503-a138-b78babb4e726.png">
   
   * *After:*
   
   <img width="180" alt="image" src="https://user-images.githubusercontent.com/122576334/221100859-472eef2f-3c58-4231-a04c-3440c5ddfd69.png">

   3. Afterward, I pressed *< Ctrl + O >*, pressed *< Enter >*, then pressed *< Ctrl + X >*. This saves the changes to the file and closes the nano editor.

5. To run the test after fixing the mistake:
   1. Since I compiled the java files before this, I pressed the *< Up >* key 3 times and pressed *< Enter >* to compile the tests.
   2. Then, I ran the test by pressing the *< Up >* key 3 times and pressed *< Enter >*. This is what it looks like:
   
   <img width="757" alt="image" src="https://user-images.githubusercontent.com/122576334/221101937-4679f15f-ae48-458a-a164-621bafeb1f57.png">

6. To commit and push the changes to Github:
   1. I typed *git add ListExamples.java* and pressed *< Enter >* to the staging area to be committed.
   2. Afterward, I typed *git commit -m "Fixed"* and pressed *< Enter >* to commit the changes.
   3. Lastly, I typed *git push origin main* and pressed *< Enter >* to push the changes to the Github repository. This is what it looks like after doing that:
   
   <img width="385" alt="image" src="https://user-images.githubusercontent.com/122576334/221103002-ac034022-76c1-409d-9f1c-ec40c8b077c9.png">
   
## Some before and after screenshots

* Original:

<img width="660" alt="image" src="https://user-images.githubusercontent.com/122576334/221103320-d8195adc-e636-4e2e-bae0-bbbe347df1ad.png">

* After changes:

<img width="661" alt="image" src="https://user-images.githubusercontent.com/122576334/221103391-3925bc11-b9bb-41b1-8bfb-7d1f863e2b3e.png">

* Original file:

<img width="212" alt="image" src="https://user-images.githubusercontent.com/122576334/221103580-0a505e15-2673-4cc5-b245-9a58f84743dd.png">

* After changes:

<img width="214" alt="image" src="https://user-images.githubusercontent.com/122576334/221103722-ea55d02d-8ad8-4562-8e2c-e86f65bf53c6.png">








