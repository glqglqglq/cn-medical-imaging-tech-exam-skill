# Output Formats

## Default Markdown format

Use this format when the user does not request JSON.

```markdown
## 第 1 题

题型：A1
所属模块：基础知识
二级知识点：...
考查角度：...
认知层级：理解
难度：中等

题干：...

A. ...
B. ...
C. ...
D. ...
E. ...

正确答案：A

解析：...

命题质量自查：
1. 是否只有一个最佳答案：是，...
2. 是否符合所属模块：是，...
3. 是否超纲：否，...
4. 是否存在题干歧义：否，...
5. 是否存在干扰项过弱：否，...
6. 是否适合医学影像技术职称考试：是，...
```

## Single-choice JSON fields

Use these fields for ordinary single-best-answer items:

- question_number
- question_type
- module
- secondary_knowledge_point
- assessment_angle
- cognitive_level
- difficulty
- stem
- option_a
- option_b
- option_c
- option_d
- option_e
- correct_answer
- explanation
- quality_check

## A2/B1 JSON fields

For A2 groups:

- group_number
- question_type
- shared_stem
- questions

For B1 groups:

- group_number
- question_type
- shared_options_intro
- option_a
- option_b
- option_c
- option_d
- option_e
- questions

Each subquestion should include:

- group_number
- item_number
- question_number
- question_type
- module
- secondary_knowledge_point
- assessment_angle
- cognitive_level
- difficulty
- shared_stem
- stem
- option_a to option_e
- correct_answer
- explanation
- quality_check
