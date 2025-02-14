# Grocery Goose Site

## Overview

Grocery Goose is a site that allows you to learn about the grocery goose app and sign up for the waitlist.


# Local Development

```bash
pip install -r requirements.txt
mkdocs serve
```

## Git Configuration

To ensure proper GitHub attribution, set up your Git configuration:

```bash
# Set your Git username
git config --global user.name "gtshepard"

# Set your Git email to match your GitHub email
git config --global user.email "g.shepardt@gmail.com"
```

Make sure the email matches the one you use for your GitHub account to avoid double attribution in commits.

### Fixing Initial Commit Attribution

If you need to fix the attribution on the initial commit:

```bash
# Create a temporary backup branch
git branch backup

# Start the rebase from the first commit
git rebase -i --root

# In the editor that opens, change 'pick' to 'edit' for the commits you want to fix
# Save and close the editor

# For each commit, run:
git commit --amend --reset-author --no-edit
git rebase --continue

# After fixing all commits, force push the changes
git push origin main --force
```

⚠️ Warning: Only use `git push --force` if you're the only one working on this repository, as it rewrites history.
