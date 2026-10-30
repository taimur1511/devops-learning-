# Challenge 4: Backup Script for Text Files

Create a script that backs up all .txt files from one directory to another.
Requirements:
- Prompt user for source directory
- Create a backup directory if it doesn't exist
- Copy all .txt files to the backup directory
- Add timestamp to backup directory name
- Display count of files backed up


The script uses `read` to collect the source directory and `-d` to check that it exists. It then generates a timestamp using `date` and uses it to create a backup directory with `mkdir`.

The `cp` command copies all `.txt` files into the backup directory using the *.txt wildcard. Finally, `find` and `wc -l` count the copied files, storing the result in `file_count` which is displayed using `echo`.

<img width="2750" height="932" alt="image" src="https://github.com/user-attachments/assets/532b1dcf-093f-4786-92d3-da627eef9999" />
