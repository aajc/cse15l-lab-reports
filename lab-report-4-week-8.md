# Lab Report 4

My markdown-parse repository: 
[My repo](https://github.com/aajc/markdown-parse)

Reviewed markdown-parse repository: 
[Other Repo](https://github.com/tanpatil/markdown-parse)

## Snippet 1

### My repository
My repository test for snippet 1 based off the VScode preview should produce [`google.com, google.com, ucsd.edu].

![Image](pictures/snippet1.png)

My implementation did not pass.
![Image](pictures/snip1test1.png)

I think there is a small change that will fix cases with inline code with backticks. One would only need a short if statement to find the opening and closing backticks and then would only need to ignore that part of the algorithm.

### Reviewed repository
The reviewed repository test for snippet 1 based off the VScode preview should produce [`google.com, google.com, ucsd.edu].

## Snippet 2

### My repository
My repository test for snippet 2 based off the VScode preview should produce [a.com, a.com(()), example.com].

![Image](pictures/snip2test1.png)

My implementation did not pass.
![Image](pictures/snippet2.png)

I think there is not a small change that will fix cases with nested special characters such as parentheses and brackets. It is more of an involved challenge because one does not know how many extra parenthesis and other special characters there are which makes it difficult to tell when to start and stop the link. It would need to be a smart program that checks for the last parenthesis and find the first parenthesis and then make the link which would take over ten lines most likely.

### Reviewed repository
The reviewed repository test for snippet 1 based off the VScode preview should produce [`google.com, google.com, ucsd.edu].

## Snippet 3

### My repository
My repository test for snippet 1 based off the VScode preview should produce [https://www.twitter.com, https://ucsd-cse15l-w22.github.io/, https://cse.ucsd.edu/].

![Image](pictures/snippet3.png)

My implementation did not pass.
![Image](pictures/snip3test1.png)

I think there is a small change that will make my program work for snippet3 and all related cases with newlines. The most needed change for my program would be a check for closingParen being -1 or it not existing and newlines in brackets and parenthesis should not break the program.

### Reviewed repository
The reviewed repository test for snippet 1 based off the VScode preview should produce [`google.com, google.com, ucsd.edu].