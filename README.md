# Git Alias Cheat Sheet - nicolaslopez82
---
`g` – `git` :octocat:

`gst` – `git status` :octocat:

`gpl` – `git pull` :octocat:

`gplr` – `git pull --rebase` :eight_pointed_black_star:

`gp` – `git push` :octocat:

`gd` – `git diff` :octocat:

`gdc` – `git diff --cached` :eight_pointed_black_star:

`gdv` – `git diff -w "$@" | view -` :octocat:

`gc` – `git commit -m` :octocat:

`gamend` - `git commit --amend --no-edit` :eight_pointed_black_star: > Adds all the staged changes to the last commit without change its message.

`gco` – `git checkout` :octocat:

`gcm` – `git checkout master` :octocat:

`gr` – `git remote` :eight_pointed_black_star:

`grv` – `git remote -v` :octocat:

`grbi` – `git rebase -i` :eight_pointed_black_star:

`grbc` – `git rebase --continue` :eight_pointed_black_star:

`grba` – `git rebase --abort` :eight_pointed_black_star:

`gb` – `git branch` :octocat:

`gba` – `git branch -a` :octocat:

`gcl` – `git config --list` :eight_pointed_black_star:

`gcp` – `git cherry-pick`  :eight_pointed_black_star: > It will bring all commit changes but also stage them.

`gss` – `git status -s` :eight_pointed_black_star:

`ga` – `git add .` :octocat:

`gm` – `git merge` :octocat:

`grh` – `git reset HEAD` :octocat:

`grhh` – `git reset HEAD --hard` :eight_pointed_black_star:

`gclean` – `git reset --hard && git clean -dfx` :eight_pointed_black_star:

`gwc` – `git whatchanged -p --abbrev-commit --pretty=medium` :eight_pointed_black_star:

`gsts` – `git stash show --text` :octocat:

`gsta` – `git stash` :octocat:

`gstp` – `git stash pop` :octocat:

`gstd` – `git stash drop` :eight_pointed_black_star:

`ggpull` – `git pull origin $(current_branch)` :eight_pointed_black_star:

`ggpur` – `git pull --rebase origin $(current_branch)` :eight_pointed_black_star:

`ggpush` – `git push origin $(current_branch)` :eight_pointed_black_star:

`ggpnp` – `git pull origin $(current_branch) && git push origin $(current_branch)` :eight_pointed_black_star:

`glog` – `git log --oneline --decorate --color --graph` :octocat:

`glogline` -  `git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit` :octocat:


---

## 3 levels of configuration of `git config`:
- `git config --system` > Related to machine configuration. Any change here will affect all the users and projects that exists on the environment.
- `git config --global` > Related to single user configuration. Any change here will affect all projects under your user.
- `git config --local` > Related to single project configuration. Any change here will affect the current project only, can only be used inside a git repository.

For git alias purpose, I used only the global one.

---

## Enables how to work with our favourite code editor. I choose Atom.

:black_small_square: `git config --global core.editor "atom --wait"`

 :black_small_square:`git config --global alias.dv 'difftool -t atom -y'`


---

![git-flow](https://github.com/nicolaslopez82/git-alias-cheat-sheet/blob/master/git-flow.png)

---
:small_red_triangle_down: [Download -> atlassian-git-cheatsheet.pdf](https://github.com/nicolaslopez82/git-alias-cheat-sheet/blob/master/atlassian-git-cheatsheet.pdf) :pirate_flag:

---
:small_red_triangle_down: [Git-Tutorial.pdf](https://github.com/nicolaslopez82/git-alias-cheat-sheet/blob/master/Git-Tutorial.pdf) :octocat:
