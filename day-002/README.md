## Day 2 - Grep Log (Scripting | Basic Shell Commands)

### Problem: 
Problem [Link](https://www.interviewbit.com/problems/grep-log)

Given a log file named input. You have to write a bash script which prints all the lines which contains mysql commands.

>Note

Assume that all the mysql commands start with mysql::.

>Example:

Assume that the input has the following content:

```
mysql:: SELECT * FROM courses;
rails:: Course.all
mysql:: SELECT id FROM courses;
rails:: Course.pluck(:id)
```
>Then your bash script should output the following:

```
mysql:: SELECT * FROM courses;
mysql:: SELECT id FROM courses;
```

>Our engineers were able to write this much code, can you complete it for us?

```
cat input | grep
```

### Solution :

```
#!/bin/bash
cat input | grep "mysql"
```
