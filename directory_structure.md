# Pre-Work Section B — File Systems & Directory Structures

## Part 1: Directory Structure

The following directory tree represents verified locations within my macOS home directory.

```text
/Users/
└── jordanhill/
    ├── Documents/
    │   ├── AutoTunePro/
    │   ├── terminal-practice/
    │   ├── about_me.py
    │   └── introduction.py
    ├── Desktop/
    ├── Downloads/
    ├── Applications/
    ├── Pictures/
    ├── Movies/
    ├── Music/
    └── VS CODE PYTHON SCHOOL FILES/
```

This structure illustrates how directories are organized hierarchically. The `jordanhill` directory is my home folder, and the directories beneath it contain different categories of files and projects.

## Part 2: Terminal Verification

I used the macOS terminal to verify the actual locations of directories in my filesystem and compare them with my original directory map.

### Check 1 — Downloads Directory

**Commands:**

```bash
cd ~/Downloads
pwd
```

**Actual output:**

```text
/Users/jordanhill/Downloads
```

### Check 2 — Desktop Directory

**Commands:**

```bash
cd ~/Desktop
pwd
```

**Actual output:**

```text
/Users/jordanhill/Desktop
```

### Check 3 — Home Directory

**Commands:**

```bash
cd ~
pwd
```

**Actual output:**

```text
/Users/jordanhill
```

### Check 4 — Hidden Files

**Command:**

```bash
ls -a
```

**Observed results:**

The terminal displayed both visible and hidden files and directories, including:

- `.zshrc`
- `.gitconfig`
- `.DS_Store`
- `.vscode`
- `Documents`
- `Downloads`
- `Desktop`

The `-a` option displays hidden entries whose names begin with a period.

### Check 5 — Final Working Directory

**Command:**

```bash
pwd
```

**Actual output:**

```text
/Users/jordanhill
```

### Comparison With My Original Directory Map

My original directory map correctly represented the general hierarchy of my files and folders, but it contained some inaccuracies. I initially used arrows to represent paths instead of the actual filesystem format.

The terminal confirmed that macOS paths use forward slashes (`/`) to separate directories. I also learned that `pwd` displays the full absolute path of my current working directory, while `ls -a` reveals hidden configuration files that are not always visible in Finder.

This exercise reinforced the importance of verifying directory locations through the terminal rather than relying entirely on memory or visual representations.

My original map also included a Library folder inside AutoTunePro. While I verified that the AutoTunePro directory exists, I did not independently confirm that specific Library subfolder. This showed me why it is important to verify each level of a directory path instead of assuming that every folder exists.
