如果你想获得一份已经存在了的 Git 仓库的拷贝，比如说，你想为某个开源项目贡献自己的一份力，这时就要用到 `git clone` 命令。 如果你对其它的 VCS 系统（比如说 Subversion）很熟悉，请留心一下你所使用的命令是 `clone` 而不是 `checkout`。 这是 Git 区别于其它版本控制系统的一个重要特性，Git 克隆的是该 Git 仓库服务器上的几乎所有数据，而不是仅仅复制完成你的工作所需要文件。 当你执行 `git clone` 命令的时候，默认配置下远程 Git 仓库中的每一个文件的每一个版本都将被拉取下来。

## 任务

执行 `[[cd /home/coder/git-101/workspace/]]{{RUN}}` 切换到新的目录

执行 `[[git clone /home/coder/git-101/remote-project/project_2]]{{RUN}}` 克隆远端仓库到目录下。

执行 `[[cd project_2]]{{RUN}}` 进入到刚刚克隆的项目中。

## Tips

如果你想在克隆远程仓库的时候，自定义本地仓库的名字，你可以通过额外的参数指定新的目录名：

`git clone https://github.com/libgit2/libgit2 mylibgit`
这会执行与上一条命令相同的操作，但目标目录名变为了 `mylibgit`。