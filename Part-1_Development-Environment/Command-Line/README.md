# Command Line Basics

Learn to control your computer with text commands like a pro developer!

## 🎯 What is the Command Line?

The command line (also called terminal, shell, or command prompt) is a text-based interface to your computer. Instead of clicking icons, you type commands to:

- Navigate through folders
- Create and delete files
- Run programs
- Install software
- Control your development environment

## 🖥️ Accessing the Command Line

### Windows
- **Command Prompt:** Press `Win + R`, type `cmd`, press Enter
- **PowerShell:** Press `Win + X`, select "PowerShell"
- **Git Bash:** (Install with Git) - Recommended for this course
- **Windows Terminal:** Modern option from Microsoft Store

### macOS
- **Terminal:** Press `Cmd + Space`, type "Terminal", press Enter
- **iTerm2:** Popular alternative (download from iterm2.com)

### Linux
- **Terminal:** Usually `Ctrl + Alt + T`
- **Various options:** gnome-terminal, konsole, xterm

## 📚 Lesson Plan

### Lesson 1: Getting Started (15 minutes)
- Understanding the command line interface
- Basic navigation and file system structure
- Your first commands

### Lesson 2: Essential Commands (20 minutes)
- File and directory operations
- Viewing and editing files
- Common shortcuts and tips

### Lesson 3: File Management (15 minutes)
- Creating, copying, moving files
- Working with multiple files
- File permissions and safety

### Lesson 4: Advanced Techniques (20 minutes)
- Command history and shortcuts
- Pipes and redirection
- Environment variables
- Customizing your shell

## 🎯 Learning Objectives

By the end of this section, you will:
- Navigate your file system confidently using commands
- Create, move, copy, and delete files and directories
- Understand file paths (absolute vs relative)
- Use command line efficiently with shortcuts
- Feel comfortable with the terminal interface
- Be ready to use Git and other development tools

## 🚀 Quick Reference

### Essential Commands (Learn These First!)

| Command | What it does | Example |
|---------|--------------|---------|
| `pwd` | Show current directory | `pwd` |
| `ls` (Mac/Linux) `dir` (Windows) | List files | `ls` or `dir` |
| `cd` | Change directory | `cd Documents` |
| `mkdir` | Make directory | `mkdir my-project` |
| `touch` (Mac/Linux) `echo.>` (Windows) | Create file | `touch readme.txt` |
| `cp` (Mac/Linux) `copy` (Windows) | Copy file | `cp file1.txt file2.txt` |
| `mv` (Mac/Linux) `move` (Windows) | Move/rename | `mv old.txt new.txt` |
| `rm` (Mac/Linux) `del` (Windows) | Delete file | `rm unwanted.txt` |
| `clear` (Mac/Linux) `cls` (Windows) | Clear screen | `clear` |

## 💡 Why Learn Command Line?

### For Programming
- **Git requires it:** Version control uses command line
- **Package managers:** Install libraries and tools
- **Build tools:** Compile and run your programs
- **Servers:** Deploy your applications

### For Efficiency
- **Faster navigation:** Jump directly to any folder
- **Batch operations:** Work with many files at once
- **Automation:** Write scripts to repeat tasks
- **Flexibility:** More control than GUI interfaces

### For Your Career
- **Professional requirement:** All developers use command line
- **System administration:** Manage servers and deployments
- **DevOps:** Continuous integration and deployment
- **Troubleshooting:** Debug issues more effectively

## 🎮 Gamification Challenges

As you learn, try to complete these challenges:

**Beginner (⭐)**
- [ ] Navigate to your Desktop using `cd`
- [ ] Create a new folder called "coding-practice"
- [ ] Create 3 files inside that folder
- [ ] List all files in the folder

**Intermediate (⭐⭐)**
- [ ] Create a folder structure: `projects/web/my-site`
- [ ] Navigate to `my-site` in one command
- [ ] Copy a file from Desktop to this folder
- [ ] Rename the copied file

**Advanced (⭐⭐⭐)**
- [ ] Use a single command to create multiple folders
- [ ] Find all `.txt` files on your computer
- [ ] Create a backup of an entire folder
- [ ] Set up a custom command alias

## 🛡️ Safety Tips

**Always Remember:**
- **Double-check before deleting:** Use `ls` to verify location
- **Start in safe folders:** Practice in Documents or Desktop
- **Backup important files:** Before experimenting
- **Read before pressing Enter:** Understand what a command does

**Dangerous Commands to Avoid (for now):**
- `rm -rf /` (Unix) or `del *.*` (Windows) - Can delete everything!
- `sudo` commands - Can modify system files
- `chmod 777` - Can create security vulnerabilities

## 📱 Learning on Mobile

Can't access a computer? You can still learn:
- **Termux (Android):** Real Linux terminal on your phone
- **iSH (iOS):** Linux shell for iPhone/iPad
- **Online terminals:** Try terminals in your browser
- **Watch videos:** See commands in action

## 🔧 Common Issues and Solutions

**"Command not found"**
- Check spelling and case sensitivity
- Make sure you're using the right OS commands
- Try the full path to the program

**"Permission denied"**
- You might not have access to that file/folder
- Try from your home directory
- On Unix systems, you might need `sudo` (be careful!)

**"No such file or directory"**
- Check your current location with `pwd`
- Verify the file/folder exists with `ls`
- Check spelling and spaces in names

## 🎉 Success Indicators

You'll know you're ready to move on when you can:
- Navigate to any folder on your computer without looking
- Create project folders and files quickly
- Feel comfortable typing commands instead of clicking
- Understand error messages and fix simple issues
- Want to use terminal for tasks you used to do with mouse

## 🔜 Next Steps

After mastering command line basics:
1. **Git Basics:** Use command line for version control
2. **SSH Setup:** Secure connections with keys
3. **Development Workflow:** Professional practices

---

**Ready to start?** Open your terminal and begin with [Lesson 1: Getting Started](01-Getting-Started.md)!

*Remember: Everyone feels intimidated by the command line at first. With practice, you'll wonder how you ever lived without it!* 💪