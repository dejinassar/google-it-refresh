# Recap - August 4, 2025

---

## Linux Folder Structure

**Key directories and what they do:**

| Folder | Description |
|---|---|
| `/` | Root of the entire filesystem |
| `/home` | Contains personal directories for users |
| `/etc` | Configuration files (e.g. `/etc/passwd`) |
| `/bin` | Essential binary programs (`ls`, `cp`, etc) |
| `/usr` | User-installed apps and utilities |
| `/var` | Logs, temporary files, etc. |
| `/tmp` | Temporary files, wiped after reboot |
| `/root` | Home directory for the root user |

**Practice Commands:**
```bash
ls /
cd /etc
tree / -L 1       # View structure one level deep

Linux User & Group Management
Create a New User

sudo adduser student1

Modify an Existing User


sudo usermod -aG sudo student1        # Add to sudo group
sudo usermod -l newname student1      # Rename user
Create and Assign Group


sudo groupadd devops
sudo usermod -aG devs student1        # Add user to group
View Users and Groups


cat /etc/passwd         # List all users
cat /etc/group          # List all groups
groups student1         # See groups for student1
Password Management


sudo passwd student1     # Set or change user password
sudo passwd -l student1  # Lock user account
Practical Linux Command Practice


ls -la                # List all files (including hidden)
pwd                   # Show current directory
cd /etc               # Move to /etc
mkdir testfolder      # Create a directory
rm -r testfolder      # Delete a directory
touch file.txt        # Create a file
nano file.txt         # Edit file using nano
cat file.txt          # Display file contents
SSH — Secure Shell
What is SSH?
SSH (Secure Shell) allows secure terminal access to a remote computer.

Basic SSH Usage

ssh username@ip_address
Example:

ssh biola@192.168.1.114
Common Issues & Fixes
Connection Refused

➤ Cause: SSH server not installed or not running

➤ Fix:

sudo apt install openssh-server
sudo systemctl start ssh
Permission Denied

➤ Cause: Wrong username or password

Host Key Not Found

➤ Fix: First-time connection — type yes to proceed

Useful Extras

hostname -I     # Show IP address
whoami          # Show current user
exit            # Exit remote session
What I Achieved Today
Understood the Linux folder structure

Practiced real Linux terminal commands

Created users and groups from the terminal

Set and locked user passwords

Connected to another machine using SSH

Started documenting my DevOps learning journey