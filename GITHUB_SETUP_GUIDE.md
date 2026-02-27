# 📦 GitHub Upload Guide — Amazon Prime Video Analysis

## Complete Step-by-Step Instructions for Kiran Rawat

---

## STEP 1: Install Git (if not already installed)

### Windows:
1. Go to https://git-scm.com/download/windows
2. Download and run the installer
3. Keep all default settings and click Next
4. Open "Git Bash" from your Start menu

### Mac:
Open Terminal and run:
```bash
xcode-select --install
```

### Check if Git is installed:
```bash
git --version
# Should show something like: git version 2.40.0
```

---

## STEP 2: Configure Git (one-time setup)

```bash
git config --global user.name "Kiran Rawat"
git config --global user.email "your-email@gmail.com"
```

---

## STEP 3: Create a GitHub Account (if needed)

1. Go to https://github.com
2. Click "Sign up"
3. Use your email and create a password
4. Verify your email

---

## STEP 4: Create a New Repository on GitHub

1. Log in to GitHub
2. Click the **"+"** button in the top-right corner
3. Click **"New repository"**
4. Fill in:
   - **Repository name**: `Amazon-Prime-Video-Dashboard-Analysis`
   - **Description**: `End-to-end data analysis of Amazon Prime Video content using Python EDA and Tableau dashboard`
   - **Visibility**: Public ✅ (so recruiters can see it)
   - ❌ Do NOT check "Add a README file" (we have our own)
5. Click **"Create repository"**

---

## STEP 5: Prepare Your Files

Create a folder on your computer called `amazon-prime-analysis` and put ALL of these files inside:

```
amazon-prime-analysis/
├── README.md                          ← (use the one provided)
├── .gitignore                         ← (use the one provided)
├── Capstone_project_2_EDA.ipynb       ← your Jupyter notebook
├── amazon_prime_titles.csv            ← your dataset
├── Amazon_Prime_Analysis_Report.pdf   ← the PDF report
└── dashboard_screenshot.png           ← screenshot of your Tableau dashboard
```

### How to take a dashboard screenshot:
1. Open your Tableau dashboard in the browser
2. Press `Ctrl + Shift + S` (Windows) or `Cmd + Shift + 4` (Mac)
3. Save as `dashboard_screenshot.png` in your project folder

---

## STEP 6: Upload to GitHub

Open Git Bash (Windows) or Terminal (Mac/Linux), then:

```bash
# 1. Navigate to your project folder
cd Desktop/amazon-prime-analysis
# (change the path to wherever your folder is)

# 2. Initialize git
git init

# 3. Add all files
git add .

# 4. Make your first commit
git commit -m "Initial commit: Amazon Prime Video content analysis"

# 5. Connect to your GitHub repository
#    (replace YOUR_USERNAME with your actual GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/Amazon-Prime-Video-Dashboard-Analysis.git

# 6. Rename branch to main
git branch -M main

# 7. Push to GitHub
git push -u origin main
```

---

## STEP 7: Verify It Worked

1. Go to `https://github.com/YOUR_USERNAME/Amazon-Prime-Video-Dashboard-Analysis`
2. You should see all your files listed
3. The README.md will automatically display below the files ✅

---

## STEP 8: Update Your Existing Repo (if adding to existing one)

If you want to add files to your EXISTING repository instead:

```bash
# Clone your existing repo
git clone https://github.com/kiranrawat-learning/Amazon-Prime-Video-DatasetEDA.git

# Go into the folder
cd Amazon-Prime-Video-DatasetEDA

# Copy your new files into this folder, then:
git add .
git commit -m "Add README, PDF report, and dashboard screenshot"
git push
```

---

## STEP 9: Make Your Profile Look Great (Optional but Recommended)

### Pin the repository:
1. Go to your GitHub profile page
2. Click "Customize your pins"
3. Check the Amazon Prime Video project
4. Click Save — it will now appear on your profile!

### Add topics to your repo:
1. Open the repository on GitHub
2. Click the gear icon ⚙️ next to "About"
3. Add topics like: `data-analysis`, `tableau`, `python`, `eda`, `amazon-prime`, `pandas`, `visualization`
4. Click Save

---

## ❓ Common Issues & Fixes

| Problem | Solution |
|---------|----------|
| `git: command not found` | Install Git from git-scm.com |
| `Permission denied` | Use `git remote set-url origin https://YOUR_TOKEN@github.com/...` |
| `File too large` | Add large files to `.gitignore`, or use Git LFS |
| `Repository already exists` | Use `git remote set-url` instead of `git remote add` |
| Authentication failed | Go to GitHub → Settings → Developer Settings → Personal Access Tokens → Generate new token |

---

## 🔑 If GitHub Asks for Password (Token Authentication)

GitHub no longer accepts passwords. Use a Personal Access Token instead:

1. Go to GitHub → click your profile photo → **Settings**
2. Scroll down to **Developer settings** → **Personal access tokens** → **Tokens (classic)**
3. Click **Generate new token (classic)**
4. Select scopes: check **repo**
5. Click **Generate token**
6. Copy the token (you won't see it again!)
7. Use this token as your "password" when Git prompts you

---

*You're all set! 🚀 Your project is now live on GitHub.*
