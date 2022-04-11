通过远端仓库(Remote Repository)可以将你的修改对外进行分析
或是从远端获取其他开发者所作的修改。通常远端仓库部署在可远程
访问的服务器或是服务中，例如Github和Gitee。可以通过
`git remote`命令来将某个远端仓库和你的仓库进行关联，远端仓库通常使用
SSH链接或HTTPS URL地址，例如：
https://gitee.com/opengauss/community.git 和
git@gitee.com:opengauss/community.git

可以通过为远端仓库指定名称用于在其他命令中引用这些仓库。

远端仓库也可以配置为本机的某个目录，本例就使用这种方式来进行演示。

## 任务

当前环境中有一个位于 `/home/coder/git-101/remote-project/project_1` 的远端仓库，使用
`[[git remote add origin /home/coder/git-101/remote-prpject/project_1]]{{RUN}}`
命令添加这个远端仓库并命名为`origin`。

## Tips

如果你使用`git clone`命令(将在未来的章节中单独介绍)，你所
克隆的仓库将会被自动添加到`origin`。