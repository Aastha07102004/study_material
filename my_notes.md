# Git and GitHub Learning Guide

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
* Opened terminal and went to my Desktop: `cd Desktop`
* Created a clean project folder: `mkdir study_material`
* Entered the folder: `cd study_material`
* Started Git tracking: `git init`
* Set the branch: `git branch -M main`
* Linked to my GitHub URL: `git remote add origin https://github.com/Aastha07102004/study_material`

## 4. What Went Wrong (My Mistakes & Solutions)
* I originally ran `git init` and `git add .` directly in my main home directory (`/home/ashish/`). This caused the terminal to freeze because it tried to track every file on my computer.
* I fixed it by pressing `Ctrl + C`, closing the terminal, and typing `rm -rf .git` in the home directory to delete the accidental tracking.

## 5. How to Push Updates to GitHub
Every time I write new code or update these notes, I run these three commands in my terminal:
1. `git add .` (Stages the changes)
2. `git commit -m "Your update message"` (Saves a snapshot)
3. `git push -u origin main` (Uploads it to GitHub)

If this shows an error, use `echo "study material" > my_notes.md` to reset, then repeat the `git add`, `git commit`, and `git push` steps.
Open your file anytime with `nano my_notes.md`.
Save and close the file inside nano by pressing `Ctrl + O`, then `Enter`, then `Ctrl + X`.

if you want to edit the existing repo where the notes is taken in nano so to open the existing nano and edit the content in it these are the steps
 
## Part 1: Your Daily Workflow (Open and Edit)
Whenever you open your computer to continue working, run these commands in order:
* **Step 1:** Open your repository folder: `cd ~/Desktop/study_material`
* **Step 2:** Open and edit your file in Nano: `nano my_notes.md`
* **Step 3:** Save and Exit Nano: Press `Ctrl + O` then press `Enter` to save your changes. Press `Ctrl + X` to exit the Nano editor screen.

## Part 2: Saving Your Changes to GitHub
Once you are done editing and want your changes to show up on the GitHub website, run these three commands in your terminal one after another:
* **Step 1:** Stage all your modified text: `git add .`
* **Step 2:** Write a descriptive save note: `git commit -m "Updated my notes"`
* **Step 3:** Send the changes safely up to your online profile: `git push -u origin main --force`
