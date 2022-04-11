可以用 `git diff` 命令查看已暂存和未暂存的修改，以便更详细的了解当前Git目录的差异情况，`git diff` 命令用来查看尚未暂存的文件更新了哪些部分，而`git diff --staged`查看已暂存的将要添加到下次提交里的内容，这条命令将比对已暂存文件与最后一次提交的文件差异。

## 任务

运行 `[[echo 'This is a new line' > untracked]]{{RUN}}` 对该文件进行修改。

运行 `[[echo 'This is a new file' > new_file]]{{RUN}}` 创建一个新的文件并写入内容。

运行 `[[git add new_file]]{{RUN}}` 将新文件添加到暂存区域。

运行 `[[git diff]]{{RUN}}` 及 `[[git diff --staged]]{{RUN}}` 并观察结果



## Tips

`git diff` 本身只显示尚未暂存的改动，而不是自上次提交以来所做的所有改动。 所以有时候你一下子暂存了所有更新过的文件，运行 `git diff` 后却什么也没有，就是这个原因。