# Git

## Configuration

Git can be configured by the CLI using the `git config` command. For first configuration it is necessary to configure at least the parameters `user.name` and `user.email`. This can be done by the following commands:

git config --global user.name "MyFancyUser"

git config --global user.email "developer@mydomain.com"

## Using Git

### Delete merged branches

```bash
git branch --merged | egrep -v "(^\\*|master|develop)" | xargs git branch -d
```

### Global gitignore

```bash
git config --global core.excludesfile ~/.gitignore
```

### Update password on Mac:

```bash
git config --global credential.helper osxkeychain
```

### Squash commits

[](https://blog.carbonfive.com/2017/08/28/always-squash-and-rebase-your-git-commits/)[https://blog.carbonfive.com/2017/08/28/always-squash-and-rebase-your-git-commits/](https://blog.carbonfive.com/2017/08/28/always-squash-and-rebase-your-git-commits/)

### Copy file from another branch

```bash
git checkout branchB
git checkout branchA -- .
git commit -m 'copy files from branchA to branchB'
```