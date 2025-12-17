# Chapter 6 Input Output Redirection

This focus of this chapter is to cover the I/O Redirection Commands which allow a user to connect the input and output of commands to sort, read and print the output and input of text to standard out in the commandline

**Basic Commands Utilized**

- `cat`: Concatenates files together combining them into a single file

- `sort`: used to sort lines of text files from the commandline

- `uniq`: report or omit repeated lines to standard out or another element with a pipe

- `grep`: prints the lines matching a specified pattern

- `wc`: displays the newline, word and bytes of each file supplied to the command

- `head`: display the first part of the specified file

- `tail`: display the output of the specified file

- `tee`: read from standard input and write to standard outputs and files

------  

## Redirecting Standard Output and Standard Error to One File

combining the standard output redirection `>` with the `2>` will allow us to combine 
a call to the standard output and also include a location for our standard error to appear in the same location. the `2>&1` redirects standard error '`2>`' to the same location as the standard output with `&1` being appended to the end. 

```bash
# basic command for large output
ls -l /bin/usr > ls-output.txt 2>&1
```

