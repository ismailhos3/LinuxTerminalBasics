# `Vim` Text Editor

In Vim, there are three modes;

* `command` mode,
* `insert` mode,
* `visual` mode,

## `insert` mode

Press `i` for the `insert` mode to start writing something on the document. When you press `i`, you will see on the bottom-left corner that `--INSERT--` will be printed out. 

![](../figures/001_vim_figures.png)

Type something and press `ESC` to go back the `command` mode.

* `i` to start typing where the cursor is,
* `shift+i` to start typing at the beginning of the line where the cursor is,
* `a` to start typing one character right from where the cursor is,
* `shift+a` to start typing at the end of the line where the cursor is,
* `o` to start typing one line below from where the cursor is.
* `shift+o` to start typing one line above from where the cursor is.

## `command` mode

In the `command` mode, you can move on the text:

### Move the cursor on the text

|Keys|Explanation|
|----|-----------|
|`k` ↑      |To move the cursor up (or the upper arrow can be used)|
|`j` ↓      |To move the cursor down (or the lower arrow can be used)|
|`h` ←      |To move the cursor left (or left arrow can be used)|
|`l` →      |To move the cursor to the right (or the right arrow can be used)
|`w`        |To jump forwards to the start of a word (Punctuation is considered words as well)|
|`shift+w`  |To jump forwards to the start of a word (Punctuation is NOT considered words)|
|`e`        |To jump forwards to the end of a word (Punctuation is considered words as well.)|
|`shift+e`  |To jump forwards to the end of a word (Punctuation is NOT considered words)|
|`b`        |To jump backwards to the start of a word (Punctuation is considered words as well)|
|`shift+b`  |To jump backwards to the start of a word (Punctuation is NOT considered words)|
|`ge`       |To jump backwards to the end of a word (Punctuation is considered words)|
|`g+shift+e`|To jump backwards to the end of a word (Punctuation is NOT considered words)|
|`g+g`      |To go to the first character of the document|
|`shift+g`  |To go to the last character of the document|

### Select and copy or cut

|Keys|Explanation|
|----|-----------|
|`shift+v`         |You can select the current line                           |
|`ctrl+v`          |You can select character by character                     |
|`y+y`             |The current line is copied (copy 1 line)                  |
|`y+3`             |4 lines are copied (number starts at 0)                   |
|`shift+v` then `y`|The line is selected and copied                           |
|`ctrl+v` then `x` |The line is selected and cut                              |
|`p`               |Items which are selected are pasted                       |


