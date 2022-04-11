openGauss MoocStudio课程通过创建course-content文件来进行组织，采用JSON格式，course-content文件用来定义哪些章节需要被包含在本课程内以及各章节的顺序。


## 克隆示例

使用下面的命令克隆示例代码：
`[[git clone https://github.com/opengauss/playground-course.git playground-course-examples]]{{RUN}}`

在`courses`目录中，创建了我们的示例课程`create-courses-101`，这个课程所对应的course-content定义在：
`playground-course-examples/course/create-courses-101/course-content.json` .

在`course-content`文件中，我们使用JSON格式对课程进行了定义, 例如:

```
{
    "title": "创建openGauss Playground章节与课程",
    "description": "学习如何在openGauss Playground中创建新的章节与课程",
    "logo": "openGauss",
    "chapters": [
    ...
    ]
}
```

定义中的**title**, **description** 和 **logo** 将会在课程欢迎页面进行展示。
定义中的 **chapters** 用于定义课程中的各个章节，具体定义方式在下一节中进行展示。
