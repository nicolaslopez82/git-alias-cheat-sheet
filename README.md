# Git Alias Cheat Sheet - nicolaslopez82

`g` – `git`

`gst` – `git status`

`gpl` – `git pull`

`gplr` – `git pull --rebase`

`gp` – `git push`

`gd` – `git diff`

`gdc` – `git diff --cached`

`gdv` – `git diff -w "$@" | view -`

`gc` – `git commit -m`

`gamend` - `git commit --amend --no-edit` > Adds all the staged changes to the last commit without change its message.

`gco` – `git checkout`

`gcm` – `git checkout master`

`gr` – `git remote`

`grv` – `git remote -v`

`grbi` – `git rebase -i`

`grbc` – `git rebase --continue`

`grba` – `git rebase --abort`

`gb` – `git branch`

`gba` – `git branch -a`

`gcl` – `git config --list`

`gcp` – `git cherry-pick` > It will bring all commit changes but also stage them.

`gss` – `git status -s`

`ga` – `git add .`

`gm` – `git merge`

`grh` – `git reset HEAD`

`grhh` – `git reset HEAD --hard`

`gclean` – `git reset --hard && git clean -dfx`

`gwc` – `git whatchanged -p --abbrev-commit --pretty=medium`

`gsts` – `git stash show --text`

`gsta` – `git stash`

`gstp` – `git stash pop`

`gstd` – `git stash drop`

`ggpull` – `git pull origin $(current_branch)`

`ggpur` – `git pull --rebase origin $(current_branch)`

`ggpush` – `git push origin $(current_branch)`

`ggpnp` – `git pull origin $(current_branch) && git push origin $(current_branch)`

`glog` – `git log --oneline --decorate --color --graph`

`glogline` -  `git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit`


---

## 3 levels of configuration of `git config`:
- `git config --system` > Related to machine configuration. Any change here will affect all the users and projects that exists on the environment.
- `git config --global` > Related to single user configuration. Any change here will affect all projects under your user.
- `git config --local` > Related to single project configuration. Any change here will affect the current project only, can only be used inside a git repository.

For git alias purpose, I used only the global one.

---

## Enables how to work with our favourite code editor. I choose Atom.

`git config --global core.editor "atom --wait"`

`git config --global alias.dv 'difftool -t atom -y'`
