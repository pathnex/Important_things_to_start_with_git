✅ How to Push to GitHub from an EC2 Instance (Step-by-Step)
Below are complete steps so you can do it easily.


🟩 STEP 1 — Install Git on EC2
For Amazon Linux / RHEL / CentOS:
sudo yum install git -y
For Ubuntu:
sudo apt update
sudo apt install git -y


🟩 STEP 2 — Configure Git (Only once)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"


🟩 STEP 3 — Authenticate to GitHub (Two Options)
You have two ways to authenticate:
🔹 OPTION A (Recommended): SSH Key Method

1. Generate SSH key on EC2:
ssh-keygen -t ed25519 -C "your@email.com"
Press Enter for all prompts.
Your key will be stored here:
~/.ssh/id_ed25519
~/.ssh/id_ed25519.pub

2. Copy the public key:
cat ~/.ssh/id_ed25519.pub
Copy the output.

3. Add it to GitHub:
GitHub → Profile → Settings → SSH and GPG keys → New SSH Key → paste → Save.

4. Test connection:
ssh -T git@github.com
If you see:
Hi username! You've successfully authenticated.
You’re ready to push!


🔹 OPTION B: HTTPS + Personal Access Token
If you use HTTPS, GitHub requires a token, not a password.
Generate token:
GitHub → Settings → Developer settings → Personal access tokens → Generate token
Then use this when pushing.


🟩 STEP 4 — Clone Your Repo on EC2
Using SSH (recommended):
git clone git@github.com:yourname/yourrepo.git


🟩 STEP 5 — Make changes, add files, and commit
Example:
echo "Hello from EC2" > hello.txt

git add .
git commit -m "Added hello.txt from EC2"


🟩 STEP 6 — Push to GitHub
git push
🎉 Your code is now pushed from EC2 to GitHub!