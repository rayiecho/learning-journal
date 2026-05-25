# Linux Commands — Regan Ayiecho

## Navigation
- `pwd` — print working directory (where am I?)
- `cd folder` — go into folder
- `cd ..` — go up one level
- `cd ~` or `cd` — go home
- `cd /full/path` — go anywhere (absolute path)
- `ls` — list files
- `ls -l` — detailed list with permissions
- `ls -a` — show hidden files
- `ls -la` — detailed + hidden

## File Operations
- `touch file.txt` — create empty file
- `echo "text" > file.txt` — create file with content (overwrites)
- `echo "text" >> file.txt` — append to file
- `cat file.txt` — read file
- `cat -n file.txt` — read with line numbers
- `wc -l file.txt` — count lines
- `cp file destination` — copy file
- `mv file newname` — move or rename
- `rm file` — delete file
- `rm -rf folder` — delete folder and all contents

## Folder Operations
- `mkdir folder` — create folder
- `mkdir -p path/to/folder` — create nested folders
- `rmdir folder` — remove empty folder

## Users & Permissions
- `whoami` — see current user
- `sudo command` — run command as admin
- `sudo whoami` — returns root

## Useful Tips
- Use `_` or `-` instead of spaces in filenames
- `>` overwrites, `>>` appends
- `/` at start = absolute path (works from anywhere)
- No `/` at start = relative path (depends where you are)
- Hidden files start with `.`

## Search
- `grep "word" file` — search for word in a file
- `grep -i "word" file` — case insensitive search
- `grep -n "word" file` — show line numbers
- `grep -v "word" file` — lines WITHOUT the word
