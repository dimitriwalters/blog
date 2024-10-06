---
title: 'Git Guide for Teams (Integrating Changes)'
date: '2024-10-03'
---

This is a all-you-need-to-know guide for using Git while working in a team. Even for veterans using Git memorizing all the commands is tiring so here's a simple guide.

Besides basic commands like `git add` and `git commit`, the main question is how to integrate your changes into the `main` branch of your repository.

We will first assume your team is using feature branches which leaves you with the problem of integrating other people's changes into your own branch. What you must do is `rebase` the `main` branch, and then incorporate the latest changes into your own by doing so:

```
git checkout main
git pull --rebase
git checkout [feature branch]
git rebase main
```

There will likely be conflicts, this is usually solvable by looking at the code and commits to see what changes were made. One resource that might be helpful is this choose-your-own-adventure guide for common Git problems:

[https://sethrobertson.github.io/GitFixUm/fixup.html](https://sethrobertson.github.io/GitFixUm/fixup.html)

Once your branch looks good, push your branch (`git push`). The last thing that will be done is merging your changes. This should typically be done by another developer, and this command will be `git merge --no-ff [feature branch]`.

After that is complete, your branch is merged and your feature is officially integrated and ready for deployment!