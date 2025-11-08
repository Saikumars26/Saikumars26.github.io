# CI/CD Pipeline Report

## Student Information
- **Name:** Sai Kumar Sheri
- **Date:** November 8, 2025
- **Repository:** https://github.com/Saikumars26/Saikumars26.github.io
- **Live URL:** https://Saikumars26.github.io

## Deployment History
Check the Actions tab for complete deployment history.

### Iteration Summary

1. **Initial Deployment**
   - **Commit:**  ff97b9d
   - **Time to Deploy:** ~38 seconds
   - **Status:** ✅ Success
   - **Notes:** Added initial website files (`index.html`, `about.html`, `projects.html`, `style.css`).

2. **Iteration 1: Trello Link in README**
   - **Commit:**   fde593c
   - **Changes Made:** Added project-tracking section with Trello board link to `README.md`.
   - **Deployment Time:** ~36 seconds
   - **Status:** ✅ Success

3. **Iteration 2: Deploy Info + Personalization**
   - **Commits:** 
     -  d0d566a — Personal content updates (name/university where applicable)
     -  c0470ee — Added `deploy-info.json` and updated Projects with CI/CD card
   - **Changes Made:** Replaced placeholders with real info; added `deploy-info.json` and the “CI/CD Pipeline Status” card.
   - **Deployment Time:** ~ 1  minutes
   - **Status:** ✅ Success

4. **Iteration 3: Feature Branch**
   - **PR Number:** #1
   - **Branch:** `feature/add-contact`
   - **Commits on feature branch:** 
     -  5e542bc — Add `contact.html`
     -  5de7391 — Add “Contact” link to all pages
   - **Deployment triggered by:** Pull Request merge into `main`
   - **Deployment Time:** ~1 minutes
   - **Status:** ✅ Success

## CI/CD Understanding

### What is CI/CD?
CI/CD - Continuous Integration/Continuous Deployment-- automates integrating code changes and deploying them to production. Each push to the `main` branch triggers a repeatable build and deployment, reducing manual work and preventing errors.

### Benefits Observed
1. **Automatic deployment** on every push to `main`.
2. **Clear visibility** via the Actions tab (green checks, logs, failures).
3. **Safe collaboration** using branches and Pull Requests before merging to `main`.

### Challenges Faced
- **Authentication Issue:** When trying to push commits to GitHub, I was prompted for a password but GitHub no longer supports password authentication for HTTPS pushes.  
  **Fix:** I created a **Personal Access Token (PAT)** on GitHub and used it in place of my password. After that, `git push` worked successfully.

- **Network Error:** Encountered “Could not resolve host: github.com” — fixed by retrying after checking Wi-Fi  connection.

### Real-World Application
On larger teams, CI/CD ensures consistent, automated releases. Developers work on feature branches, open PRs for review, and merges trigger automated builds/tests/deployments. This shortens feedback cycles, maintains quality, supports quick rollbacks using commit history, and enables multiple contributors to deploy safely and reliably.

