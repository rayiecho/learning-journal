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
- `grep -v "word" file` — lines WITHOUT th


## File Operations
cp file.txt backup.txt          # copy a file
cp -r folder/ backup/           # copy a folder
mv old.txt new.txt              # rename a file
mv file.txt ../otherfolder/     # move a file up one level
rm file.txt                     # delete a file
rm -r folder/                   # delete a folder
mkdir foldername                # create a folder
mkdir -p a/b/c                  # create nested folders
touch file.txt                  # create empty file

## Viewing Files
less file.txt                   # scroll through a file
head file.txt                   # first 10 lines
tail file.txt                   # last 10 lines
head -1 file.txt                # first 1 line
tail -1 file.txt                # last 1 line

## Finding Things
find . -name "*.txt"            # find by name
find . -type f -name "*.txt"    # find files only
find . -type d -name "myfolder" # find directories only
find . -maxdepth 1 -name "*.txt" # find without going deep
find . -size +1M                # find files bigger than 1MB
## Permissions
ls -l     see permisions
chmod +x add execution
chmod -x remove execution
chmod 644  # rw- r-- r-- (files)
chmod 755  # rwx r-x r-x (scripts/folders)
chmod 700  #rwx --- --- (prvate)

#number permisions
# r=4 w=2 x=1
# 7 = rwx (4+2+1)
# 6 = rw- (4+2)
# 5 = r-x (4+1)
# 4 = r 

## Processes
ps                #see process in the current terminal
ps aux            #see all processes in teh all system
top               #live processor monitor
kill PID          #stop a process
kilL 9 PID        #force stop a frozen process
sleep 100 &       #run a process in the background

## Shell scripting
#!/bin/bash    #Shebang always first lin.
NAME="Regan"   #Variable no spaces around =e
echo $NAME     #use variable with $
$(command)     #command substitution
if [ "$NAME" = "Regan" ];  then   #if statement
   echo Welcome
else
   echo Who are you
fi 
for i in {1..10}               # for loop
do 
   echo $i
Done
