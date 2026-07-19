# Linux File & Directory Management Commands

এই Repository-তে Linux-এর গুরুত্বপূর্ণ **File & Directory Management Commands** উদাহরণসহ ব্যাখ্যা করা হয়েছে। প্রতিটি Command-এর সাথে Syntax, Example, Output এবং Ethical Hacking-এ এর ব্যবহার উল্লেখ করা হয়েছে।

---

# Table of Contents

- pwd
- ls
- ls -l
- ls -a
- cd
- cd ..
- cd ~
- mkdir
- rmdir
- rm
- rm -r
- rm -rf
- touch
- cp
- cp -r
- mv
- find
- locate
- tree
- stat
- file
- du
- df

---

## `pwd`

### কাজ

বর্তমান (Current) Directory-এর সম্পূর্ণ Path দেখায়।

### Syntax

```bash
pwd
```

### Example

```bash
pwd
```

### Example Output

```text
/home/kali/Linux-Commands
```

### Ethical Hacking Use

Burp Suite Project, Wordlist অথবা Script কোন Directory-তে আছে তা জানার জন্য।

---

## `ls`

### কাজ

বর্তমান Directory-এর ভিতরের File ও Folder-এর তালিকা দেখায়।

### Syntax

```bash
ls
```

### Example

```bash
ls
```

### Example Output

```text
Documents
Downloads
notes.txt
script.py
```

### Ethical Hacking Use

Wordlist, Payload, Script এবং Scan Report দ্রুত দেখার জন্য।

---

## `ls -l`

### কাজ

File ও Folder-এর বিস্তারিত তথ্য দেখায়।

### Syntax

```bash
ls -l
```

### Example

```bash
ls -l
```

### Example Output

```text
drwxr-xr-x 2 kali kali 4096 Jul 20 Documents
-rw-r--r-- 1 kali kali 120 Jul 20 notes.txt
```

### Ethical Hacking Use

File Permission, Owner, Size এবং Modification Time দেখার জন্য।

---

## `ls -a`

### কাজ

Hidden File-সহ সব File ও Folder দেখায়।

### Syntax

```bash
ls -a
```

### Example

```bash
ls -a
```

### Example Output

```text
.
..
.bashrc
.profile
notes.txt
```

### Ethical Hacking Use

Hidden Configuration File যেমন `.bashrc`, `.git`, `.ssh` ইত্যাদি দেখার জন্য।

---

## `cd`

### কাজ

এক Directory থেকে অন্য Directory-তে যাওয়ার জন্য ব্যবহৃত হয়।

### Syntax

```bash
cd directory_name
```

### Example

```bash
cd Documents
```

### Example Output

```text
/home/kali/Documents
```

### Ethical Hacking Use

Project Folder, Wordlist Folder অথবা Tool Directory-তে যাওয়ার জন্য।

---

## `cd ..`

### কাজ

এক ধাপ উপরের Directory-তে যায়।

### Syntax

```bash
cd ..
```

### Example

```bash
cd ..
```

### Example Output

```text
/home/kali
```

### Ethical Hacking Use

দ্রুত Parent Directory-তে ফিরে যাওয়ার জন্য।

---

## `cd ~`

### কাজ

বর্তমান User-এর Home Directory-তে নিয়ে যায়।

### Syntax

```bash
cd ~
```

### Example

```bash
cd ~
```

### Example Output

```text
/home/kali
```

### Ethical Hacking Use

যেকোনো অবস্থান থেকে দ্রুত Home Directory-তে যাওয়ার জন্য।

---

## `mkdir`

### কাজ

নতুন Directory তৈরি করে।

### Syntax

```bash
mkdir directory_name
```

### Example

```bash
mkdir project
```

### Example Output

```text
project/
```

### Ethical Hacking Use

Pentesting Project, Notes অথবা Lab Folder তৈরি করার জন্য।

---

## `rmdir`

### কাজ

খালি Directory মুছে ফেলে।

### Syntax

```bash
rmdir directory_name
```

### Example

```bash
rmdir project
```

### Example Output

```text
(No output if successful)
```

### Ethical Hacking Use

অপ্রয়োজনীয় Empty Directory মুছে ফেলার জন্য।

---

## `rm`

### কাজ

একটি File মুছে ফেলে।

### Syntax

```bash
rm filename
```

### Example

```bash
rm notes.txt
```

### Example Output

```text
(No output if successful)
```

### Ethical Hacking Use

অপ্রয়োজনীয় Script, Log File অথবা Payload মুছে ফেলার জন্য।

---

## `rm -r`

### কাজ

Directory এবং তার ভিতরের সব File ও Folder মুছে ফেলে।

### Syntax

```bash
rm -r directory_name
```

### Example

```bash
rm -r project
```

