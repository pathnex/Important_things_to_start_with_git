# Steps to Start Practice Course with PathNex

## ✅ PART 1 — Create ONE GitHub Repository
# 1. Go to [github.com](https://github.com)
# 2. Login
# 3. Click `+` (top right) → New repository
# 4. Repository name: `Batch_Name_Pathnex` (e.g., `Dec2025_Neeraj_Pathnex`)
# 5. Select **Public**
# 6. **DO NOT** add README (optional)
# 7. Click **Create repository**

# Your GitHub repo is ready.

---

## ✅ PART 2 — Prepare Local Files (On Your Laptop)
Open your terminal (or Git Bash), then follow:

**Step 1 — Create project folder**
```bash

mkdir Batch_Name_Pathnex
cd Batch_Name_Pathnex

Step 2 — Create two folders
mkdir Timings
mkdir "Coding Practice"

Step 3 — Create today’s files
#Example file name: Day01-06-Dec-2025
#Inside Timings:
vim Timings/Day01-06-Dec-2025.txt

# Inside Coding Practice:
vim Coding\ Practice/Day01-06-Dec-2025.txt
# Add your content and save

# Folder structure:
# Batch_Name_Pathnex/
 ├── Timings/
 │     └── Day01-06-Dec-2025.txt
 └── Coding Practice/
       └── Day01-06-Dec-2025.txt


# PART 3 — Push to GitHub from Local

# Step 1 — Initialize Git
git init

# Step 2 — Add the remote GitHub repo
# Copy your GitHub repo URL (HTTPS) and run:
git remote add origin https://github.com/your-username/Batch_Name_Pathnex.git

# Step 3 — Add all files
git add .

# Step 4 — Commit
git commit -m "Added Day01 files in Timings and Coding Practice"

# Step 5 — Push
git branch -M main
git push -u origin main
# Congratulations — everything is uploaded to GitHub!
# NEXT DAY (Daily Routine)

# Create new files for today, e.g., Day02-07-Dec-2025.txt
# Inside both folders:
vim Day02-07-Dec-2025.txt
vim Day02-07-Dec-2025.txt

# Add → Commit → Push:
git add .
git commit -m "Added Day02 files"
git push

# Summary
# You will have:
# One GitHub repo
Batch_Name_Pathnex/
   ├── Timings/
   │     ├── Day01-06-Dec-2025.txt
   │     ├── Day02-07-Dec-2025.txt
   │     └── ...
   └── Coding Practice/
         ├── Day01-06-Dec-2025.txt
         ├── Day02-07-Dec-2025.txt
         └── ...