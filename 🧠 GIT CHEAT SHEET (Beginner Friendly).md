🧠 GIT CHEAT SHEET (Beginner Friendly)
🔹 1. Setup Git (Only once)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
Check config:
git config --list
🔹 2. Start a New Project (Initialize Git)
git init
🔹 3. Check Status of Files
git status
🔹 4. Add Files to Staging Area
Add one file:
git add filename
Add ALL files:
git add .
🔹 5. Commit Files
git commit -m "Your commit message"
🔹 6. Connect Local Repo to GitHub
git remote add origin https://github.com/username/reponame.git
Check remote:
git remote -v
🔹 7. Push Code to GitHub
First push:
git branch -M main
git push -u origin main
Next pushes:
git push
🔹 8. Pull Latest Changes from GitHub
git pull
🔹 9. Clone a Repository
git clone https://github.com/username/reponame.git
🔹 10. View Commit History
git log
Simple view:
git log --oneline
🔹 11. Create and Switch Branch
Create branch:
git branch feature1
Switch to branch:
git checkout feature1
Create + Switch (shortcut):
git checkout -b feature1
🔹 12. Merge a Branch
Switch to main:
git checkout main
Merge:
git merge feature1
🔹 13. Delete a Branch
git branch -d feature1
🔹 14. Undo Mistakes
Undo staged file:
git reset filename
Undo commit (keep changes):
git reset --soft HEAD~1
Undo commit (discard changes):
git reset --hard HEAD~1
🔹 15. Remove a File from Repo
Delete file from repo AND local:
git rm filename
git commit -m "Removed file"
git push
Just remove from Git but keep locally:
git rm --cached filename
🔥 QUICK DAILY WORKFLOW (Most Used)
git add .
git commit -m "Updated day files"
git push
