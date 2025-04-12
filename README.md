listfiles-nonzip is a simple shell command that recursively lists all non-.zip files in the current directory and its subdirectories. It prints each file path to the terminal and outputs the total count at the end. Useful for quickly auditing directory contents while ignoring archive files.


Usage:
find . -type f -not -name "*.zip" -print | tee /dev/tty | wc -l
