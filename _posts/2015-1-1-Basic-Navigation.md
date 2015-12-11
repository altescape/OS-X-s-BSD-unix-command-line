---
layout: post
title: Basic Navigation (cd, pwd, ls) 
---

### __`cd`__ - Change directory. This lets you navigate to different directories.

Examples:

<dl>
  <dt class="code">cd Documents</dt>
  <dd>go into a subdirectory (of the current directory) named "Documents"</dd>

  <dt class="code">cd Documents/temp</dt>
  <dd>go into "Documents", then from there into a subdirectory named "temp"</dd>

  <dt class="code">cd ..</dt>
  <dd>go up to the parent of the current directory</dd>

  <dt class="code">cd ../..</dt>
  <dd>go up two levels, to the parent's parent</dd>

  <dt class="code">cd /</dt>
  <dd>go to the top of the boot volume</dd>

  <dt class="code">cd /Users</dt>
  <dd>go to the top of the boot volume, then into the top-level directory named "Users"</dd>

  <dt class="code">cd ~<dt>
  <dd>go to your home directory (note: that's a tilde, not a dash)</dd>

  <dt class="code">cd ~/Documents</dt>
  <dd>go to your home directory, then into your "Documents" directory</dd>

  <dt class="code">cd '/Applications (MacOS 9)'</dt>
  <dd>go to the of the boot volume, then into the top-level directory named "Applications (MacOS 9)". The quote marks tell the shell (command interpreter) to ignore the special characters (spaces and parentheses) in the directory name that would otherwise confuse it.</dd>

  <dt class="code">cd -</dt>
  <dd>go back to the previous directory</dd>
</dl>


### __`pwd`__ - Print working directory. This prints the path of the current working directory (i.e. it tells you where you are).

---

### __`ls`__ - List the files in the current directory, and (optionally) their characteristics.

Examples:

<dl>
  <dt>ls</dt>
  <dd>list just the names of the files in the current directory</dd>

  <dt>ls -l</dt>
  <dd>(long) list the files with their characteristics (size, privs, owner, etc)</dd>

  <dt>ls -lo</dt>
  <dd>list the files with their flags (see chflags) in addition to the usual characteristics -l shows</dd>

  <dt>ls -a</dt>
  <dd>list all files in the current directory (including those that would normally be invisible)</dd>

  <dt>ls -F</dt>
  <dd>list filenames with a special character at the end that tells you what kind of file it is ("/" for directory, "\*" for unix executable, "@" for alias/symlink, etc)</dd>

  <dt>ls \*.jpg</dt>
  <dd>list the names of all files with names ending in ".jpg"</dd>

  <dt>ls a\*</dt>
  <dd>list the names of all files with names beginning with "a"</dd>

  <dt>ls \*att\*</dt>
  <dd>list the names of all files with names containing "att"</dd>
</dl>
