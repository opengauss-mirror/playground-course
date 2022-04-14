openGauss MoocStudio课程还可以引用其他现有openGauss MoocStudio中的章节，以促进基础知识内容的重复利用。

可以通过使用下面的定义方式进行章节重用:

```
{
    ...
    chapters:[
        {
            "course_id": "reuseable-course",
            "chapter_id": "test_chapter",
            "title": "测试章节",
            "description": "测试章节"
        },
        ...
    ]
}
```

这样就可以从`reusable-course`中引用`test-chapter`章节，如果该章节没有被包含在任何章节中，请将`course_id`留空。
