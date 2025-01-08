## overview of kali
- There are many tool on kali that used for many purpose.

1. information gathering 
2. vulnerability analysis
3. web application analysis
4. database assessment
5. password attacks 
6. Wireless attacks
7. Reverse engineering 
8. exploitation tools
9. sniffing and spoofing 
10. post exploitation
11. forensics
12. Reporting tools 
13. social Engineering tools 
14. system services
15. usually used applications

# folder managers 
1. dolphin
2. thunar
3. nautilus

# LINUX COMMANDS💎💎
- LINUX systems uses shell. the shell helps us to communicate with the kernel and helps to execute codes.
- shell is also called **Terminal** 
- WHAT IS THE DEFAULT SHELL TYPE FOR KALI LINUX?
   - BASH

## LINUX COMMAND BASICS
- On linux there are over 1000 commands. but we are expected to know the main and useful only.
- Also those commands have their own options and arguments.
# what is command 
- small programs that do one task well
- **Important Commands:**
    
    - `ls` - List directory contents.
    - `cd` - Change directory.
    - `pwd` - Print working directory.
    - `echo` - Display text.
    - `cat`, `head`, `tail`, `less` - Display file content.
    - `touch` - Create empty files.
    - `mkdir` - Create directories.
    - `clear` - Clear screen.
    - `rm` - Remove files or directories.
    - `cp`, `mv` - Copy or move files/directories.
    - `grep` - Search for patterns in files.
    - `wc` - Word, line, and byte count.

#### Advanced Tools

- **sed (Stream Editor):**
    
    - Text substitution and deletion.
    - Example: `sed 's/old/new/g' file`.
- **awk:**
    
    - Pattern scanning and data extraction.
    - Example: `awk '{print $1, $3}' file`.
   
## out put redirecting 
- you can write output of any command into files, this is called Redirecting 
- to do this we will use the ">"sign.
- echo text file.txt
- you can add texts (append )
- echo text >> file .txt

### Multiple command execution

- you can run /execute multiple command in 1 line 
- using three methods:
    - and(&&)
    - or (||)
    - Piping(|)

1. AND 
- ON AND operation all command will be executed. if both are working without error.
2. OR
- ON OR operation the command will be executed if it have error or not
3. Piping 
- on pipe, will help you run commands by using the output of the first command as the input for the next one .
