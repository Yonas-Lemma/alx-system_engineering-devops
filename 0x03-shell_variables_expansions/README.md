# 0-alias Script

This script creates an alias named `ls` that runs the command `rm *`. 

To activate the alias, run:
```bash
source ./0-alias


## 1-hello_you Script
This script prints a greeting message that includes the current Linux username.

Usage
Make the script executable:

bash
chmod +x 1-hello_you
Run the script:

bash
./1-hello_you
Output
It will display:

hello <your-username>
where <your-username> is the username of the current user.


source ./0-alias


## Script: 2-path
Description
This script adds /action to the end of the current PATH environment variable.
After running this script with source, the shell will look into /action last when searching for commands.

Usage
Make the script executable:

bash
chmod +x 2-path
Run the script in your current shell session:

bash
source ./2-path
Verify the change:

bash
echo "$PATH"
You should see /action as the last directory in the list.

Important
The change affects only the current session unless you add the command to your shell configuration files (like ~/.bashrc).
Make sure /action directory exists if you plan to add commands there.

###Script: 3-paths
Description
This script counts how many directories are listed in the current environment variable $PATH. It outputs the total number of directories.

How it works
It takes the $PATH string.
Replaces each colon (:) with a newline (\n) to split the list into individual directories.
Counts the number of lines (directories) using wc -l.
Prints the total count.
Usage
Make the script executable:

bash
chmod +x 3-paths
Run the script:

bash
. ./3-paths
The script will output a number, which is how many directories are in your $PATH.
Example
If your $PATH is:

/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin
Running the script will output:

4
