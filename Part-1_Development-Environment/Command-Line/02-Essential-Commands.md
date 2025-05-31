# Lesson 2: Essential Commands

## 🎯 Learning Objectives
- Master essential file and directory operations
- Learn to create, copy, move, and delete files
- Understand command options and arguments
- Build confidence with daily development tasks

## 📁 Directory Operations

### Creating Directories (`mkdir`)

```bash
# Create a single directory
mkdir my-project

# Create multiple directories
mkdir project1 project2 project3

# Create nested directories (parent directories too)
mkdir -p projects/web/my-site
# Windows: mkdir projects\web\my-site

# Create directory with spaces in name
mkdir "My Awesome Project"
```

**Practice Example:**
```bash
# Create a coding workspace
mkdir coding-workspace
cd coding-workspace
mkdir python-projects javascript-projects resources
ls
```

### Removing Directories (`rmdir` or `rm -r`)

```bash
# Remove empty directory
rmdir empty-folder

# Remove directory and all contents (BE CAREFUL!)
# Mac/Linux
rm -r folder-with-files
rm -rf folder-with-files  # Force removal, no prompts

# Windows
rmdir /s folder-with-files
```

**⚠️ Safety Warning:** `rm -rf` and `rmdir /s` permanently delete everything! Double-check before using.

## 📄 File Operations

### Creating Files

**Mac/Linux:**
```bash
# Create empty file
touch filename.txt
touch index.html style.css script.js

# Create file with content
echo "Hello, World!" > hello.txt
echo "print('Hello, Python!')" > hello.py
```

**Windows:**
```bash
# Create empty file
echo. > filename.txt
type nul > index.html

# Create file with content
echo Hello, World! > hello.txt
echo print('Hello, Python!') > hello.py
```

### Viewing File Contents

```bash
# Display entire file
# Mac/Linux
cat filename.txt
cat hello.py

# Windows
type filename.txt
type hello.py

# Display first few lines
head filename.txt      # Mac/Linux
more filename.txt      # Windows (shows page by page)

# Display last few lines
tail filename.txt      # Mac/Linux

# View file page by page
less filename.txt      # Mac/Linux (press 'q' to quit)
more filename.txt      # Windows
```

### Copying Files (`cp` or `copy`)

**Mac/Linux:**
```bash
# Copy file to new name
cp original.txt backup.txt

# Copy file to different directory
cp file.txt Documents/
cp file.txt ~/Desktop/newname.txt

# Copy multiple files
cp file1.txt file2.txt file3.txt target-directory/

# Copy directory and contents
cp -r source-folder/ destination-folder/
```

**Windows:**
```bash
# Copy file
copy original.txt backup.txt

# Copy to different directory
copy file.txt Documents\
copy file.txt %USERPROFILE%\Desktop\newname.txt

# Copy multiple files
copy *.txt target-directory\

# Copy directory
xcopy source-folder destination-folder /E /I
```

### Moving/Renaming Files (`mv` or `move`)

**Mac/Linux:**
```bash
# Rename file
mv oldname.txt newname.txt

# Move file to directory
mv file.txt Documents/
mv file.txt ~/Projects/web/

# Move and rename simultaneously
mv oldfile.txt ~/Documents/newfile.txt

# Move multiple files
mv *.txt text-files/
```

**Windows:**
```bash
# Rename file
move oldname.txt newname.txt
ren oldname.txt newname.txt

# Move file to directory
move file.txt Documents\
move file.txt %USERPROFILE%\Projects\web\

# Move multiple files
move *.txt text-files\
```

### Deleting Files (`rm` or `del`)

**Mac/Linux:**
```bash
# Delete single file
rm filename.txt

# Delete multiple files
rm file1.txt file2.txt
rm *.txt              # Delete all .txt files

# Delete with confirmation
rm -i important.txt   # Asks before deleting

# Force delete (no confirmation)
rm -f filename.txt
```

**Windows:**
```bash
# Delete single file
del filename.txt

# Delete multiple files
del file1.txt file2.txt
del *.txt             # Delete all .txt files

# Delete with confirmation
del /p important.txt  # Asks before deleting
```

## 🔍 Finding Files and Information

### Listing with Details

**Mac/Linux:**
```bash
# Detailed list
ls -l                 # Long format
ls -la                # Long format + hidden files
ls -lh                # Long format + human-readable sizes
ls -lt                # Sort by modification time
ls *.py               # List only Python files
```

**Windows:**
```bash
# Detailed list
dir /a                # Show all files including hidden
dir /o:d              # Order by date
dir /o:s              # Order by size
dir *.py              # List only Python files
```

### Finding Files

**Mac/Linux:**
```bash
# Find files by name
find . -name "*.py"           # Find all Python files
find . -name "config.txt"     # Find specific file
find . -type d -name "test*"  # Find directories starting with "test"

# Search file contents
grep "function" *.js          # Find "function" in JS files
grep -r "TODO" .              # Search "TODO" in all files recursively
```

**Windows:**
```bash
# Find files
dir /s *.py               # Find all Python files recursively
where python              # Find where Python is installed

# Search file contents
findstr "function" *.js   # Find "function" in JS files
findstr /s "TODO" *.*     # Search "TODO" in all files
```

