# 🐧 Linux Shell Commands with Explanations

```sh
# Set an environment variable
export MESSAGE="Hello World"  

# Print text (literal)
echo Message                 

# Print variable value
echo $MESSAGE               

# List files
ls                          

# Long, hidden, human-readable
ls -lah                     

# Sorted by time, reversed, human-readable
ls -lrth  

# Sorted by size, human-readable
ls -lSh

# Show current directory
pwd                         

# Change to a specific directory
cd /root/sudhanshu          

# Go back one directory
cd ..                       

# Go back two directories
cd ../..                    

# Create an empty file
touch index.js

# Write into a file (overwrites)
echo "Hello World" > index.css

# Delete a file
rm file_name

# Open file in Vim
vim file_name

# Open file in Vi
vi file_name

# Edit with Nano
nano filename

# Nano commands:
#   ctrl + o → save
#   Enter    → confirm
#   ctrl + x → exit

# Display file content
cat filename.txt

# Display with line numbers
cat -n filename.txt

# Display multiple files with line numbers
cat -n filename1 filename2

# View file paged
more filename.txt

# View file with scroll (↑/↓), quit with 'q'
less filename.txt

# View with file info (less verbose mode)
less -M filename.txt

# Show first 10 lines
head filename.txt

# Show first 25 lines
head -n 25 filename.txt

# Show last 10 lines
tail filename.txt

# Show last 25 lines
tail -n 25 filename.txt

# Redirect ls output to a file (overwrite)
ls -lrth > output.txt

# Append ls output to a file
ls -lrth >> output.txt

# Append multiple files with line numbers to output.txt
cat -n filename.txt filename2.txt >> output.txt

# Redirect stdout to output.sh, stderr to error.txt
cat sshConnect.sh sshDisconnectAlll.sh 1>> output.sh 2>> error.txt

# Redirect stdout to output.sh, ignore stderr
cat sshConnect.sh sshDisconnectAlll.sh 1>> output.sh 2>> /dev/null

# Redirect both stdout and stderr to output.sh
cat sshConnect.sh sshDisconnectAlll.sh &> output.sh

# Print formatted text
printf "Hello World\n ghfref"

# Move file to a directory
mv index.js /root/sudhanshu/

# Move file back to current directory
mv /root/sudhanshu/index.js .

# Move directory to another path
mv Pranshu /root/sudhanshu/

# Move directory back to current path
mv /root/sudhanshu/Pranshu .

# Rename a file
mv index.js renamed.js

# Move and rename file
mv index.js /root/sudhanshu/output.js

# Move and rename back
mv /root/sudhanshu/output.js index.js

# Show help manual for mv
man mv

# Copy file to another directory
cp index.js /root/sudhanshu/

# Copy file back
cp /root/sudhanshu/index.js .

# Copy directory to another path
cp Pranshu /root/sudhanshu/

# Copy directory back
cp /root/sudhanshu/Pranshu .

# Rename a file by copying
cp index.js renamed.js

# Copy and rename to another path
cp index.js /root/sudhanshu/output.js

# Copy and rename back
cp /root/sudhanshu/output.js index.js

# Show help manual for cp
man cp

# Create multiple files with one command
touch /root/sudhanshu/temp/files{a,b,c}.txt

# List all files (including hidden) in the new directory
ls -lah /root/sudhanshu/temp/

# Copy the entire directory recursively
cp -r /root/sudhanshu/temp .