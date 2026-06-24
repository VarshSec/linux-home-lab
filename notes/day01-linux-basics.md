# Day 1 — Linux Basics

## Objective

Learn the fundamentals of Linux navigation, filesystem structure, hidden files, and basic terminal commands.

---

## What is Linux?

Linux is an open-source operating system widely used in:

* Web servers
* Cloud infrastructure
* Cybersecurity
* Embedded systems
* Supercomputers

Most cybersecurity tools are designed to run on Linux.

Examples:

* Kali Linux
* Ubuntu
* Debian
* Fedora
* Arch Linux

---

## Linux Filesystem Hierarchy

Linux uses a hierarchical filesystem that starts from the root directory:

```text
/
```

### Important Directories

#### /

Root directory of the entire operating system.

All files and folders originate from here.

#### /home

Contains user home directories.

Example:

```text
/home/kali
/home/varshit
```

#### /root

Home directory of the root user (administrator).

#### /etc

Contains configuration files.

Examples:

```text
/etc/passwd
/etc/hosts
```

#### /var

Stores logs and frequently changing data.

Examples:

```text
/var/log
```

#### /tmp

Temporary files.

#### /usr

Contains installed programs and utilities.

#### /bin

Essential system commands.

Examples:

```text
ls
cp
mv
cat
```

---

## Absolute vs Relative Paths

### Absolute Path

Starts from the root directory.

Example:

```text
/home/kali/Documents
```

Always points to the same location.

### Relative Path

Starts from the current directory.

Example:

```text
Documents
```

Depends on where you currently are.

---

## Commands Learned

### pwd

Print Working Directory.

Shows current location.

Example:

```bash
pwd
```

Output:

```text
/home/kali
```

---

### ls

Lists files and directories.

Example:

```bash
ls
```

---

### ls -la

Shows:

* Hidden files
* Permissions
* Owner
* Size
* Detailed information

Example:

```bash
ls -la
```

---

### cd

Change directory.

Examples:

```bash
cd /
cd ~
cd Documents
```

---

### cd ..

Move one directory up.

Example:

```text
/home/kali
```

becomes

```text
/home
```

---

### cd ~

Return to the user's home directory.

Example:

```text
/home/kali
```

---

### cd /

Move directly to the root directory.

---

### file

Identifies file type.

Example:

```bash
file access.log
```

Possible output:

```text
ASCII text
empty
directory
ELF executable
```

Useful during penetration testing when investigating unknown files.

---

### clear

Clears the terminal screen.

```bash
clear
```

---

## Hidden Files

Files beginning with a dot (.) are hidden.

Examples:

```text
.zshrc
.bashrc
.gitconfig
.ssh
```

View hidden files:

```bash
ls -la
```

### Why Hidden Files Matter

They often contain:

* SSH keys
* Configuration files
* Command history
* API keys
* Credentials

Common targets during security assessments.

---

## Practical Exercises Completed

### Terminal Navigation

Practiced:

```bash
pwd
ls
ls -la
cd
cd ..
cd ~
cd /
```

### File Investigation

Practiced:

```bash
file access.log
```

### Hidden Files

Explored hidden files using:

```bash
ls -la
```

---

## Cybersecurity Relevance

Linux is the foundation of:

* Penetration Testing
* Bug Bounty Hunting
* Cloud Security
* Digital Forensics
* Malware Analysis

Understanding Linux navigation is required before learning:

* Nmap
* Burp Suite
* Metasploit
* Wireshark
* Privilege Escalation
* Web Application Security

---

## Key Takeaways

1. Linux uses a hierarchical filesystem beginning at `/`.
2. `pwd` shows current location.
3. `ls` lists files.
4. `ls -la` reveals hidden files and details.
5. `cd` changes directories.
6. Hidden files often contain sensitive information.
7. Linux skills are essential for cybersecurity professionals.