## 🎯 Command Structure and Options

### Understanding Command Syntax

```bash
command [options] [arguments]

# Examples:
ls -la Documents          # command: ls, option: -la, argument: Documents
cp -r source destination  # command: cp, option: -r, arguments: source, destination
mkdir -p path/to/folder   # command: mkdir, option: -p, argument: path/to/folder
```

### Common Option Patterns

**Single letter options:**
```bash
ls -l    # Long format
ls -a    # All files (including hidden)
ls -h    # Human readable
```

**Combined options:**
```bash
ls -la   # Long format + all files
ls -lah  # Long format + all files + human readable
```

**Long form options (Mac/Linux):**
```bash
ls --help          # Get help
rm --interactive   # Same as rm -i
```

## 🏋️ Practice Exercises

### Exercise 1: File Management Basics
```bash
# 1. Create a project directory
mkdir my-first-project
cd my-first-project

# 2. Create some files
touch README.md
touch app.py
touch style.css

# 3. List files to verify
ls -la

# 4. Create subdirectories
mkdir src tests docs

# 5. Move files to appropriate directories
mv app.py src/
mv style.css src/

# 6. Copy README to docs
cp README.md docs/

# 7. List everything
ls -la
ls src/
ls docs/
```

### Exercise 2: Content Creation and Viewing
```bash
# 1. Create a file with content
echo "# My Project" > README.md
echo "This is my first project" >> README.md

# 2. View the file
cat README.md        # Mac/Linux
type README.md       # Windows

# 3. Create a Python script
echo "print('Hello, World!')" > hello.py

# 4. Create multiple files at once
touch script1.py script2.py script3.py

# 5. List only Python files
ls *.py             # Mac/Linux
dir *.py            # Windows
```

### Exercise 3: Organization and Cleanup
```bash
# 1. Create a messy directory with mixed files
mkdir temp-workspace
cd temp-workspace
touch file1.txt file2.py file3.js file4.txt file5.py

# 2. Create organization directories
mkdir python-files javascript-files text-files

# 3. Move files to appropriate directories
mv *.py python-files/
mv *.js javascript-files/
mv *.txt text-files/

# 4. Verify organization
ls -la
ls python-files/
ls javascript-files/
ls text-files/

# 5. Clean up (be careful!)
cd ..
rm -r temp-workspace    # Mac/Linux
rmdir /s temp-workspace # Windows
```

## 💡 Pro Tips

### 1. Wildcards
```bash
# * matches any characters
ls *.txt          # All files ending in .txt
cp *.py backup/   # Copy all Python files

# ? matches single character
ls file?.txt      # file1.txt, file2.txt, but not file10.txt

# [] matches character range
ls file[1-3].txt  # file1.txt, file2.txt, file3.txt
```

### 2. Command History and Shortcuts
```bash
# Navigate command history
↑ ↓               # Previous/next commands
!!                # Repeat last command
!ls               # Repeat last command starting with 'ls'

# Keyboard shortcuts
Ctrl+C            # Cancel current command
Ctrl+L            # Clear screen (same as 'clear')
Ctrl+A            # Go to beginning of line
Ctrl+E            # Go to end of line
```

### 3. Safety Practices
```bash
# Always verify location
pwd

# List before deleting
ls file-to-delete.txt
rm file-to-delete.txt

# Use confirmation for important deletions
rm -i important-file.txt    # Mac/Linux
del /p important-file.txt   # Windows

# Backup before major changes
cp important-file.txt important-file.txt.backup
```

## 🚨 Common Mistakes and How to Avoid Them

### 1. Deleting Wrong Files
```bash
# ❌ Dangerous
rm *              # Deletes everything in current directory

# ✅ Safe
ls               # Check what's here first
rm filename.txt  # Delete specific file
```

### 2. Wrong Directory Operations
```bash
# ❌ Wrong
mkdir project
cd projects      # Typo! Directory doesn't exist

# ✅ Correct
mkdir project
cd project       # Correct spelling
```

### 3. Case Sensitivity Issues
```bash
# ❌ Won't work on Mac/Linux
cd desktop

# ✅ Correct
cd Desktop
```

## ✅ Knowledge Check

Before moving to the next lesson, ensure you can:

- [ ] Create and remove directories
- [ ] Create files with and without content
- [ ] Copy files and directories
- [ ] Move and rename files
- [ ] Delete files safely
- [ ] Use wildcards to work with multiple files
- [ ] View file contents
- [ ] Understand command options and arguments
- [ ] Navigate command history efficiently

## 🎉 Congratulations!

You now have the essential file management skills every developer needs! You can:
- Organize project directories efficiently
- Create and manage files from the command line
- Use powerful shortcuts and wildcards
- Work safely with important files

## 🔜 Next Steps

In the next lesson, you'll learn:
- Advanced file management techniques
- File permissions and security
- Working with multiple files efficiently
- Preparation for Git workflows

---

**Ready to continue?** Move on to [Lesson 3: File Management](03-File-Management.md)

**Want more practice?** Try organizing a real project directory, or create a practice workspace to experiment with all these commands safely! 🚀