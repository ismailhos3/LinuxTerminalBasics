# Computer Programming
## `cat` Command 
This command can add content to a file, and this makes it super powerful.
In its simplest usage, `cat` prints a file's content to the standard output:

`cat example.txt` 

![2.png](./figures/2.png)

You can print the content of multiple files:

`cat example.txt example2.txt` 

![1.png](./figures/1.png)

and using the output redirection operator `>` you can concatenate the content of multiple files into a new file:

`cat example.txt example2.txt > new_example.txt`

Here, ***new_example.txt*** is a concatenated version of files ***example.txt*** and ***example2.txt***

![3.png](./figures/3.png)

Using `>>` you can append the content of multiple files into a new file, creating it if it does not exist:

`cat example.txt example2.txt >> example3.txt`

`cat example3.txt`

![4.png](./figures/4.png)

When you're looking at source code files it's helpful to see the line numbers. You can have cat print them using the -n option:

`cat -n example3.txt`
![7.png](./figures/7.png)
![5.png](./figures/5.png)

You can only add a number to non-blank lines using -b:

`cat -b example3.txt`


![6.png](./figures/6.png)

The command `cat > example5.txt` creates a new file as output. We can write text in this file from the terminal.

![7.png](./figures/7.png)

When we want to write in a present file via on terminal:

`cat >> example5.txt` 

![8.png](./figures/8.png)

## `less` Command
