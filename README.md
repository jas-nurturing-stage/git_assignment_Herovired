# 🚀 Step-by-Step Git Workflow Guide

## 📜 Project Description
This project is a **Git Assignment** for managing a **basic calculator and geometry calculator** using **Git best practices**. The repository follows a structured branching strategy and includes features like Git LFS for handling large files.

---

## 🛠️ Prerequisites
Before starting, ensure you have:
- ✅ Installed **Git** ([Download here](https://git-scm.com/downloads))
- ✅ Installed **Git LFS** (`git lfs install`)
- ✅ A **GitHub account**
- ✅ Basic knowledge of **Git commands**
- ✅ Python installed (`python --version` to check)

---

## 📂 Folder Structure
```
📦 git_assignment_HeroVired
 ┃ 📜 calculator.py
 ┃ 📜 geometry_calculator.py
 ┣ 📜 README.md
 
```

---

## 📝 1. Create a GitHub Repository
### 📂 Log in to GitHub & Create a New Repository
- **Sign in** to your GitHub account.
- Click on the ➕ **"+"** sign in the top right corner.
- Select **"New repository"** from the dropdown.
- **Enter repository details:**
  - **📂 Repository Name:** `git_assignment_HeroVired`
  - **📝 Description (Optional):** Add a short description.
  - **🔒 Visibility:** Set to **Private** (only you and collaborators can see it).
- **Initialize the repository:**
  - ✅ Check **"Add a README file"** (recommended).
  - ✅ Optionally, add a **.gitignore** file if needed.
- **💾 Click "Create repository"** to finalize the setup.

---

## 🌿 2. Clone the Repository
```bash
git clone (https://github.com/jas-nurturing-stage/git_assignment_Herovired.git)
cd git_assignment_HeroVired
```

---

## 🔀 3. Create and Switch to the `dev` Branch
```bash
git checkout -b dev
```

---

## 📂 4. Add Your Code to the Repository
### ✍️ Create `src/calculator.py` and Add Code:
```python
import math
class Calculator:
    def add(self, a, b):
        return a + b

    def subtract(self, a, b):
        return a - b

    def multiply(self, a, b):
        return a * b

    def divide(self, a, b):
        return a / b

if __name__ == "__main__":
    calculator = Calculator()
    num1 = 16
    num2 = 4
    print(f"{num1} + {num2} = {calculator.add(num1, num2)}")
    print(f"{num1} - {num2} = {calculator.subtract(num1, num2)}")
    print(f"{num1} * {num2} = {calculator.multiply(num1, num2)}")
    print(f"{num1} / {num2} = {calculator.divide(num1, num2)}")
```
### ✅ Add & Commit Changes:
```bash
git add .
git commit -m "Added initial code to dev branch"
```

---

## 🚀 5. Push `dev` Branch to Remote Repository
```bash
git push origin dev
```

---

## 🔀 6. Merge `dev` into `main` & Release Version 1️⃣
```bash
git checkout main
git merge dev
git push origin main
git tag v1.0
git push origin v1.0
```

---

## 👥 Add a Collaborator
### 📌 Adding **Uthkarsha** as a Collaborator
1. **⚙️ Open Repository Settings:**
   - Navigate to your repository.
   - Click on the **"Settings"** tab.
   - In the left sidebar, go to **"Collaborators"**.
2. **➕ Add a Collaborator:**
   - Click "Add people".
   - Enter **Uthkarsha's** GitHub username or email.
   - Click ✅ "Add" to send an invite.
3. **📩 Wait for Acceptance:**
   - Uthkarsha will receive an email invitation.
   - Once accepted, their name will appear under **Collaborators**.

---

## 🚀 Implement a Square Root Feature in Git
### 🌿 Create a New Branch
```bash
git checkout -b feature/sqrt
```
### ✨ Add the Square Root Function in `src/calculator.py`
```python
import math
class Calculator:
    def square_root(self, x):
        return math.sqrt(x)

num3 = 25
print(f"The square root of {num3} = {calculator.square_root(num3)}")
```
### 📌 Commit & Push Changes:
```bash
git add .
git commit -m "✨ Implement square root function"
git push origin feature/sqrt
```

---

## 🚀 Final Testing & Releasing Version 2️⃣
```bash
git checkout main
git merge dev
git push origin main
git tag v2.0
git push origin v2.0
```
🎉 **Version 2 Released!** 🎉

---

## 📦 Using Git LFS for Large Files
### 🚀 Step 1: Install Git LFS
```bash
git lfs install  # (For Windows)
sudo apt install git-lfs && git lfs install  # (For Linux)
```
### 🌿 Step 2: Clone & Create a New Branch
```bash
git clone https://github.com/jas-nurturing-stage/git_assignment_Herovired.git
cd git_assignment_HeroVired
git checkout -b lfs
```
### 🔧 Step 3: Configure & Track Large Files
```bash
git lfs track "*.exe"
git add .gitattributes
git add .
git commit -m "Added large file using Git LFS"
git push origin lfs
```
### 🔍 Step 4: Verify Git LFS
```bash
git lfs ls-files
```
✅ **Verification Complete!** 🎉

---

## 🎯 Expected Output
```bash
The area of the circle with radius 5 = 78.54
The area of the rectangle with length 10 and width 6 = 60
```

🚀 **You're now a Git Pro!** 🏆🎉

