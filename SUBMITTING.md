# How to submit — with a Pull Request

You've never done this before, and that's fine — every step is here.
A **fork** is your own copy of this repository on GitHub. A **branch**
is where your changes live. A **Pull Request (PR)** asks to bring your
branch's changes into the original repository.

## 1. Install Git

- **Windows:** install [Git for Windows](https://git-scm.com/download/win). Use "Git Bash" (installed alongside it) as your terminal for the rest of these steps.
- **macOS:** open Terminal and run `git --version` — if it's not installed, macOS will prompt you to install it.
- **Linux:** `sudo apt install git` (Debian/Ubuntu) or your distro's package manager.

Confirm it worked:
```
git --version
```

## 2. Create a GitHub account

If you don't have one, sign up at [github.com](https://github.com).

## 3. Configure Git with your name and email

```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## 4. Fork this repository

Go to this repository's GitHub page and click **Fork** (top right).
Use the default settings. This creates
`https://github.com/<your-username>/python-127-homework-1`.

## 5. Clone YOUR fork

Replace `<your-username>` with your actual GitHub username:

```
git clone https://github.com/<your-username>/python-127-homework-1.git
cd python-127-homework-1
```

## 6. Create a branch named after your GitHub username

```
git checkout -b <your-username>
```

## 7. Create your folder and add your files

Inside `submissions/`, create a folder named after your GitHub
username, and put your exercise files there:

```
submissions/<your-username>/exercise_1.py
submissions/<your-username>/exercise_2.py
submissions/<your-username>/exercise_3.py
submissions/<your-username>/exercise_4.py
submissions/<your-username>/exercise_5.py
```

**Only your own folder.** Do not edit `README.md`, `EXERCISES.md`,
`SUBMITTING.md`, or any other student's folder.

## 8. Run every file before committing

```
python submissions/<your-username>/exercise_1.py
```

Compare the output to what `EXERCISES.md` says to expect.

## 9. Commit and push your branch

```
git add .
git commit -m "Add homework 1"
git push -u origin <your-username>
```

## 10. Open the Pull Request

GitHub will show a "Compare & pull request" banner on your fork's page
after pushing — click it. Or open one manually:

- **base repository:** `PythonADI/python-127-homework-1`, branch `main`
- **head repository:** `<your-username>/python-127-homework-1`, branch `<your-username>`

**Title:** `Homework 1 - Your Name` (your real name).

Fill in the checklist in the PR description template.

## 11. Wait for review

You cannot push directly to the original repository — its `main`
branch is protected. Your instructor is automatically requested as a
reviewer. If they ask for changes, push more commits to the **same
branch** — don't open a second PR. The PR updates automatically.
