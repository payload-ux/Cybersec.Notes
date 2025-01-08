

### **Advanced User Management**

#### **Commands:**

- **Change User Password:**

    
    `sudo passwd <username>`
    
- **Change User ID:**

    
    `sudo usermod -u <new_id> <username>`
    
- **Delete User:**
    

    
    `sudo userdel -r <username>`
    
- **Switch User in Terminal:**
    
    `su - <username>`
    
- **Create Home Directory:**

    
    `sudo mkhomedir_helper <username>`
    
- **Change Default Login Shell:**

    
    `sudo usermod <username> -s /bin/<shell>`
    

#### **Group Management Commands:**

- Create Group: `sudo groupadd <groupname>`
- Add User to Group: `sudo usermod -aG <groupname> <username>`
- Remove User from Group: `sudo gpasswd -d <username> <groupname>`

#### **Sudoers File:**

- The file determines who can use `sudo`.
- To modify:
    
    
    `sudo visudo`
    
- Add user to sudoers for elevated privileges.

---

### **File Ownership and Permissions**

- **Ownership Types:**
    
    - **User (Owner)**: The creator or assigned owner of the file.
    - **Group**: Group of users sharing access.
- **Changing Ownership:**

    
    `chown <user>:<group> <filename>`
    

#### **File Permissions:**

- **Permission Types:**
    - **Read (r)**: Value = 4
    - **Write (w)**: Value = 2
    - **Execute (x)**: Value = 1
- Permissions are represented as:
    - User (`u`), Group (`g`), Others (`o`), All (`a`).

#### **CHMOD Command:**

- Change permissions:
    
    `chmod <permissions> <filename>`
    
- **Using Symbolic Parameters:**
    - Add execute permission for all:
        
        `chmod a+x <filename>`
        
    - Remove execute permission for user:
        
        `chmod u-x <filename>`
        
- **Using Numeric Parameters:**
    - Example: `chmod 755 <filename>` (User: `rwx`, Group: `r-x`, Others: `r-x`).

#### **Special Permissions:**

- **SUID (Set User ID):** Add `4` (e.g., `4000`).
- **SGID (Set Group ID):** Add `2` (e.g., `2777`).
- **Sticky Bit:** Add `1` (e.g., `1602`).

---

### **Software Installation**

- **APT (Advanced Package Tool):**
    
    - Online/Offline Debian-based package manager.
    - Common commands:
        `sudo apt update sudo apt install <package> sudo apt remove <package> sudo apt upgrade sudo apt purge <package>`
        
- **Dpkg (Debian Package Manager):**
    
    - For `.deb` packages (offline).
    - Commands:
        
        `sudo dpkg -i <package> sudo dpkg -r <package> sudo dpkg -P <package>`
        

#### **Common Repository Errors:**

1. **Could not get lock:**
    - Solution: Restart the system or close other `apt` processes.
2. **Could not open lock:**
    - Solution: Run with `sudo`.
3. **Unable to locate package:**
    - Solution: Check for typos or repository configuration.
4. **Repository does not have a Release file:**
    - Solution: Fix repository configuration or update URL.