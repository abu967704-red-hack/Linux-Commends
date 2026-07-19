# File and Directory Commands

## pwd

### কাজ
বর্তমান Directory দেখায়।

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

Burp Suite, Wordlist অথবা Script কোন Directory-তে আছে তা জানার জন্য।

---

## ls

### কাজ

Directory-এর ভিতরের File ও Folder দেখায়।

### Syntax

```bash
ls
```

### Example

```bash
ls
ls -la
```

### Ethical Hacking Use

Payload, Script, Scan Result এবং Wordlist দেখার জন্য।

---

## cd

### কাজ

Directory পরিবর্তন করে।

### Example

```bash
cd Desktop
cd ..
```

### Ethical Hacking Use

একটি Tool-এর Folder-এ প্রবেশ করার জন্য।

---
ls -l
কাজ

ফাইল ও ফোল্ডারের বিস্তারিত তথ্য দেখায়।

Syntax
ls -l
Example
ls -l
Example Output
drwxr-xr-x 2 kali kali 4096 Jul 20 Documents
-rw-r--r-- 1 kali kali  120 Jul 20 notes.txt
4. ls -a
কাজ

Hidden File-সহ সব ফাইল ও ফোল্ডার দেখায়।

Syntax
ls -a
Example
ls -a
Example Output
.
..
.bashrc
.profile
notes.txt
5. cd
কাজ

এক Directory থেকে অন্য Directory-তে যাওয়ার জন্য ব্যবহৃত হয়।

Syntax
cd directory_name
Example
cd Documents
Example Output
/home/kali/Documents
6. cd ..
কাজ

এক ধাপ উপরের Directory-তে যায়।

Syntax
cd ..
Example
cd ..
Example Output
/home/kali
7. cd ~
কাজ

বর্তমান User-এর Home Directory-তে নিয়ে যায়।

Syntax
cd ~
Example
cd ~
Example Output
/home/kali
8. mkdir
কাজ

নতুন Directory তৈরি করে।

Syntax
mkdir directory_name
Example
mkdir project
Example Output
project/
9. rmdir
কাজ

খালি Directory মুছে ফেলে।

Syntax
rmdir directory_name
Example
rmdir project
Example Output
(No output if successful)
10. rm
কাজ

একটি File মুছে ফেলে।

Syntax
rm filename
Example
rm notes.txt
Example Output
(No output if successful)
11. rm -r
কাজ

Directory এবং তার ভিতরের সব File ও Subdirectory মুছে ফেলে।

Syntax
rm -r directory_name
Example
rm -r project
Example Output
(No output if successful)
12. rm -rf
কাজ

Force করে Directory ও তার সবকিছু মুছে ফেলে।

Syntax
rm -rf directory_name
Example
rm -rf project
Example Output
(No output if successful)
13. touch
কাজ

নতুন খালি File তৈরি করে।

Syntax
touch filename
Example
touch notes.txt
Example Output
notes.txt
14. cp
কাজ

File কপি করে।

Syntax
cp source destination
Example
cp notes.txt backup.txt
Example Output
notes.txt
backup.txt
15. cp -r
কাজ

Directory কপি করে।

Syntax
cp -r source_directory destination_directory
Example
cp -r project backup
Example Output
backup/
16. mv
কাজ

File বা Directory Move অথবা Rename করে।

Syntax
mv source destination
Example
mv old.txt new.txt
Example Output
new.txt
17. find
কাজ

নির্দিষ্ট File বা Directory খুঁজে বের করে।

Syntax
find path -name "filename"
Example
find . -name "notes.txt"
Example Output
./notes.txt
18. locate
কাজ

দ্রুত File খুঁজে বের করে।

Syntax
locate filename
Example
locate notes.txt
Example Output
/home/kali/Documents/notes.txt
19. tree
কাজ

Directory Structure Tree আকারে দেখায়।

Syntax
tree
Example
tree
Example Output
.
├── Documents
├── Downloads
└── notes.txt

2 directories, 1 file
20. stat
কাজ

File-এর বিস্তারিত Metadata দেখায়।

Syntax
stat filename
Example
stat notes.txt
Example Output
Size: 120
Access: 2026-07-20
Modify: 2026-07-20
Owner: kali
21. file
কাজ

File-এর ধরন (File Type) নির্ণয় করে।

Syntax
file filename
Example
file image.jpg
Example Output
image.jpg: JPEG image data
22. du
কাজ

File বা Directory কত Disk Space ব্যবহার করছে তা দেখায়।

Syntax
du -sh directory_name
Example
du -sh Downloads
Example Output
2.5G Downloads
23. df
কাজ

Disk-এর মোট, ব্যবহৃত এবং খালি Space দেখায়।

Syntax
df -h
Example
df -h
Example Output
Filesystem      Size Used Avail Use%
/dev/sda1        80G  30G   50G  38%
