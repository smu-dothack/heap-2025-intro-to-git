# Introduction to Git

This hands-on lab is designed to assess your understanding of the fundamental Git concepts of branching, committing, and merging. You are free to complete this lab using any environment.

## Instructions

To successfully complete this lab, please follow these steps:

1. Create a new branch: Create a branch with your name (e.g., git checkout -b your-name).

2. Make changes and commit: Make a change to any file in this repository (or create a new one).  Commit your changes to your branch.

3. Merge your branch: Merge your branch into the main branch.

4. Push your changes: Push your branch to the remote repository.
	- Example: `git push -u origin your-name`.
	- If you merge locally instead of via a PR, push `main` after merging (see examples below).
5. Submit a Pull Request: Submit a Pull Request to merge your branch into the main branch.

### Notes

- Preferred workflow: create a Pull Request on GitHub and merge there — this ensures the merge is recorded and the repository's checks run on the merged history.
- If you merge locally, prefer creating a merge commit so the action can detect the merge (for example, `git merge --no-ff your-name`).

### Example commands

```bash
# create a branch
git checkout -b your-name

# make changes, then commit
git add .
git commit -m "Add: short description of change"

# push branch and set upstream
git push -u origin your-name

# Option A: create a PR on GitHub and merge via the web UI

# Option B: merge locally and push main
git checkout main
git merge --no-ff your-name
git push origin main
```

## Evaluation

Your submission will be evaluated automatically by a GitHub Action. The action will check the commit history to verify that you have:

- Created a branch (other than the initial default branch of **main**)

- Made at least one commit

- Performed a merge

**Reminder**: Ensure that your commit messages are clear and descriptive.

If the GitHub Action passes, you have successfully completed the assignment :D