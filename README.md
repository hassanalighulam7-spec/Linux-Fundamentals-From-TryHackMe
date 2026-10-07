# Linux-Fundamentals-From-TryHackMe
# Linux Fundamentals Part 1

**Platform:** [TryHackMe](https://tryhackme.com/room/linuxfundamentalspt15vm?utm_campaign=social_share&utm_medium=social&utm_content=room&utm_source=copy&sharerId=6ac5f6131d1a4c91cd8e4b38)
**Status:** ✅ Completed

## What is Linux?

Linux is an open-source operating system used widely on servers, cloud platforms, and security tools. It comes in many versions called **distributions** (distros), such as Ubuntu, Debian, Fedora, and Kali Linux. Most distros share the same core commands, so what I learn on one carries over to the others.

<img width="1366" height="655" alt="image" src="https://github.com/user-attachments/assets/6d10a871-d53e-4ed2-9bfa-a60be33e7a4a" />


## Commands Learned

| Command | What it does | Example |
|---------|--------------|---------|
| `echo` | Prints text to the terminal | `echo Hello` |
| `whoami` | Shows the current logged-in user | `whoami` |
| `ls` | Lists files and folders in the current directory | `ls` |
| `cd` | Changes the directory | `cd Documents` |
| `cat` | Displays the contents of a file | `cat note.txt` |
| `pwd` | Prints the current working directory | `pwd` |
| `find` | Searches for files by name | `find -name "*.txt"` |
| `grep` | Searches for text inside a file | `grep "error" access.log` |

## Searching for Files

**`find`** looks for files by name or pattern.

```bash
find -name passwd          # search the current directory for a file named passwd
find -name "*.txt"         # search for all .txt files (wildcard *)
find / -name passwd        # search the whole system
```

**`grep`** looks for specific text inside a file, which is very useful for reading large log files.

```bash
grep "81.143.211.90" access.log     # find every line containing this IP address
```

## Shell Operators

Operators let me combine commands or control where the output goes.

| Operator | Meaning | Example |
|----------|---------|---------|
| `&` | Runs a command in the background | `cp bigfile.txt copy.txt &` |
| `&&` | Runs the second command only if the first one succeeds | `cd Documents && ls` |
| `>` | Sends output to a file (overwrites the file) | `echo hello > file.txt` |
| `>>` | Sends output to a file (appends to the end) | `echo world >> file.txt` |

## Key Takeaways

- The terminal is faster and more powerful than a GUI once the basic commands are known.
- `>` overwrites a file while `>>` adds to it, so I need to be careful which one I use.
- `grep` and `find` are the commands I'll use most for investigating logs and files as a SOC Analyst.
- Wildcards (`*`) make searching much more flexible.

## Next

➡️ Linux Fundamentals Part 2: SSH, command flags, and file management.
