# Computer Programming

## `pwd` Command

`pwd` stands for `Print Work Directory` in Linux. Terminal opens at the home directory by default in Ubuntu. If you type pwd and press Enter you will see your home directory.

![](./figures/pwd_command.png)

## `ls` Command

We can list the files and folders in a directory using this command. It shows the files and folders located in your /home/"computer_name" directory. 

![](./figures/ls_command.png)

`ls` also has some options with it. One of them is `ls -l` which prints the details of the files such as the size of a file in KB and the date that the file has been created.

![](./figures/ls-l_command.png)

The other is `ls -la` and used for printing also the hidden files starting with `.` in your working directory.

![](./figures/ls-la_command.png)

## `cd` Command

Once you have a folder, you can move into it using the `cd` command. `cd` means `Change Directory` in Linux. You invoke it specifying a folder to move into. You can specify a folder name, or an entire path.

![](./figures/cd_command.png)

You can use the `..` special path to indicate the parent folder:

`cd ..` 

![](./figures/cd_back_command.png)

## `mkdir` Command

You create folders using the mkdir command:

`mkdir fruits`

![](./figures/mkdir_command.png)

You can create multiple folders with one command:

`mkdir plants animals`

![](./figures/mkdir_multiple_command.png)

You can also create multiple nested folders by adding the -p option:

`mkdir -p fruits/apples`

![](./figures/mkdir_nested_command.png)

You can also create a new set of nested files:

`mkdir -p vehicles/electric_vehicles/tesla_car`

![](./figures/mkdir_new_nested_folder_command.png)

## `touch` Command

You can create an empty file or files using the touch command:

`touch lessons`

![](./figures/touch_command.png)

## `rmdir` Command

Just as you can create a folder using `mkdir`, you can delete a folder using `rmdir`:

`mkdir test_file`

`rmdir test_file`

The folder you delete must be empty!

![](./figures/rmdir_command.png)

You can also delete multiple folders at once:

`mkdir testfile1 testfile2`

`rmdir testfile1 testfile2`

The folders you delete must be empty!

![](./figures/rmdir_multiple_delete_command.png)

## `rm` Command

To delete folders with files in them, we'll use the more generic `rm` command which deletes files and folders, using the `-rf` option:

When this command is used alone, it only deletes files, not folders.

`rm TestFile.txt`

![](./figures/rm_command.png)

If this command is used with `-rf` option, deletes everything such as folders and files. 

![](./figures/rm_with_rf_command.png)

## `cat` Command 

This command can add content to a file, and this makes it super powerful.
In its simplest usage, `cat` prints a file's content to the standard output:

`cat example.txt` 

![](./figures/cat_command.png)

You can print the content of multiple files:

`cat example.txt example2.txt` 

![](./figures/cat_multiple_command.png)

and using the output redirection operator `>` you can concatenate the content of multiple files into a new file:

`cat example.txt example2.txt > new_example.txt`

Here, ***new_example.txt*** is a concatenated version of files ***example.txt*** and ***example2.txt***

![](./figures/cat_merged_command.png)

To write to a file, we’ll make cat command listen to the input stream and then redirect the output of cat command into a file using the Linux redirection operators “>”.

Concretely, to write into a file using cat command, we enter this command into our terminal:

```cat > readme.txt``` 

We’ll see that once again the terminal is waiting for our input.

However, this time it won’t echo the texts we’ve entered. This is because we’ve instructed the command to redirect the output to the file readme.txt instead of the standard output stream.

Let's enter some text in the terminal and then continue with CTRL+D to terminate the command:

```
cat > readme.txt
This line was written by using terminal. # After typing, press CTRL+D to exit.
```

![](./figures/cat_writing_from_terminal_command.png)

Using `>>` you can append the content of multiple files into a new file, creating it if it does not exist:

`cat example.txt example2.txt >> example3.txt`

`cat example3.txt`

![](./figures/cat_transfer_to_newfile_command.png)

When you're looking at source code files it's helpful to see the line numbers. You can have cat print them using the -n option:

`cat -n example3.txt`

![](./figures/cat_add_number_command.png)

You can only add a number to non-blank lines using -b:

`cat -b example3.txt`

![](./figures/cat_add_nonblank_number_command.png)

The command `cat > example5.txt` creates a new file as output. We can write text in this file from the terminal.

![](./figures/cat_create_text_on_terminal_command.png)

When we want to write in a present file via on terminal:

`cat >> example5.txt` 

![](./figures/writing_to_existing_file_from_terminal.png)

## `echo` Command
  
We use `echo` to print anything on the command line:

![](./figures/echo1_command.png)

We can also use `echo` to write something into a file:

![](./figures/echo2_command.png)

If the file does not exist, we should use single `>` instead of `>>` :

![](./figures/echo3_command.png)

## `tail` Command

You can print the last 2 (or NUM) lines in a file:

`tail -n 2 example3.txt`

![](./figures/tail1_command.png)

You can print the whole file content starting from a specific line using `+` before the line number:

`tail -n +2 example3.txt`

![](./figures/tail2_command.png)

## `xdg-open` Command

`xdg-open file_name or folder_name` 

This command opens the specified file or folder.

![](./figures/xdg_command.png)

To open current directory:

`xdg-open .` is always used to open the current directory. Here the dot represents the current directory.

![](./figures/xdg2_command.png)

## `mv` Command

Once you have a file, you can move it around using the `mv` command. You specify the file current path, and its new path:

`mv mvcommand.txt move_command.txt`

Here, mvcommand.txt is renamed as move_command.txt.

![](./figures/move1_command.png)

`mv move_command.txt plants`

Here, move_command.txt is moved into the plants folder.

![](./figures/move2_command.png)

If the last parameter is a folder, the file located at the first parameter path is going to be moved into that folder. In this case, you can specify a list of files and they will all be moved in the folder path identified by the last parameter:

`mv example.txt example2.txt example3.txt example4.txt example5.txt examples`

![](./figures/move3_command.png)

## `cp` Command

You can copy a file using the `cp` command:

![](./figures/cp1_command.png)

To copy folders you need to add the `-r` option to recursively copy the whole folder contents:

![](./figures/cp2_command.png)

To copy multiple files to in to a folder:

`cp lesson1 lesson1_new lessons_folder` --> The lesson1 and lesson1_new is copied in to the lessons_folder

![](./figures/cp3_command.png)

## 'gedit' Command

`gedit` is the command to open the Ubuntu's default text editor Gedit. We can open and some files using it change and save:

`gedit new_file.txt`

![](./figures/gedit_command.png)

![](./figures/gedit_edit_file_command.png)

If we enter 'gedit' command on terminal, The file editor is opened immediately and you can write on it something.

To close the text editor and back to the terminal window you can use `ctrl+s` to save, `ctrl+w` to close the document editing and once more `ctrl+w` to close Gedit. 

As an other way to close it, press `ctrl+s` to save and go back to the terminal and press `ctrl+c`.

## `ln` Command

It's used to create links. 

We have 2 types of links: `hard links` and `soft links`.

### Hard Links
Hard links are rarely used. They have a few limitations: ***you can't link to directories, and you can't link to external filesystems (disks)***.

For example, say you have a file called lesson.txt. You can create a hard link to it using:

`ln lesson.txt lesson_linked.txt` # ln "orginal file name" "linked file"

![](./figures/ln_hardlink_command.png)

If we want to link a directory, we get an error:

![](./figures/ln_hardlink_limitation_command.png)



