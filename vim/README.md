This is a short introduction to vim and how to feel awesome with vim

## Installtion:
Most of the time its installed no matter what you have linux/unix/mac

To use the latest version you can install it again:
```
#Mac installation
brew install vim
```

vim = VI improved
vim is the improved version of vi 

when you edit a file using vim
```
vi <file>
#or you can
vim <file>
```

Every settings of vim is saved in `~/.vimrc` file


## Setting line numbers in vim
By default when you open a file using vim you dont see line numbers, open a file and do this to see the line numebrs
```
<esc> +:set number <enter>
```

Or you can just put this line in `~/.vimrc` file directly to always by default see line numbers in all files opened by vim

##2. Change modes in vim
There are 2 modes in vim one is INSERT mode another is command mode

Where you are in INSERT mode you will see `-- INSERT --` at the bottom of the file. When you press <esc> you go into command mode to start writing a command in this mode you need to 

##3. Some quick commands

```
:qw #quit with saving
:w #save file
:q #quit without saving
```

##4. Modes in vim
1. INSERT: when you are allowed to put text into the doc
2. VISUAL: when you are allowed to select some text from your doc


##5. Copy text

```
#goto visual mode
<esc> + v
scroll and select the lines
y # n lines are yanked
goto the place where you want to put the text
<esc> + p
```

#6. Cut/delete n line

```
<esc> + <number>dd
p
```

#7. Undo/Redo
```
<esc> + u
<esc> + <ctrl> + r
```

#8. search words in a file
```
<esc> + /<word>
<shift> + 8
```

#9. search and replace:
```
:%s/<find_word>/<replace_word>     # this will replace all
:%s/<find_word>/<replace_word>/c   # this will give you a prompt for each lines
```

# 10. file traverse
```
<shift> + up/down/left/right
```



