# lab2-vc
repo to do tasks of lab2 "Git Version Control " course

Q:  how to remove the branches locally and
           remotely?

A:  To delete a local branch we use (git branch -d branch-name)
     
    To delete a remote branch we use ( git push origin --delete branch-name)

# Git Tagging and Rebase Guide

## Annotated Tags vs Lightweight Tags
- **Annotated Tags**:
  - Store additional metadata (e.g., author, date, message).
  - Created with: `git tag -a <tagname> -m "<message>"`.
  - Recommended for releases or important milestones.

- **Lightweight Tags**:
  - Act as a simple pointer to a commit.
  - Created with: `git tag <tagname>`.
  - Ideal for temporary tags or quick references.

## When to Use Rebase
- Use `git rebase` to:
  1. Clean up commit history by combining multiple commits into one.
  2. Move changes from one branch to another to keep a linear history.
- Avoid rebasing shared branches as it rewrites commit history.

## How to List Tags
To list all tags in a repository:
```bash
git tag


 ## to Delete a Tag
 -Locally
 -git tag -d <tagname>

-Remotely
-git push origin --delete <tagname>


![Git Workflow](download.jpeg)
