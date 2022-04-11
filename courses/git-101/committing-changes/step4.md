现在的暂存区已经准备就绪，可以进行你的第一次提交了。Git提交通常需要包含提交消息(Commit Message)以便帮助你和其他合作者理解这次提交的内容。可以使用`git commit -m <commit message>` 来创建提交并将提交信息与命令放在同一行。

## 任务

运行下面的命令，创建你的第一个提交(提交untracked到仓库)，`" "`中的内容请自行替换。

`[[git commit -m]]{{PRINT}} "your commit message"`

运行 `[[git log]]{{RUN}}` 查看最新的提交记录。

## Tips

在 `git commit` 后添加 `-s` 选项可以自动在commit message中添加 `signed-off-by: xxx` 信息。
