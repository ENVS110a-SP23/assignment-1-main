# Assignment 1: Command Line Interface

The UNIX questions below will either give you a task or ask a question about bash and CLI. 
If the question gives you a task, write the bash command used to do this operation in `answers.txt`, 
a file you will create as part of this exercise.

## Bash

1.	Create a directory in your local assignment 1 directory called `answers`.
2.	Create a file called `answers.txt` in the answers directory. This is where you will be recording your answers to the rest of the questions for this assignment. 
3.	Edit the `answers.txt` file to record the commands used for questions 1 and 2.
4.	List the absolute path to your `answers.txt` file. 
5.	What flag lets us use `ls` to list all files in a directory, including hidden files?
6.	How can you use `ls` to list files outside of your current directory?
7.	Why is `rm` a dangerous command? Describe a scenario where it could lead to unintended negative consequences.
8.	Create a subdirectory in answers called `results`.
9.	Create a script that contains the following code:

```bash
#!/usr/bin/env bash

tsv="${1/.csv/.tsv}" 

sed "s/,/\t/g" $1 > $tsv

awk -F '\t' '{print $1}' $tsv
```

10.	Change permissions on the file to be able to execute it.
11.	Navigate to `data` directory in the assignment1 directory from the answers directory in a single command.
12.	Make a one-line pipe that returns the number of words in second largest file in the directory. 
13.	Loop through the .csv files in the data directory and run the script you created above.
14.	.zip files use data compression to reduce file size. We can unzip files to get back the original versions of them with `unzip filename.zip`. Unzip all files in `data` with the `.zip` extension and store them in a directory called `unzipped-files`.
15.	Remove all .zip files.
16.	Go to `unzipped-files` and copy all files from the 2000s to the results subdirectory you made earlier.

Stage, commit, and push your changes. 

## GitHub

1.	Go to GitHub and create a new repository called “ENVS110-intro” without a README.
2.	Clone the directory into your main GitHub directory.
3.	Within that directory, create a new file empty file named `README.md`. 
4.	Open `README.md`.
5.	Add your name and hit enter twice. Then write a short description about yourself, including things like your major, potential careers you are interested in, why you took this course, and your hobbies.
6.	Stage, commit, and push your changes. 

Source of data:

[https://aqs.epa.gov/aqsweb/airdata/download_files.html](https://aqs.epa.gov/aqsweb/airdata/download_files.html)
