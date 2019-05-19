# Git Advanced Guide

## Commit in the past

If the commit is the last commit

e.g. a day ago

```sh
git commit --date='1 day ago' -m "Commit Messages"
```

## Undo Last Commit

### amend

### Reset - Remove last commit

* [Git Questions & Answers - How can I undo the last commit?](https://www.git-tower.com/learn/git/faq/undo-last-commit)
* [Stackoverflow - How do I undo the most recent local commits in Git?](https://stackoverflow.com/questions/927358/how-do-i-undo-the-most-recent-local-commits-in-git)

### Rebase - Override afterward

### Update history

* [How do I make a Git commit in the past?](https://stackoverflow.com/questions/3895453/how-do-i-make-a-git-commit-in-the-past)

## When Pulling the Repository

* [Pull 下載更新](https://gitbook.tw/chapters/github/pull-from-github.html)

Original `git pull` = `git fetch + git merge`

### `git pull --rebase`

* [使用 git rebase 避免無謂的 merge](https://ihower.tw/blog/archives/3843?nsukey=fybPZ5LU0Wg6W4IFJYf8yi0mtnfc%2BkoUSBtuU1AS3WOGER8IiyeXSlRCAu26JUIZAcvNoDU8mYW2Ig%2B1Cg6B3m6wPnJmSoDRGhA1dT8fgiv6QIi2Cr011yJ5la05YYxIJsppaJcuzKhYR9wFp7jk1jdWsOqV45FAwwZzExHkPBRyk%2F296dfSNVuZWWhC%2Bxc6UE6GxZs7C5jg%2B2Opkd5tyQ%3D%3D)
* [潔癖者用Git：pull --rebase 和 merge --no-ff](https://hungyuhei.github.io/2012/08/07/better-git-commit-graph-using-pull---rebase-and-merge---no-ff.html)

Use `git pull --rebase` as default `git pull`. Add the following code in the workspace `.git/config`

```git
[branch "master"]
  remote = origin
  merge = refs/heads/master
  rebase = true
```

Or for global setting

```git
[branch]  
  autosetuprebase = always
```

## Merge Branch

* [合併分支](https://gitbook.tw/chapters/branch/merge-branch.html)
