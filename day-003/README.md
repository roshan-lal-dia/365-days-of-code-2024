## Day 3 - Tenth Line (Scripting | Basic Shell Commands)

### Problem: 
Problem [Link]([https://www.interviewbit.com/problems/grep-log](https://www.interviewbit.com/problems/tenth-line/))

>The following command prints the top 10 lines of file named input

```
cat input | head -n 10
```

>The following command prints the bottom 10 lines of file named input

```
cat input | tail -n 10
```

> Can you somehow use the above information to print the 10th line of the file named input ?

## Example:

>Assume that the input contains the following:

Line 1

Line 2

Line 3

Line 4

Line 5

Line 6

Line 7

Line 8

Line 9

Line 10

Line 11

Line 12

Line 13

Line 14

Line 15

>Your bash script should output the following:

Line 10

### Solution :

```
#!/bin/bash
cat input | head -n 10 | tail -1
```
