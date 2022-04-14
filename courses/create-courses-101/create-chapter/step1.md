一个openGauss MoocStudio章节中所包含的内容通过一系列的Markdown文件、Bash脚本以及JSON文件进行描述和组织。

## Task

使用`git clone`将我们的示例目录进行克隆：

`[[git clone https://github.com/opensourceways/playground-courses.git playground-course-examples]]{{RUN}}`

在课程目录中，你将看到一系列openGauss Playground课程的相应示例，您现在正在阅读的示例就位于其中，使用下面的命令查看它是如何组织的：

`[[ls -lha playground-course-examples/courses/create-courses-101/create-chapter]]{{RUN}}`

目录名将与章节URL对应。

您现在正在阅读的步骤位于：

`playground-course-examples/courses/create-courses-101/create-chapter/step1.md`

本章节内所有的步骤(step)都通过一个名为index.json的JSON文件来进行组织：

`playground-course-examples/courses/create-courses-101/create-chapter/index.json`

index.json文件定义了章节的名称、简介、步骤顺序、UI风格以及运行环境。
