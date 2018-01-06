https://try.github.io/levels/1/challenges/1

Git Quick tips

Git graph for all the branches:
git log --branches --remotes --tags --graph --oneline --decorate
git log --graph --abbrev-commit --decorate --date=relative --all

Remove a submodule from git

mv a/submodule a/submodule_tmp
git submodule deinit -f -- a/submodule
 rm -rf .git/modules/a/submodule 
git rm -f a/submodule 
# Note: a/submodule (no trailing slash)
 # or, if you want to leave it in your working tree
 git rm --cached a/submodule
mv a/submodule_tmp a/submodule




Remove Old mode New Mode changes in git

git config core.filemode false

Working with Submodules
https://medium.com/@porteneuve/mastering-git-submodules-34c65e940407



Next checklist when working with git
Git checklist when working with branches
Git checkout develop
Git pull develop
Git create branch: git checkout -b new-feature-name
Work on the branch and the specific feature.
Git commit and push the changes
Create a PR, once the review is approved merge branch from github


GIT REBASE:

Git rebase re-writes the commit history

git add .
git log
git commit --fixup (commit hash for where this change should go)
git log          (To Check how many commits needs to be fixedup)
git rebase -i head~[number from the top the commit has been changed]
Vim changes
git push -f


Update git submodule to the latest commit
git pull --recurse-submodules
git submodule update --remote --recursive

Update submodule to a specific branch
$git config -f .gitmodules submodule.[path].branch [branchname]
git submodule update --remote [path]   ----> lets to update just the [path] submodule

Push submodule Changes

https://code.tutsplus.com/tutorials/quick-tip-how-to-work-with-github-and-multiple-accounts--net-22574