### Example Output

```text
(No output if successful)
```

### Ethical Hacking Use

পুরো Project Folder বা Test Environment মুছে ফেলার জন্য।

---

## `rm -rf`

### কাজ

Force করে Directory এবং তার ভিতরের সবকিছু মুছে ফেলে।

### Syntax

```bash
rm -rf directory_name
```

### Example

```bash
rm -rf project
```

### Example Output

```text
(No output if successful)
```

### Ethical Hacking Use

সতর্কতার সাথে বড় Project বা Temporary Directory দ্রুত মুছে ফেলার জন্য।

> ⚠️ Warning: `rm -rf` ভুলভাবে ব্যবহার করলে গুরুত্বপূর্ণ Data স্থায়ীভাবে মুছে যেতে পারে।

---

## `touch`

### কাজ

নতুন খালি File তৈরি করে।

### Syntax

```bash
touch filename
```

### Example

```bash
touch notes.txt
```

### Example Output

```text
notes.txt
```

### Ethical Hacking Use

Python Script, Notes অথবা Log File তৈরির জন্য।

---

## `cp`

### কাজ

File কপি করে।

### Syntax

```bash
cp source destination
```

### Example

```bash
cp notes.txt backup.txt
```

### Example Output

```text
backup.txt
```

### Ethical Hacking Use

Backup তৈরি করার জন্য।

---

## `cp -r`

### কাজ

Directory কপি করে।

### Syntax

```bash
cp -r source_directory destination_directory
```

### Example

```bash
cp -r project backup
```

### Example Output

```text
backup/
```

### Ethical Hacking Use

সম্পূর্ণ Project Backup রাখার জন্য।

---

## `mv`

### কাজ

File অথবা Directory Move বা Rename করে।

### Syntax

```bash
mv source destination
```

### Example

```bash
mv old.txt new.txt
```

### Example Output

```text
new.txt
```

### Ethical Hacking Use

Script Rename অথবা অন্য Folder-এ Move করার জন্য।

---

## `find`

### কাজ

File অথবা Directory খুঁজে বের করে।

### Syntax

```bash
find path -name "filename"
```

### Example

```bash
find . -name "notes.txt"
```

### Example Output

```text
./notes.txt
```

### Ethical Hacking Use

Wordlist, Log File অথবা Python Script খুঁজে বের করার জন্য।

---

## `locate`

### কাজ

দ্রুত File খুঁজে বের করে।

### Syntax

```bash
locate filename
```

### Example

```bash
locate notes.txt
```

### Example Output

```text
/home/kali/Documents/notes.txt
```

### Ethical Hacking Use

System-এর যেকোনো File দ্রুত খুঁজে বের করার জন্য।

---

## `tree`

### কাজ

Directory Structure Tree আকারে দেখায়।

### Syntax

```bash
tree
```

### Example

```bash
tree
```

### Example Output

```text
.
├── Documents
├── Downloads
└── notes.txt

2 directories, 1 file
```

### Ethical Hacking Use

Project Structure বোঝার জন্য।

---

## `stat`

### কাজ

File-এর বিস্তারিত Metadata দেখায়।

### Syntax

```bash
stat filename
```

### Example

```bash
stat notes.txt
```

### Example Output

```text
Size: 120
Access: Jul 20
Modify: Jul 20
Owner: kali
```

### Ethical Hacking Use

Timestamp, Permission এবং Ownership যাচাই করার জন্য।

---

## `file`

### কাজ

File-এর প্রকৃত Type নির্ণয় করে।

### Syntax

```bash
file filename
```

### Example

```bash
file image.jpg
```

### Example Output

```text
image.jpg: JPEG image data
```

### Ethical Hacking Use

Unknown File-এর আসল ধরন শনাক্ত করার জন্য।

---

## `du`

### কাজ

File অথবা Directory কত Disk Space ব্যবহার করছে তা দেখায়।

### Syntax

```bash
du -sh directory_name
```

### Example

```bash
du -sh Downloads
```

### Example Output

```text
2.5G Downloads
```

### Ethical Hacking Use

বড় Wordlist, Capture File অথবা Report কত Space নিচ্ছে তা জানার জন্য।

---

## `df`

### কাজ

Disk-এর মোট, ব্যবহৃত এবং খালি Space দেখায়।

### Syntax

```bash
df -h
```

### Example

```bash
df -h
```

### Example Output

```text
Filesystem      Size Used Avail Use%
/dev/sda1        80G 30G 50G 38%
```

### Ethical Hacking Use

Capture File, VM অথবা Tool Install করার আগে পর্যাপ্ত Disk Space আছে কিনা যাচাই করার জন্য।

---

# ⭐ If you found this repository helpful, don't forget to give it a Star!
