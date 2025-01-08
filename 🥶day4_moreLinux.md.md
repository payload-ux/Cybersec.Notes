### **Linux File Hierarchy**

Linux/UNIX uses a structured file system different from Windows.

#### Key Directories in Linux:

1. **/** (Root):
    
    - The top-level directory, starting point of the filesystem.
    - Only the root user can write here.
    - `/root`: Home directory for the root user (not the same as `/`).
2. **/bin**:
    
    - Binary executables essential for single-user mode (e.g., `cat`, `ls`, `cp`, `pwd`).
3. **/boot**:
    
    - Contains boot loader files like kernels .
4. **/dev**:
    
    - Files for devices attached to the system .
5. **/etc**:
    
    - Configuration files for programs and scripts for start up/shutdown (e.g., `/etc/passwd`).
6. **/home**:
    
    - User home directories (e.g., `/home/nathan`).
    - Denoted by `~`.
7. **/lib**:
    
    - Libraries required by binaries in `/bin` and `/sbin`.
8. **/media**:
    
    - Mount points for removable media like CDs and USBs.
9. **/mnt**:
    
    - Temporary mount directory for system administrators.
10. **/opt**:
    
    - Optional application packages (e.g., vendor software).
11. **/sbin**:
    
    - System binaries for administrators (e.g., `useradd`, `cron`).
12. **/tmp**:
    
    - Temporary files; cleared upon system reboot.
13. **/usr**:
    
    - User utilities and secondary programs.
    - Subdirectories:
        - `/usr/bin`: User binaries.
        - `/usr/sbin`: System binaries for administrators.
        - `/usr/lib`: Libraries for `/usr/bin` and `/usr/sbin`.

---

### **Text Editors**

#### **VIM** (VI Improved)

- **Modes:**
    - **Normal mode**  
    - **Command Mode:** Default mode, allows saving, quitting, undoing, and executing commands.
    - **Insert Mode:** Enter text by pressing `i`.
    - **Visual Mode:** Select and manipulate text blocks.
        - `v`: Character-wise.
        - `Shift + v`: Line-wise.
        - `Ctrl + v`: Block-wise.
- **Key Commands:**
    - Save: `:w`
    - Quit: `:q`
    - Save & Quit: `:wq!`
    - Undo: `:u`
    - Execute: `:%!command`

#### **Nano**

- Simple and user-friendly text editor.
- **Basic Commands:**
    - Save: `Ctrl + S`
    - Undo: `Alt + U`
    - Exit: `Ctrl + X`
    - Copy: `Ctrl + Shift + C`
    - Paste: `Ctrl + Shift + V`
- Appending text from files: `Ctrl + R`.

---

### **Linux User Management**

- **User Types:**
    
    - **Root User:** ID = 0; has complete system access.
    - **Normal User:** ID ranges from 1–999.
- **Commands:**
    
    - Check username: `whoami`.
    - Gain root access: `sudo su`.
    - Create users:
        - Simple: `sudo useradd username`.
        - Detailed: `sudo adduser username`.
- **Files for User Management:**
    
    - User details: `/etc/passwd`.
    - Passwords: `/etc/shadow`.