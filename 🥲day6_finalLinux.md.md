# Finishing for Linux – Summary

## Key Topics

- Script Installation
    
- Linux Help Commands
    
- Services & Processes
    
- Symbolic Linking
    
- Aliases
    
- Tmux Terminal Multiplexer
    
- Wget File Downloader
    
- Find Command
    

---

## Script Installation

- Use `git clone <url>` to download scripts from GitHub.
    
- Scripts use languages like Python, Bash, Go, Ruby.
    
- Install dependencies:
    
    - Python: `pip install <module>` or `pip install -r requirements.txt`
        
    - Go: `go install <module>`
        
    - Ruby: `gem install <module>`
        

---

## Linux Help

- `man <command>` – Full manual.
    
- `<command> -h` or `--help` – Brief help.
    

---

## Linux Processes & Services

- **Process**: Running program instance.
    
- View processes:
    
    - `ps` – Current shell
        
    - `ps -A` – All processes
        
    - `ps -u <user>` – User-specific
        
- Kill process:
    
    - `kill <PID>`, `killall <name>`
        
    - `kill -9 <PID>` – Force kill
        
- Monitor:
    
    - `top` or `htop`
        

---

## Foreground & Background

- Run in background: `command &` or `Ctrl+Z`
    
- Bring to foreground: `fg`
    
- Kill: `Ctrl+C`
    

---

## Managing Services

- Use `systemctl` or `service`:
    
    - `sudo systemctl start|stop|status|enable|disable <service>`
        
    - `sudo service <service> start|stop`
        

---

## Output Redirection

- `/dev/null` – Discards output.
    
- Redirect:
    
    - Errors: `2>`
        
    - Output: `1>`
        
    - To null: `command 2> /dev/null`
        

---

## Symbolic Linking

- Creates a shortcut to a file or folder.
    
- Syntax: `ln -s <original> <linkname>`
    
- Identified in `ls` by `l` and `->`
    

---

## Aliases

- Create shortcut for command:
    
    - Example: `alias ll='ls -la'`
        
- Make permanent:
    
    - Bash: `~/.bashrc`
        
    - Zsh: `~/.zshrc`
        
    - Fish: `~/.config/fish/config.fish`
        

---

## Tmux (Terminal Multiplexer)

- Start with: `tmux`
    
- Config file: `.tmux.conf`
    
- Basic commands:
    
    - Split horizontally: `Ctrl+A then o`
        
    - Split vertically: `Ctrl+A then e`
        
    - New tab: `Ctrl+A then c`
        
    - Rename tab: `Ctrl+A then ,`
        
    - Switch tab: `Ctrl+A then <number>`
        
    - Exit: `Ctrl+A then x` or type `exit`
        

---

## Wget

- Download from web: `wget <URL>`
    

---

## Find

- Search files or folders.
    
- Syntax: `find <path> [options] [pattern]`
    
- Examples:
    
    - `find / -name "linux"`
        
    - `find /home -perm 777`
        
    - `find -type f`, `find -type d`