# Lab Report 4

## **Step 1: Creating Your CSE15L Account Using ieng6**
`$ ssh cs15lsp23xx@ieng6.ucsd.edu` 
You will then be prompted to insert your password like usual and type in yes. 

## **Step 2: Clone the Link**
Git clone the fork of the repository github link for the lab 7 report. 
`$ git clone https://github.com/ucsd-cse15l-s23/lab7` 

*Notice*: 
You might encounter the problem where you are not able to run the file as the terminal will display the message 
```java
    Error: Main method not found in class ListExamples, please define the main method as:
    public static void main(String[] args)
    or a JavaFX application class must extend javafx.application.Application
```
1. To resolve this problem, first type in `cd lab7` to see where your current directory is. 
2. Type in `ls` to show the files in the directory. 
3. Use `bash test.sh` to run the tests and see where the files have failed. 

## Step 3: Use VIM 
Let's now edit the file using vim. We need to debug an error in our code so the tests can pass. 
1. In the terminal, insert `vim ListExamples.java` so you can see the file using vim. 
2. We need to fix index1 to index2 in the final loop in the merge method. On computer, we normally do `control + F` or `command + F` (MAC users). For vim, the command is /<contentToFInd>, we will do `/index1`. To search through occurrences of the word like index1 in this case, press n to find the particular index1 we are looking for. 
3. Then move cursor using key l and place it on `1` in the word index1 then press on `2` and it will become index21. 
4. Press `esc` and then search `/index21`, then move the cursor until it is on 1 and press `x` to delete the 1. 
5. The error is now fixed, you will need to exit and save the file by pressing `esc` then `:wc + <enter>(or <return> for MAC users)`

