# CommandLine
Levels 1 to 13 of the bandit.labs.overthewire.org as part of IDFC Neev Interns Training

Basic Commands:
1) ls - List contents
   - ls -a : Lists all files, including hidden files (those starting with a dot)
   - ls -l : Lists files in a long format, showing additional details like permissions, ownership, size, and timestamp.
   - ls -lh : Same as -l, but displays file sizes in a human-readable format

2) cd — Change directory
   - cd tmp : change directory to tmp
   - cd ..  : Move up 1 directory level
   - cd ~   : Move to home dir

3) cat - Concatenate and display file contents
   - cat file.txt : display contents of file.txt
   - cat -n file.txt : Displays the content with line numbers.

4) file - Determine file type
   - file filename : Tells you the type of filename.
   - file ./* : Tells the type of all files in dir

5) du - Disk usage
   - du -h : Shows disk usage in human-readable format
   - du -sh : Displays the total size of a directory.
   - du -a : Includes all files, not just directories.
  
6) find - Search for files in a directory
   - find /path/to/search -name "*.txt" : Finds all .txt files under the specified path.
   - find . -type f : Finds all files (not directories) in the current directory.
   - find . -type d : Finds all directories in the current directory.
   - find / -size +100M : Finds files larger than 100 MB.

Commands:
1) **To connect to website using SSH**: ssh username@web_url -p 0000
   - Enter password after this command
   - 0000 can be any port number
2) **To read contents of a file**: cat command
3) **To read a file starting with -**: cat ./-
4) **To read a file where file name has spaces**: cat "file name"
5) **To view hidden files**: Use command ls -a to list all files including hidden files
6) **To see all the file types in dir**: file ./*
7) **To find a file by adding filters**: example human readable, 1033 bytes non executable file then: find . -type f -size 1033c ! -executable
8) **To search for patterns within a file**: Like to search a word next to the word next to the word millionth we do: grep "millionth" data.txt
9) **To use unique**: uniq options:
   - -c: Count and show how many times each line appears.
   - -d: Show only duplicate lines.
   - -u: Show only unique lines.
10) **The strings command**: Searches for and prints sequences of printable characters in a binary file or a file that may contain non-text content.
11) **To decode base4**: base64 -d data.txt
12) **To rotate by 13 spaces**: cat data.txt | tr 'A-Za-Z' 'N-ZA-Mn-za-m'

