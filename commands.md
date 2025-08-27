---
layout: page
title: Commands to Practice
description: Commands we talked about that you should practice.
---

This page lists the commands that you should be practicing.  I will do my best to keep this list updated as we go through things in class.

# Connecting

* `ssh` - connect to remove server
  * `ssh username@server_address`
  * E.g., `ssh yourusername@eos01.cis.gvsu.edu`

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

# Editing

* `nano <filename>` - edit a file with the nano editor
  * `^` in the bottom menu represents Ctrl (or Cmd if you're on Mac) 
