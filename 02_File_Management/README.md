# Linux File Management

This section contains important Linux commands used to create, view, copy, move, rename, and delete files and directories.

## 1. pwd

Displays the current working directory.

```bash
pwd
```

Example output:

```text
/home/ubuntu
```

---

## 2. ls

Lists files and directories.

```bash
ls
```

Long listing format:

```bash
ls -l
```

Show hidden files:

```bash
ls -a
```

Show hidden files in long format:

```bash
ls -la
```

---

## 3. touch

Creates an empty file or updates the timestamp of an existing file.

Create one file:

```bash
touch file1.txt
```

Create multiple files:

```bash
touch file1.txt file2.txt file3.txt
```

Create numbered files:

```bash
touch file{1..10}.txt
```

---

## 4. mkdir

Creates a directory.

```bash
mkdir project
```

Create multiple directories:

```bash
mkdir frontend backend database
```

Create nested directories:

```bash
mkdir -p project/frontend/src
```

---

## 5. cd

Changes the current directory.

Move into a directory:

```bash
cd project
```

Move one level up:

```bash
cd ..
```

Move to the home directory:

```bash
cd ~
```

Move to the root directory:

```bash
cd /
```

---

## 6. cat

Displays the contents of a file.

```bash
cat file.txt
```

Create or overwrite a file using redirection:

```bash
cat > file.txt
```

Append content to an existing file:

```bash
cat >> file.txt
```

Press `Ctrl + D` after entering content.

---

## 7. head

Displays the first 10 lines of a file by default.

```bash
head file.txt
```

Display the first 5 lines:

```bash
head -n 5 file.txt
```

---

## 8. tail

Displays the last 10 lines of a file by default.

```bash
tail file.txt
```

Display the last 5 lines:

```bash
tail -n 5 file.txt
```

Monitor a log file continuously:

```bash
tail -f /var/log/syslog
```

---

## 9. cp

Copies files or directories.

Copy a file:

```bash
cp source.txt destination.txt
```

Copy a file to another directory:

```bash
cp file.txt /home/ubuntu/project/
```

Copy a directory recursively:

```bash
cp -r source-directory destination-directory
```

---

## 10. mv

Moves or renames files and directories.

Move a file:

```bash
mv file.txt /home/ubuntu/project/
```

Rename a file:

```bash
mv oldname.txt newname.txt
```

---

## 11. rm

Deletes files.

```bash
rm file.txt
```

Ask for confirmation before deleting:

```bash
rm -i file.txt
```

Delete a directory and its contents:

```bash
rm -r directory-name
```

Use this command carefully:

```bash
rm -rf directory-name
```

`rm -rf` deletes files recursively without confirmation.

---

## 12. rmdir

Deletes an empty directory.

```bash
rmdir empty-directory
```

It does not remove a directory containing files.

---

## 13. find

Searches for files and directories.

Search by name:

```bash
find /home -name "file.txt"
```

Search for directories:

```bash
find /home -type d -name "project"
```

Search for files:

```bash
find /home -type f -name "*.log"
```

Search by permission:

```bash
find / -type f -perm 0644
```

Search by size:

```bash
find / -type f -size +100M
```

---

## Practice Task

Perform these commands on a Linux machine:

```bash
mkdir -p devops/linux/files
cd devops/linux/files

touch app{1..5}.log
mkdir backup

cp app1.log backup/
mv app2.log application.log
ls -la
find . -name "*.log"
```

## Expected Learning

After completing this task, you should understand how to:

- Create files and directories
- Navigate between directories
- Copy and rename files
- Display file contents
- Search for files
- Delete files safely

- ---

# Practice Screenshot

Below is my hands-on Linux file management practice performed on an AWS EC2 instance.

![Linux File Management Practice](file-management-practice.png)
