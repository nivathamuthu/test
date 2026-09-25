# Git & GitHub Workflow

This document outlines the standard process for contributing code using Git and GitHub.

## 1. Clone the Repository
```bash
git clone https://github.com/<username>/<repo-name>.git
cd <repo-name>
```

## 2. Create a New Branch
Always create a new branch for each feature or fix — never work directly on `main`.
```bash
git checkout -b feature/<short-description>
```

## 3. Make Changes & Stage Them
```bash
git status
git add .
```

## 4. Commit Your Changes
Write clear, meaningful commit messages.
```bash
git commit -m "Add: short description of the change"
```

## 5. Pull Latest Changes (avoid conflicts)
```bash
git pull origin main
```

## 6. Push Your Branch
```bash
git push origin feature/<short-description>
```

## 7. Create a Pull Request (PR)
- Go to the repository on GitHub.
- Click **Compare & pull request**.
- Add a clear title and description of the changes.
- Request a review from a teammate.

## 8. Code Review & Merge
- Reviewer checks the code, leaves comments if needed.
- Once approved, merge the PR into `main` (usually via **Squash and Merge**).
- Delete the feature branch after merging.

## 9. Sync Local Repo
```bash
git checkout main
git pull origin main
```

## Branch Naming Convention
| Type       | Example                     |
|------------|------------------------------|
| Feature    | `feature/login-api`         |
| Bug fix    | `fix/token-expiry-issue`    |
| Hotfix     | `hotfix/prod-crash`         |
| Docs       | `docs/update-readme`        |

## Commit Message Convention
```
<type>: <short summary>

Types: Add, Fix, Update, Remove, Refactor, Docs
```
