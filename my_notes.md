# study material

# Git and GitHub Learning Guide

You can create a brand new file (for example, git_guide.txt or steps.md) so it sits neatly in your repository files section.

##Create and open the new file in your terminal:```nano my_notes.txt```

This repository contains my study materials and notes on how to link a local terminal to GitHub.

## 1. How I Created the Repository
1. Logged into GitHub.com.
2. Clicked the `+` icon -> **New repository**.
3. Named it `study_material`.
4. Kept it completely blank (did not check README, .gitignore, or license).
5. Copied the HTTPS repository URL.

## 2. Where I Actually Wrote the Code
I opened the default **Terminal app on my computer** (Ubuntu/Linux bash terminal).

## 3. How I Linked the Terminal to GitHub
How I connected the terminal to GitHub:
   - Opened terminal and went to my Desktop:``` cd Desktop```
   - Created a clean project folder:``` mkdir study_material```
   - Entered the folder:``` cd study_material```
   - Started Git tracking:``` git init```
   - Set the branch:``` git branch -M main```
   - Linked to my GitHub URL:``` git remote add origin <MY_URL>```

in the MY_URL section  we have to paste the link which we copied earlier

## 4. What Went Wrong (My Mistakes & Solutions)
 I originally ran `git init` and `git add .` directly in my main home directory (`/home/ashish/`). This caused the terminal to freeze because it tried to track every file on my computer, including deleted files in the Trash folder.
   - I fixed it by pressing Ctrl + C, closing the terminal, and typing ``'rm -rf .git``' in the home directory to delete the accidental tracking.
11
## 5. How to Push Updates to GitHub
Every time I write new code or update these notes, I run these three commands in my terminal:
1. `git add .` (Stages the changes)
2. `git commit -m "Your update message"` (Saves a snapshot)
3. `git push` (Uploads it to GitHub)

Save and close the file by pressing Ctrl + O, then Enter, then Ctrl + X.

##Push it to GitHub using your standard routine:
```git add my_notes.txt
git commit -m "Added my personal setup steps guide"
git push```
