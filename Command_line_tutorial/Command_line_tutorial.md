### Self-Guided Command Line Tutorial (Beginner - Windows Git Bash - 20 minutes)

Welcome! You're about to learn the basics of navigating and managing files using the command line. This tutorial is designed for beginners and will take about 20 minutes. You have Git Bash open in VS Code, so let's get started.

#### 1. Know Where You Are: `pwd` (Print Working Directory) - 1 minute

Your first command tells you which folder you're currently in.

```bash
pwd
```

Type this and press Enter. You'll see a path like `/c/Users/Emily Wilson/Downloads`. This is your **current working directory** — think of it as your current location in the file system.

**Try it now:** Run `pwd` in your terminal.

#### 2. List Files and Folders: `ls` (List) - 2 minutes

Now let's see what's in your current folder.

```bash
ls
```

This shows all files and folders in your current location.

**Useful flags:**
- `ls -l` — shows details (file size, date, permissions)
- `ls -a` — shows hidden files (those starting with a dot, like `.ssh`)
- `ls -la` — combines both; shows detailed view including hidden files

**Try it now:** Run `ls`, then `ls -la`, and notice the difference.

#### 3. Navigate Folders: `cd` (Change Directory) - 3 minutes

Move into a folder using `cd`:

```bash
cd Documents
```

Now run `pwd` again — you've moved into the Documents folder. To go back up one level (to your parent folder):

```bash
cd ..
```

To jump directly to your home directory from anywhere:

```bash
cd ~
```

**Try it now:** 
1. Run `cd Documents` (or any folder you see from `ls`)
2. Run `pwd` to confirm you moved
3. Run `cd ..` to go back
4. Run `pwd` again

#### 4. Tab Completion: Your Keyboard Shortcut - 2 minutes

This is a game-changer. Instead of typing full folder or file names, type the first few letters and press **Tab**.

```bash
cd Doc[TAB]
```

Git Bash will auto-complete `Doc` to `Documents` (or whatever matches). If multiple options exist, press **Tab** twice to see them all.

**Try it now:** Start typing `cd D` and press Tab — it should auto-complete.

#### 5. Make a New Folder: `mkdir` (Make Directory) - 2 minutes

Create a new folder:

```bash
mkdir test_folder
```

Verify it was created:

```bash
ls
```

You should see `test_folder` in the list.

**Try it now:** Run `mkdir my_first_folder` then `ls` to confirm.

#### 6. Create a New File: `touch` - 2 minutes

Create an empty file:

```bash
touch my_file.txt
```

Verify it exists:

```bash
ls
```

You should see `my_file.txt` in your list.

**Try it now:** Run `touch test.txt` then `ls`.

#### 7. Copy Files: `cp` (Copy) - 2 minutes

Copy a file from one location to another:

```bash
cp my_file.txt my_file_copy.txt
```

This creates a duplicate of `my_file.txt` called `my_file_copy.txt` in the same folder.

To copy into a subfolder:

```bash
cp my_file.txt test_folder/
```

**Try it now:** Run `cp test.txt test_copy.txt` then `ls`.

#### 8. Move or Rename Files: `mv` (Move) - 2 minutes

Rename a file by "moving" it to a new name:

```bash
mv my_file.txt renamed_file.txt
```

Or move a file into a folder:

```bash
mv renamed_file.txt test_folder/
```

**Try it now:** Run `mv test.txt moved_test.txt` then `ls`.

#### 9. Remove Files: `rm` (Remove) - 2 minutes

Delete a file (this is permanent):

```bash
rm moved_test.txt
```

To delete a folder and everything inside it (use with caution!):

```bash
rm -r test_folder
```

The `-r` flag means "recursive" (delete the folder and all its contents).

**Try it now:** Run `rm test_copy.txt` then `ls` to confirm it's gone.

#### 10. Get Help: `--help` and `man` - 1 minute

Confused about a command? Ask for help:

```bash
ls --help
```

This shows all the flags and options for the `ls` command. Try it for any command:

```bash
cp --help
mkdir --help
cd --help
```

**Try it now:** Run `ls --help` and scroll through the options. You'll see all the flags we mentioned.

---

**Challenge (optional):**
Now practice everything together:
1. Create a folder: `mkdir my_project`
2. Navigate into it: `cd my_project`
3. Create a file: `touch README.md`
4. Create another file: `touch data.txt`
5. List contents: `ls`
6. Copy the file: `cp README.md README_backup.md`
7. Move it into a new subfolder: `mkdir backup` then `mv README_backup.md backup/`
8. List contents of the backup folder: `ls backup`
9. Delete the original: `rm README.md`
10. Go back and clean up: `cd ..` then `rm -r my_project`

**Congratulations!** You now know the basics of command-line file management. These commands form the foundation for everything you'll do on the HPC and in software development.
