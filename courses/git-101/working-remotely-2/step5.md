如果你在完成了一些修改的提交(committed)后，又想回退这些修改，那么需要使用 `git revert` 命令来完成这个操作。 `git revert` 命令会产生一个新的提交(commit)，这个提交的内容则是指定提交的反作用。

## 任务

使用下面的命令回退最新的一次提交：

```
[[git revert HEAD --no-edit]]{{RUN}}
```

## Tips

如果你的修改还没有推送到远端，那么 `git reset HEAD~1` 同样可以用来回退最后一次提交。
