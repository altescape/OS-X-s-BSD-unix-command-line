---
layout: post
title: Basic Navigation (cd, pwd, ls) 
---

### _`cd`_ - Change directory. This lets you navigate to different directories.

Examples:

<dl>
  <dt>`cd Documents`</dt>
  <dd>go into a subdirectory (of the current directory) named "Documents"</dd>

  <dt>`cd Documents/temp`</dt>
  <dd>go into "Documents", then from there into a subdirectory named "temp"</dd>

  <dt>`cd ..`</dt>
  <dd>go up to the parent of the current directory</dd>

  <dt>`cd ../..`</dt>
  <dd>go up two levels, to the parent's parent</dd>

  <dt>`cd /`</dt>
  <dd>go to the top of the boot volume</dd>

  <dt>`cd /Users`</dt>
  <dd>go to the top of the boot volume, then into the top-level directory named "Users"</dd>

  #### cd ~
  &nbsp;&nbsp;&nbsp; go to your home directory (note: that's a tilde, not a dash)

  #### cd ~/Documents
  &nbsp;&nbsp;&nbsp; go to your home directory, then into your "Documents" directory

  #### cd '/Applications (MacOS 9)'
  &nbsp;&nbsp;&nbsp; go to the of the boot volume, then into the top-level directory named "Applications (MacOS 9)". The quote marks tell the shell (command interpreter) to ignore the special characters (spaces and parentheses) in the directory name that would otherwise confuse it.

  #### cd -
  &nbsp;&nbsp;&nbsp; go back to the previous directory
<dl>


### _`pwd`_ - Print working directory. This prints the path of the current working directory (i.e. it tells you where you are).

---

### _`ls`_ - List the files in the current directory, and (optionally) their characteristics.

Examples:

#### ls
&nbsp;&nbsp;&nbsp; list just the names of the files in the current directory

#### ls -l
&nbsp;&nbsp;&nbsp; (long) list the files with their characteristics (size, privs, owner, etc)

#### ls -lo
&nbsp;&nbsp;&nbsp; list the files with their flags (see chflags) in addition to the usual characteristics -l shows

#### ls -a
&nbsp;&nbsp;&nbsp; list all files in the current directory (including those that would normally be invisible)

#### ls -F
&nbsp;&nbsp;&nbsp; list filenames with a special character at the end that tells you what kind of file it is ("/" for directory, "\*" for unix executable, "@" for alias/symlink, etc)

#### ls \*.jpg
&nbsp;&nbsp;&nbsp; list the names of all files with names ending in ".jpg"

#### ls a*
&nbsp;&nbsp;&nbsp; list the names of all files with names beginning with "a"

#### ls \*att\*
&nbsp;&nbsp;&nbsp; list the names of all files with names containing "att"
