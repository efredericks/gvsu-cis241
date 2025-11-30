---
layout: page
title: Commands to Practice
description: Commands we talked about that you should practice.
nav_order: 2
---

This page lists the commands that you should be practicing.  I will do my best to keep this list updated as we go through things in class.

# Connecting

* `ssh` - connect to remove server
  * `ssh username@server_address`
  * E.g., `ssh yourusername@eos01.cis.gvsu.edu`

# Getting files/directories

* `wget <URL>` - gets a file from a remote URL
* `git clone <REPO>` - clones a git repository
  * Note - typically you'll want to use the `SSH` version for repositories YOU'll be updating and the `HTTP` version for repositories you just want to play with

# Special file paths

* `.` - current working directory
* `..` - parent directory (go up a level)
* `~` - shortcut to your home directory
* `/` - root of file system
  * `/home/yourusername` - your home directory

# File systems

* `ls` - List files
  * E.g., `ls ~`, `ls .`, `ls CIS241`

* `cd` - Change directory
  * E.g., `cd ~`, `cd ..`, `cd /WEB_STUDENT/yourusername`

* `touch filename` - Create empty file

* `rm` - Remove -- **BE CAREFUL - THERE IS NO RECYCLE BIN AND ANYTHING DELETED CANNOT BE RECOVERED**
  * E.g., `rm filename` - deletes filename
  * `rm -rf directory` - removes the directory AND everything inside of it

* `rmdir` - Remove directory
  * E.g., `rmdir directory` - note, directory **must** be empty for this to work (the `rm -rf` command takes care of the deletion if not)

* `mv f1 f2` - Cut and paste or rename - `f1` is the original file/directory and `f2` is the new name of the file/directory
  * Examples (assuming we have `~/file1`, `~/file2`, `~/dir1`, `~/dir1/dir2`
    * `mv file1 file2` (renames `file1` to `file2`)
    * `mv ~/file1 ~/dir1/my_new_file` (moves and renames `file1` to be `my_new_file` within `dir1`)
    * `mv dir1 my_new_dir` (renames `dir1` to be `my_new_dir`)

* `cp f1 f2` - Copy and paste (same concept as `mv`, but creates a copy)
  * Examples (assuming we have `~/file1`, `~/file2`, `~/dir1`, `~/dir1/dir2`
    * `cp file1 new_file` (copies `file1` to `new_file`)
    * `cp -r dir1 newdir` (recursively copies `dir1` to `newdir` - meaning all the contents of `dir1` are also now in `newdir`)

* `tree` - shows a tree-based graphical representation of your current working directory and its children
  * `tree <path>` - same, but for the `<path>` provided

* `pwd` - tells you where you are at in the filesystem

# Viewing Files

* `cat <filename>` - dumps contents of file to terminal

# Editing

* `nano <filename>` - edit a file with the nano editor
  * `^` in the bottom menu represents Ctrl (or Cmd if you're on Mac) 

# Piping and Redirecting

* `command1 | command2`
  * Send output of `command1` into `command2`

* `command1 > file`
  * Send output of `command` into a new file: `file`

* `command1 > file 2> file.err`
  * Send output of `command` into a new file (`file`) and error into a new file (`file.err`)

# File Manipulation

*Worth checking the `man` pages for parameters!*

* `wc`
  * Count lines, words, and bytes in a file

* `cut`
  * Get columns in a delimited file or character offsets per line

* `tr`
  * Replaces characters with a specified pattern

* `diff`
  * Compares two files

---

# fgets newline fix

```
// replace newline in fgets 
char* result = fgets(s, 10, stdin);
char *n = strchr(s, '\n');
if (n != NULL) *n = '\0';
```

