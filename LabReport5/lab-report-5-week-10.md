# Lab Report 5
## Using diff to find test results
![Image](Right1.png) 
![Image](Right2.png) 
**Description on how I found the tests** 
- First I started off by logging into ieng6 and cloning my markdown parse and cloning Joes markdown parse
- I ran multiple commands such as `make`, `chmod +x script.sh`, and `./script.sh | cat > results.txt`
- After than I ran the diff command in order to get the different test results

## Test File 506
### Different outputs
![Image](T.png) 
### Expected output
![Image](Realexpected.png) 
**Description** 
- As you can see the expected output is a url. Thus signifying that the output with the url at the top is the correct one. Which is Joes markdownparse

## Test File 510
### Different outputs
![Image](T1.png) 
### Expected output
![Image](Realexpected1.png) 
**Description** 
- As you can see the expected output is empty. Thus signifying that the output with the empty bracket is the correct one. Which is my markdownparse

## Contents of test file 506 and 510
![Image](testfiles.png) 
### Fixing my code for test file 506
![Image](mine.png) 
This image shows my repository due to the fact that the expected output was different than my output for the test file 506. As shown in the contents of test file 506 it would seem like my program does not account for quotation mark symbols. In order to fix my code and make sure that the actual output matches the expected output (Which is making sure that my code outputs a link rather than empty brackets) I could add quotation marks in the second part of line 39 of my code in order to account for the quotation marks. And potentially fix this problem in order to print out a url instead of empty brackets.

### Fixing Joes code for test file 510
![Image](joe.png) 
This image shows their repository due to the fact that the expected output was different than their output for the test file 510. As shown in the contents of test file 510 it would seem Joes program does not account for the space in between the closing bracket and the opening paranthesis .In order to fix Joes code and make sure that the actual output matches the expected output (Which is making sure that their code outputs a emtpy brackets rather than a link) I could add an if statement in the markdownparse in order to specifically account for spaces and if there are any I would return an empty bracket due to the fact that it is not a link.

