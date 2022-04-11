NOTE: 本章节工作依赖前一章节所作操作，请确保《第三章：远端操作-2》的操作内容已完成(若容器环境已被清理，需要重新完成)。


在进行接下来的操作前，我们首先创建需要创建一个新的分支并切换到这个分支。

可以使用 `git branch "branch name"` 来创建新的分支，使用 `git checkout "branch name"` 来在不同的分支之间进行切换。同时，`git checkout -b "branch name"` 可以直接创建一个新的分支并切换到该分支。

## 任务

执行 `[[cd /home/coder/git-101/workspace/project_2]]{{RUN}}` 进入工作目录。

执行 `[[git branch new_branch">git branch new_branch]]{{RUN}}` 创建一个新的分支 `new_branch`。

执行 `[[git branch]]{{RUN}}` 查看所有分支。

执行 `[[git checkout new_branch]]{{RUN}}` 切换到新创建的分支。