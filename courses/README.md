# Playground Courses
This Folder holds all the courses used by Playground Application

# Courses
Using our example course as an example, the cource resources are organized in follow:
```shell
└── cources
    └── create-course-101         # course name, a course can include a series of scenarios.
        └── course-content.json   # the course-content file describe the content of this course.
        └── create-chapter        # chapter name, a chapter can include a series of steps.
        |   └──index.json         # scenario overall plan, indicating the arrangement of this scenario, this file is in JSON format.
        |   └──intro.md           # introduction information, this will be displayed in the welcome page of this course, this file is in Markdown format.
        |   └──finish.md          # finish information, this will be displayed in the end page of this coursethis file is in Markdown format.
        |   └──step1.md           # detailed instruction for step1, this file is in Markdown format.
        |   └──step2.md           # detailed instruction for step2, this file is in Markdown format.
        └── create-course         # chapter name, a chapter can include a series of steps.
            └──index.json         # scenario overall plan, indicating the arrangement of this scenario, this file is in JSON format.
            └──intro.md           # introduction information, this will be displayed in the welcome page of this course, this file is in Markdown format.
            └──finish.md          # finish information, this will be displayed in the end page of this coursethis file is in Markdown format.
            └──step1.md           # detailed instruction for step1, this file is in Markdown format.
            └──step2.md           # detailed instruction for step2, this file is in Markdown format.
            └──step3.md           # detailed instruction for step3, this file is in Markdown format.
```
