# medical-imaging-exam

A Codex-ready skill for generating and reviewing original practice questions for the **China Medical Imaging Technology professional title examination**.

## What this skill does

This skill helps an agent create exam-style practice questions focused on Chinese medical imaging technology exams.

It supports:

- Ordinary single-best-answer questions
- A1-style questions
- A2 shared-stem question groups
- B1 shared-option question groups
- Quality auditing and restructuring of generated questions

## What this skill is not

This is not a general medical question generator. It should not be used for physician licensing, nursing exams, clinical treatment planning, or diagnostic radiology board-style interpretation questions.

## Recommended prompt

```text
请使用 medical-imaging-exam skill，基于我提供的参考资料，生成中国医学影像技术职称考试原创练习题。题型为 A2 共用题干，要求覆盖 CT、MRI、X线摄影和辐射防护，所有题目必须原创，并附解析和命题质量自查。
```

## Upload target

Upload or copy this folder as one skill:

```text
medical-imaging-exam/
```
