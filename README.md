### Directory
```
# current working directory
pwd 

# go to the home folder 
cd

# change your working directory
cd <filename>
cd <folder path>

# go to upper directory
cd ..
cd ../../.. 

# return to the previous directory
cd -
```

### Lists the content of the directory
```
ls
```

### Create/Copy/Move/Delete file or directory
```
# create new empty file
touch <filename>

# crate new folders
mkdir <foldername/>
mkdir -p <subdirectory/>

# creat a copied file or directory
cp <filename> <newcopiedfilename>
cp -r <directory> <newdirectory>

# moves a file/folder to a new location, or renames it
mv <filename> <newlocation>
mv <foldername> <newlocation>
mv <oldname> <newname>
mv <oldlocation> ./

# delete files or directories
rm <file1> <file2> <file3> ...
rm -r <emptydirectory>
rm -rf <directory>
```

### Manual Page/Clear screen/Historical commands
```
# display manualpage of rm command
man rm
# Manual page
man man

# clear the screen
clear

# show an historical list of commands 
history
```

### Change mode of a file
```
- r:read
- w:write
- x:execute

- 4 stands for "read",
- 2 stands for "write",
- 1 stands for "execute", and
- 0 stands for "no permission."

# user can read, write, and execute it; members of your group can read and execute it; and others may only read it.
chmod u=rwx,g=rx,o=r <filename>
chmod 754 <filename>

# user can execute
chmod +x <filename>
```

### Add Command
```
echo "message write here."
```

### Process
```
# finding
ps                     # processes your current shell session is running
ps aux | grep lighttpd # find running lighttpd server

# kill process
kill firefox
kill <PID number> # kill the process using a PID
kill $(lsof -t -i:8080) # kill any process listening to the port 8080
```

### Closing
```
# closing terminal
exit
```

### Read file
```
# print out the content of a text file given as argument
cat thisfile.exe

# first 10/5 lines of text file
head long.txt
head -n 5 long.txt

# last 4 lines
tail -n 4 long.txt

# search lines that contains a word
grep "linux" long.txt
```



