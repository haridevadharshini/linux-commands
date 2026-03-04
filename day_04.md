# Day 04 – Files, Temporary Locations, and Searching

## Creating Files
Files can be created in multiple ways.

touch file.txt
Creates an empty file.

echo "text" > file.txt
Creates a file and writes text into it.

echo "more text" >> file.txt
Appends text to an existing file.

## Viewing and Updating Files
cat file.txt
Displays file content.

nano file.txt
Opens the file in terminal editor for editing.

Changes made in editors modify the file content.

## Deleting Files and Directories
rm file.txt
Deletes a file.

rm -r foldername
Deletes a directory and its contents.

Be careful: deleted files cannot be recovered easily.

## File Modification and Conflicts
When a file is edited multiple times or by different processes, changes may conflict.

Common situations:
- File edited but not saved
- File modified while another program is using it
- Version control conflicts during updates

Tools like editors and Git help resolve such conflicts.

## Important Linux Directories

/etc
Stores system configuration files.

/tmp
Used for temporary files.
Files here may be cleared automatically on reboot.

/var
Stores variable data such as logs and cache files.

## Searching with grep
grep "text" file.txt
Searches for a word inside a file.

grep -i "text" file.txt
Case-insensitive search.

grep -r "text" /directory
Searches recursively in directories.

## Using Pipes
The pipe (|) passes output of one command to another.

Example:
cat file.txt | grep "error"

This shows only lines containing the word "error".
