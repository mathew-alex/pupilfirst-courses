# Notes
```
- Skipping Profile
- Skipping WSL 
```

#### Command Line

```
pwd #print working directory
```
```
# navigate through directories using `cd` command

cd ~    #change directory to $(HOME), typically /home/<username> 
cd -    #change directory to previously visited directory
cd ..   # change directory to parent directory

```

```
# create folders using `mkdir` command

mkdir dir1 dir2 dir3        #create three separate folders in the current directory
mkdir -p dir4/dir5/dir6     #create parent directories also
```

```
# output redirection

ls > list.txt                                   # reditects the output of ls command to list.txt
echo "This text goes to a file" > file.txt      # instead of printing the output in console, the output is redirected to file.txt
cat text1.txt text2.txt > output.txt            # concatenate text1.txt and text2.txt and ouputs them into output.txt
cat *.txt >> output.txt                         # instead of replacing contents with the output of the command, the output is appended to the previous contenet of output.txt
```

```
# Move directories or files using `mv` command
mv source_file1.txt source_file2.txt source_file3.txt destination_folder/       # mv command can take 1 or more source files and move them to the destination specified as the last argument

# Remove directories or files using `rm` command
rm filename.txt     # removes a file
rm -r directory     # removes a directory,  `-r` is an option required to recursively delete everything inside the directory
```

```
# piping of commnd outputs usind a pipe (|)

ls | wc -l                          #lists the contents of current directory and `wc -l` is performed on the output to get count of lines
sort items.txt | uniq | wc -l       # the command will first sort items in the items.txt file,
                                    # then `uniq` command will run on the sorted items to take only unique lines,
                                    # then `wc -l` is run to find the count of that unique number of lines
```

