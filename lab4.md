# Lab Report 4
In this lab, it will show through how to reproduce each of the steps from lab using vim.
## 1 : In this first step, log onto your ieng6 account(no longer have to put in your password)
**Steps:** `ssh cs15lsp23mg@ieng6.ucsd.edu <enter>`
- for these steps, it logs into the specific account to perform specific tasks in the folders
<img width="1440" alt="Screen Shot 2023-05-22 at 5 10 14 PM" src="https://github.com/julieli3344/lab_Report_4/assets/83881461/269c94d3-8586-45f2-8913-694eeb04e3f7">

## 2 : Next clone your fork of the repository from your Github account using ssh instead of url
**Steps:** `git clone git@github.com:julieli3344/lab7.git <enter>`
- `git clone` is a specific git command to clone the repository, instead of using the url, I used ssh so I can commit and push everything to the account.
<img width="1440" alt="Screen Shot 2023-05-22 at 5 35 29 PM" src="https://github.com/julieli3344/lab_Report_4/assets/83881461/e77c3d04-1e02-498d-b0a3-43332bd41991">

## 3 : Run the ListExamplesTests to show that it will fail
**Steps:** `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java <enter>`, then I put `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests <enter>`
- This allows the tests to run and to see if they are failing or passing. In this case it fails because there is an error on the page which we can change later to have it pass later. 

<img width="1440" alt="Screen Shot 2023-05-18 at 5 12 57 PM" src="https://github.com/julieli3344/lab_Report_4/assets/83881461/790d68a8-fef2-4d10-b4c3-6bac2a344354">

## 4 : Now edit the code file using vim on ListExamples changing the 1 to a 2
**Steps:** `vim ListExamples <enter>`, and when I got to the page I used `j` 44 times and `l` 12 times to get to the exact spot of the `1`. Then I used `x <esc>`, `i`, `2 <esc>`, next I put `;wq <enter>` to escape out and save everything. 
- `vim` is a text editor that allows changes to the given file and there are shortcuts to change the page such as using `j` for going down, `k` for going up, `j` for going to the left and `l` for going to the right. Then `x` means to delete one character and `i` means to insert a letter into it. So I used these shortcuts to change a 1 into a 2. 
<img width="1440" alt="Screen Shot 2023-05-22 at 5 37 19 PM" src="https://github.com/julieli3344/lab_Report_4/assets/83881461/f3592d82-1f2c-4672-9e3e-75eb7ae2d255">

## 5 : Do the same thing, run the tests to demonstrate that they now succeed
**Steps:** `<up>, <up>, <up>, <enter>` to get `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`, then `<up>, <up>, <enter>` to get `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests <enter>` ( I was able to use up on the arrow pad because it was saved in the history)
- This allows to see all the tests failing or passing, which this time they all have passed so in the screenshot it shows them passing.
<img width="1440" alt="Screen Shot 2023-05-22 at 5 38 29 PM" src="https://github.com/julieli3344/lab_Report_4/assets/83881461/5ad457b9-37df-424e-94dc-8890b4baa674">

## 6 : As for the last step Commit and push the resulting change to your Github account
**Steps:** `git add ListExamples.java <enter>`, then `git commit -m "updated" <enter>`, then `git push`
- these last few steps helps to push everything that is changed into the Github account in order for it to update everything. For `git add` it allows it to add every line that has been changed in ListExamples.java, then `git commit` commits these changes out with a desired message, and `git push` pushes these changes to the account changing the file. 
<img width="1440" alt="Screen Shot 2023-05-22 at 5 43 07 PM" src="https://github.com/julieli3344/lab_Report_4/assets/83881461/9d8e70f9-a758-4c33-9c8b-c89ec2efa07c">
