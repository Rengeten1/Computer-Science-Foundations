# Lesson 1: Getting Started with Command Line

## 🎯 Learning Objectives
- Open and understand the command line interface
- Learn your first essential commands
- Navigate basic file system structure
- Build confidence with text-based interaction

## 🖥️ Opening Your Terminal

### Windows Users
**Option 1: Git Bash (Recommended)**
1. Install Git from [git-scm.com](https://git-scm.com)
2. Right-click on Desktop → "Git Bash Here"
3. You'll see a terminal that works like Mac/Linux

**Option 2: Command Prompt**
1. Press `Windows key + R`
2. Type `cmd` and press Enter

**Option 3: PowerShell**
1. Press `Windows key + X`
2. Select "Windows PowerShell"

### Mac Users
1. Press `Cmd + Space` (Spotlight search)
2. Type "Terminal"
3. Press Enter

### Linux Users
1. Press `Ctrl + Alt + T`
2. Or search for "Terminal" in your applications

## 🔍 Understanding the Interface

When you open your terminal, you'll see something like:

```bash
# Mac/Linux
username@computername:~$ 

# Windows Command Prompt
C:\Users\username>

# Git Bash on Windows
username@computername MINGW64 ~
$ 
```

**Breaking it down:**
- `username` - Your login name
- `computername` - Your computer's name
- `~` - Your home directory (shortcut symbol)
- `$` or `>` - Prompt symbol (ready for your command)
- **Cursor** - Blinking line where you type

## 🚀 Your First Commands

### 1. Where Am I? (`pwd` - Print Working Directory)

```bash
pwd
```

**Result:** Shows your current location
```bash
# Mac/Linux
/Users/sarah
/home/alex

# Windows
C:\Users\Sarah
```

**What this means:** You're in your "home" directory, like your personal folder.

### 2. What's Here? (`ls` on Mac/Linux, `dir` on Windows)

**Mac/Linux:**
```bash
ls
```

**Windows:**
```bash
dir
```

**Result:** Lists files and folders in current location
```bash
Desktop    Documents    Downloads    Pictures
Music      Videos       Projects
```

### 3. Look Around More (`ls -la` or `dir /a`)

**Mac/Linux:**
```bash
ls -la
```

**Windows:**
```bash
dir /a
```

**Result:** Shows detailed information including hidden files
```bash
total 48
drwxr-xr-x  8 sarah  staff   256 May 31 12:13 .
drwxr-xr-x  4 root   staff   128 May 31 12:13 ..
-rw-r--r--  1 sarah  staff  1234 May 31 12:13 .bashrc
drwxr-xr-x  3 sarah  staff    96 May 31 12:13 Desktop
drwxr-xr-x  5 sarah  staff   160 May 31 12:13 Documents
```

**Understanding the symbols:**
- `.` = Current directory
- `..` = Parent directory (one level up)
- Files starting with `.` = Hidden files
- `d` at start = Directory (folder)
- `-` at start = Regular file

### 4. Moving Around (`cd` - Change Directory)

```bash
# Go to Desktop
cd Desktop

# Check where you are now
pwd

# Go back to home directory
cd ~

# Go up one level
cd ..

# Go to a specific path
cd Documents/Projects
```

**Important Notes:**
- **Case matters!** `Desktop` ≠ `desktop`
- Use **Tab key** to auto-complete folder names
- If folder name has spaces, use quotes: `cd "My Folder"`

## 🗂️ Understanding File Paths

### Absolute Paths (Full Address)
Starts from the root of your system:
```bash
# Mac/Linux
/Users/Rengeten1/Documents/coding-projects

# Windows
C:\Users\Rengeten1\Documents\coding-projects
```

### Relative Paths (From Current Location)
Based on where you are now:
```bash
# If you're in /Users/Rengeten1
Documents/coding-projects    # Go to Documents, then coding-projects
../Desktop                  # Go up one level, then to Desktop
./current-folder            # Stay in current location
```

### Special Path Shortcuts
```bash
~           # Home directory (/Users/Rengeten1)
.           # Current directory
..          # Parent directory (one level up)
../..       # Two levels up
-           # Previous directory (where you just were)
```

## 🏋️ Practice Exercises

### Exercise 1: Basic Navigation
1. Open your terminal
2. Check where you are with `pwd`
3. List what's in your current directory
4. Navigate to your Desktop
5. List what's on your Desktop
6. Go back to your home directory

### Exercise 2: Path Exploration
1. Navigate to your Documents folder
2. Check your current path
3. Go up one level (to your user folder)
4. Navigate to Desktop using relative path
5. Navigate to Documents using absolute path

### Exercise 3: Tab Completion
1. Type `cd Doc` and press **Tab** - it should complete to `Documents`
2. Type `cd D` and press **Tab twice** - see all options starting with D
3. Practice using Tab completion to navigate faster

## 💡 Pro Tips for Beginners

### 1. Use Tab Completion
- Type first few letters of folder name
- Press **Tab** to auto-complete
- Press **Tab twice** to see all options

### 2. Command History
- Press **Up arrow** to see previous commands
- Press **Down arrow** to go forward in history
- Type `history` to see all recent commands

### 3. Clear Your Screen
```bash
# Mac/Linux
clear

# Windows
cls
```

### 4. Cancel a Command
- Press **Ctrl + C** to stop a running command
- Press **Ctrl + D** to exit terminal

### 5. Get Help
```bash
# Mac/Linux
man ls          # Manual for 'ls' command
ls --help       # Quick help for 'ls'

# Windows
dir /?          # Help for 'dir' command
help dir        # Alternative help
```

## 🎯 Common Beginner Mistakes

### 1. Case Sensitivity
```bash
# Wrong (on Mac/Linux)
cd desktop

# Correct
cd Desktop
```

### 2. Spaces in Names
```bash
# Wrong
cd My Documents

# Correct
cd "My Documents"
# OR
cd My\ Documents
```

### 3. Forgetting Where You Are
```bash
# Always check your location
pwd

# List contents to orient yourself
ls    # Mac/Linux
dir   # Windows
```

## ✅ Knowledge Check

Before moving to the next lesson, make sure you can:

- [ ] Open a terminal on your operating system
- [ ] Use `pwd` to check your current directory
- [ ] Use `ls`/`dir` to list files and folders
- [ ] Navigate to different folders with `cd`
- [ ] Understand the difference between absolute and relative paths
- [ ] Use Tab completion to speed up navigation
- [ ] Clear your terminal screen
- [ ] Access command history with arrow keys

## 🎉 Congratulations!

You've taken your first steps into the world of command line! You can now:
- Navigate your computer using text commands
- Understand where you are in the file system
- Move around different directories
- Use essential shortcuts and tips

## 🔜 Next Steps

In the next lesson, you'll learn:
- Essential file and directory operations
- Creating, copying, and moving files
- More powerful commands for daily development
- Safety tips and best practices

---

**Ready to continue?** Move on to [Lesson 2: Essential Commands](02-Essential-Commands.md)

**Need more practice?** Spend 10-15 minutes navigating around your computer using only the command line. The more you practice, the more natural it becomes!

**Feeling stuck?** That's totally normal! Try the exercises again, and remember that every developer started exactly where you are now. 💪