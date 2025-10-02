---
layout: page
title: Midterm guide
description: >-
    Midterm guide.
---

# CIS241 - F2025 Midterm Study Guide

## All material up to the midterm is valid for questions

* In-class discussions/demos
* Homeworks
* In-class assignments
* Slides

# NOTE - THIS LIST WILL CHANGE UP TO NEXT WEEK GIVEN HOW FAR WE GET!

## Things to know

* You can bring a 1-page cheat sheet, front and back.  You'll need to turn it in with your exam, so if you want it back put your name on it.

* The exam is hand-written - no devices allowed.

* The exam will comprise a number of theory (what you understand) and practical (do a thing) types of questions.
  * For the practical questions, I'll provide a reference guide on the back of the exam.
  * For example, if I ask you to count the number of lines in a file, you'd be provided with the `wc` command somewhere in the reference guide and a list of potentially relevant parameters.

## Sample topics

**Note - this is not comprehensive - anything is valid from the slides/assignments**

* Describe what a shell is and what it can be used for
* What are the different (common) modes in vim and what are they used for
* Describe how we know what type a file actually is
* Describe what a Linux kernel actually does
* What is a Linux distribution?
* Why does Linux exist?  Why don't we just use Unix?
* Describe the difference between absolute and relative paths, and be able to navigate to or work with a specified location (for both absolute and relative)
* Describe the difference between bash commands in the shell and a bash script
* Describe advantages and disadvantages of a Linux system
* What are some common uses for a Linux system?
* What is `/` in a Linux file system?  Where do your personal files typically exist?
* What is the difference between a terminal and a shell?
* Describe the difference between cloning a repository with git using either the https: or git: protocols - why do one over the other?
* Describe the differences between FTP, sFTP, scp, and rsync
* Describe the purposes of a `host` file (hostname alias), SSH keys, and how to create them
* Describe the purpose of SSH and why we SSH into EOS
* What does `echo $0` in the shell tell you?
* What does `echo $0` in a bash script tell you?
* What can a manual (man page) be used for?  How can you use it?
* Describe and/or demonstrate redirecting, piping, and appending
* Describe the differences between stdin and stdout and stderr
* What does `sudo apt update && sudo apt upgrade` do?  Why can't you do that on EOS?
* When chaining commands, describe the difference between using `;` vs `&&`.  What happens if you use a single `&`?
* Describe (and demonstrate) the difference between the various wildcard characters when looking for files (i.e., globbing)
  * For example, list all txt files in a directory, list all files that start with 7, etc.
* Understand the purpose of `wc`, `cut`, and `tr`
* What is the purpose of a tar archive?  How do we compress it?
* What is the purpose of git?  Who created it and why?
* What does it mean for a version control system to be distributed?  Why is that important?
* What is the difference between a local and remote repository for git?
* Describe the different processes in git (staging, committing, pushing/pulling) - what does each step **do**?
* Be able to describe branching, why we branch, etc.
* Describe how you might resolve a merge conflict
* How do we identify a particular commit?
* Why do we avoid rewriting history in git?
* Why do we always check the status (or `pull`) from a remote repository **before** working and always commit/push when we're **done** working?
* What does `git stash` do?  Why would you use it?
* Describe what the various forms of permissions do and do not allow for each of the three categories of user.
* What is the purpose of the `PATH` environment variable.  Why would you need to update it?  How do you make that persist?
* What is the purpose of the background and foreground for jobs?  Why would you send a program to the background?  How would you get it back to the foreground?  How would you stop it? 
* What is the purpose of the *init* daemon?
* Understand the relationship between parent and child processes.

## Sample practical questions

**Note - this is not comprehensive - anything is valid from the slides/assignments**

* Be able to:

  * Navigate to a directory (from a relative or absolute path)
  * Create a new directory
  * Create a new empty file
  * Write to a file directly from the terminal (no editors)
  * Append to a file directly from the terminal (no editors)
  * List the contents of a directory, potentially including hidden files, permissions, etc.
  * Pipe the output of one command into the input of another command
  * Save and quit in vim
  * Show me where you are on the filesystem
  * Delete files
  * Recursively delete files and folders, potentially folders with and without files inside them
  * Get the first and last lines from some form of input (stdout or file)
  * Count the number of lines, or bytes, or words, or all, of a file
  * Search for a particular string in a file, then count the number of unique occurrences of that string
  * Sort a file
  * Convert one character to another (or uppercase to lowercase or vice versa)
  * Parse a delimited file to grab a particular set of column or columns
  * Work with a local git repository (creating, staging, committing, branching)
  * Work with a remote git repository (creating, staging, committing, branching, pushing/pulling)
  * Set specified permissions on a file/directory, potentially recursively (I will tell you whether to use octal or character-based, so be comfortable with both)
  * Create aliases and make them persist
  * Create environment variables and make them persist
  * Output information to `stdout` and `stderr`
  * In vim, perform a search and replace for a specific string for all occurrences of the word
  * Transfer files to/from a remote server
  * List out your recent command history
  * Search through a file (or `stdin`) for a string
  * Be able to use the various commands from HW2 together (e.g., `wc`, `cut`, `tr`, `head`, `tail`...)
  * Be able to use the `tar` command to create a zipped archive using a compression method of my choosing (e.g., gz, bz2, xz).
      * Also, be able to extract it
  * Be able to resolve a merge conflict, given an example.  For example, if I give you a `diff` within a file, what commands would you run to fix things?
  * Check processes, their state, and trace their history.
  * Kill processes given a PID and a particular kill signal
  * Send a job between the background and foreground
  * Be able to write a bash script and make it executable
  * Be able to write a bash script that can:
    * Handle arguments
    * Define variables
    * Use if statements/switch statements
    * Use loops