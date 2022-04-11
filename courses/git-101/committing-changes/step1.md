安装完 Git 之后，要做的第一件事就是设置你的用户名和邮件地址。 这一点很重要，因为每一个 Git 提交都会使用这些信息，它们会写入到你的每一次提交中。

## 任务

通过下面的命令来配置Git, `" "`中的内容根据实际情况进行替换。

`[[git config --global user.name]]{{PRINT}} "your name"`

`[[git config --global user.email]]{{PRINT}} "your email"`

## Tips

如果使用了`--global`选项，那么该命令只需要运行一次，因为之后无论你在该系统上做任何事情， Git 都会使用那些信息。 当你想针对特定项目使用不同的用户名称与邮件地址时，可以在那个项目目录下运行没有`--global`选项的命令来配置。

使用`git config -l`可以查看当前环境中的Git配置情况。