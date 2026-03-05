# Day 04 – Practical Linux Commands (After Dual Boot)

This page contains the Linux commands I used practically after setting up Linux in dual boot.

## System Information
uname -a  
Shows kernel and system information.

lsb_release -a  
Displays Linux distribution details.

## Current Directory and Files
pwd  
Shows the current working directory.

ls  
Lists files and folders.

ls -la  
Lists all files including hidden files with permissions.

## Directory Navigation
cd foldername  
Moves into a directory.

cd ..  
Moves one level up.

cd ~  
Moves to home directory.

## File Creation
touch test.txt  
Creates an empty file.

echo "Hello Linux" > test.txt  
Creates a file and writes text.

echo "More text" >> test.txt  
Appends text to an existing file.

## File Viewing and Editing
cat test.txt  
Displays file content.

nano test.txt  
Edits file using terminal editor.

## File and Folder Deletion
rm test.txt  
Deletes a file.

mkdir testfolder  
Creates a directory.

rmdir testfolder  
Deletes an empty directory.

rm -r foldername  
Deletes a directory and its contents.

## File Permissions
ls -l  
Shows file permissions.

chmod 777 test.txt  
Gives read, write, execute permission to all users.

chmod +x script.sh  
Makes a script executable.

## Temporary Files
cd /tmp  
Moves to temporary directory.

Files in /tmp may be deleted automatically after reboot.

## Searching with grep
grep "error" file.txt  
Searches for a word in a file.

grep -i "root" /etc/passwd  
Case-insensitive search.

grep -r "password" /etc  
Recursive search in directories.

## Networking Check
ip a  
Displays network interfaces.

iwconfig  
Displays wireless network information.

ping google.com  
Checks internet connectivity.

Press Ctrl + C to stop ping.

## System Update
sudo apt update  
Updates package list.

sudo apt upgrade  
Upgrades installed packages.
