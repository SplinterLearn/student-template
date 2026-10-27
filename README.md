# My learning repo

Welcome! This is your repo for the **zero-to-builder programme**: your projects, notes, weekly logs and progress all live here. The syllabus is in the [programme repo](https://github.com/splinterlearn/programme); your tutor bot reads it and helps you along.

## Progress

<!-- progress:start -->
_Your tutor bot updates this section when you close a module. Don't edit between these markers._

Block 0: ░░ 0/2 modules
<!-- progress:end -->

## Setup (once)

In the cs50.dev terminal (or your own computer's terminal):

1. **Use your GitHub noreply email**, so your real email never appears in your commits. Find it in GitHub → Settings → Emails (tick "Keep my email addresses private"). It looks like `12345678+username@users.noreply.github.com`.
   ```bash
   git config --global user.name "<your GitHub username>"
   git config --global user.email "<your noreply address>"
   ```
2. **Clone this repo** (copy the URL from the green "Code" button):
   ```bash
   git clone https://github.com/<org>/<this-repo>.git
   cd <this-repo>
   ```
3. **Run the tests** (there are none until your first module starts):
   ```bash
   pip install pytest   # only if `pytest` isn't found
   pytest
   ```
   "no tests ran" is fine at the start.

## The git commands you'll use until Block 3

You don't need to understand these yet; M1.3 explains them and Block 3 teaches git properly.

```bash
git switch main && git pull          # 1. start from the latest main
git switch -c m1.2-hunt               # 2. a new branch for this module (pick the module's name)
git add <files>                       # 3. choose what to save
git commit -m "Say what you did"      # 4. save a snapshot
git push -u origin m1.2-hunt          # 5. send the branch to GitHub
```

Then on github.com, click **"Compare & pull request"**, fill in the template, and open the PR. The tests run automatically (✅ or ❌). The tutor bot reviews it. When both checks are green, merge it.

## How a module works

learn → practise → remix (in this repo) → PR → review → explain-back → merge.

- Each block project lives in its own folder (e.g. `b2-watchlist/`). Each module adds to it.
- Tests in `tests/` folders are provided: **don't edit them**. Earlier modules' tests must keep passing.
- `notes/` is for your own notes; `log/` holds weekly retros (the bot commits them).
- **Never commit passwords, API keys or personal details.** Secrets go in a `.env` file, which is ignored by git.

---

<sub>Generated from the [student template](https://github.com/splinterlearn/student-template), version in [`TEMPLATE_VERSION`](TEMPLATE_VERSION). Template maintainers: bump `TEMPLATE_VERSION` (semver) on every meaningful change. MAJOR = existing repos need a manual change to keep working with the bot; MINOR = new files or features; PATCH = wording and fixes. The bot records the version when it generates a repo.</sub>
