openEuler MoocStudio课程通过创建course-content文件来进行组织，采用JSON格式，course-content文件用来定义哪些章节需要被包含在本课程内以及各章节的顺序。


## 定义章节


```
{
    ...
    chapters:[
        {
            "chapter_id": "create-chapter",
            "title": "创建openEuler MoocStudio章节",
            "description": "学习如何在openEuler MoocStudio中创建新的章节"
        },
        ...
    ]
}
```

course-content中的**chapters**字段用列表定义本课程中所包和的各个章节，章节在课程页面中出现的顺序与列表属顺序保持一致。
定义中的 **chapter_id** 与课程目录中的章节子目录相对应，如 `playground-course-examples/courses/create-courses-101/create-chapter`。
定义中的**title** 和 **description** 将会在课程欢迎页面进行展示。
