# Git 102 Assignment

## 📣 Getting Started

1. Create a `.gitignore` file

## 🛠 Requirements

1. Your commits and Pull Request **MUST EXCLUDE** all files containing sensitive data and any misc files/folder.
   i.e: files with sensitive data, misc files or folders: IDE settings, build tools (node_modules), etc.

## 📝 Instructions

1. Update the `.gitignore` file to ignore the appropriate files.
2. Create a remote repository for this project on Github.
3. Push this repository from the command line to Github.
   **NOTE:**: When adding this repository to Github, you will need to replace the word `origin` with `destination`. This is because the remote repository you cloned is already using the name, `origin`.

```
git remote add destination <your_github_repo_url>
git branch -M main
git push -u destination main
```

## ⎋ COMMIT STEPS

1. After making your initial push to your remote repository, create a new branch off your local `main` branch called, `feature/bug-tracking`
2. Create a new file, `.env.production.local`
3. Copy/paste the following sensitive data into, `.env.production.local`:
   `SENTRY_DSN=https://1eb0a2142.ingest.sentry.io/711007`
4. Create a new file, `app.js`
5. Add the following to `app.js`:

```
var loveToCode = true;
var BUG_TRACKING_DNS = process.env.production.local;
```

6. Add the following to `styles.css`:

```
h2 { color: blue; }
```

7. Commit your changes locally. Your commit message should have a subject line and body. It should also follow the 7 commit message conventions.
8. Push this branch to your remote repository. (This will create a new remote branch). Remember, when you push your code to use "destination", not "origin"
9. Create a Pull Request for this branch to be merged into `main`
10. Copy/Paste the Pull Request URL into a `.txt` file and submit that as your assignment. A Devslopes mentor will review your PR (Pull Request), comment as necessary and reject or approve your PR.
