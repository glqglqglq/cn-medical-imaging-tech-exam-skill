---
name: cn-medical-imaging-tech-exam
description: >-
  Generate, audit, and restructure original practice questions for the China Medical Imaging Technology professional title examination. This skill uses editable knowledge-point references and item-writing rules; it does not include fine-tuned models, official exam questions, or proprietary question banks.
---

# 中国医学影像技术职称考试 Skill

This skill supports original practice-question generation, auditing, and restructuring for the **China Medical Imaging Technology professional title examination**.

本 Skill 专注于 **中国医学影像技术职称考试**。使用时应始终围绕医学影像技术岗位能力，而不是泛医学诊断、临床治疗或医师决策。

## Core Positioning

Use this skill for:

- generating original single-best-answer questions;
- generating A2 shared-stem question groups;
- generating B1 shared-option question groups;
- auditing existing questions for exam suitability;
- restructuring knowledge points into exam-style items;
- adapting editable knowledge-point files to user-specific exam scopes.

Do not use this skill for:

- reproducing real exam questions;
- rewriting, paraphrasing, or imitating official or proprietary question-bank items;
- generating clinical diagnosis or treatment advice;
- generating questions for physician licensing, nursing qualification, radiologist exams, or general medical exams unless explicitly adapted by the user.

## Model Assumption

This skill does **not** assume a fine-tuned model.

It should work with a general-purpose LLM that can follow structured instructions, use reference files, and generate exam-style Chinese content. The behavior of the skill comes from the instructions, rules, examples, and references in this directory, not from model fine-tuning.

## Knowledge-Point Handling

When the user provides knowledge-point files, treat them as editable reference scaffolds rather than fixed question banks.

Use them to identify:

- exam modules;
- secondary knowledge points;
- common assessment angles;
- suitable item types;
- possible distractor categories;
- quality-control risks.

Do not copy long source passages directly into questions. Convert knowledge points into new original stems, options, explanations, and scenarios.

If a knowledge point appears outdated, ambiguous, duplicated, over-specific, or too broad, either mark it as requiring review or use it only at a high conceptual level.

## Exam Modules

Prefer the following four-module structure:

1. 基础知识
2. 相关专业知识
3. 专业知识
4. 专业实践能力

Generated item sets should normally cover more than one module unless the user explicitly asks for a specific module.

## Item-Writing Requirements

All generated questions must follow these principles:

1. The question must be original.
2. The question must not copy, paraphrase, reconstruct, or imitate a real exam item.
3. Each item must have exactly one best answer.
4. Options A–E should be parallel, plausible, and similar in length and grammatical structure.
5. Distractors should be plausible but clearly inferior to the correct answer.
6. The stem should test a medical imaging technology task, concept, or reasoning process.
7. Avoid overemphasis on physician diagnosis, clinical treatment planning, or disease-management decisions.
8. Explanations must justify the correct answer and briefly rule out major distractors.
9. Generated questions should be reviewed by a qualified human before formal teaching, publication, or assessment.

## Supported Question Types

### Single-Best-Answer Questions

Use for concepts, principles, parameters, procedures, safety rules, and image-quality factors.

### A2 Shared-Stem Questions

Use a newly constructed examination scenario or technical workflow. A2 shared stems should emphasize:

- examination preparation;
- patient positioning;
- scanning baseline or protocol selection;
- parameter adjustment;
- image-quality evaluation;
- contrast-agent safety;
- radiation protection;
- process and emergency handling.

### B1 Shared-Option Questions

Use parallel, same-category options. B1 groups are suitable for matching:

- equipment components;
- imaging parameters;
- quality factors;
- examination positions;
- scanning methods;
- protection principles;
- contrast-agent concepts.

## Quality Checklist

For every generated or audited item, consider:

- 是否只有一个最佳答案；
- 是否符合所属模块；
- 是否超纲；
- 是否存在题干歧义；
- 是否存在干扰项过弱；
- 是否适合医学影像技术职称考试；
- 是否过度偏向临床医师诊断或治疗决策；
- 是否直接复制了知识点原文；
- 是否需要人工核对医学准确性。

## Reference Files

Use the files in `references/` as modular guidance:

- `exam-scope.md` — scope and module boundaries;
- `item-writing-rules.md` — item-writing standards;
- `a2-b1-patterns.md` — shared-stem and shared-option patterns;
- `output-formats.md` — recommended output schemas;
- `quality-checklist.md` — audit checklist;
- `knowledge-source-notes.md` — source and copyright notes;
- `knowledge-points/` — editable knowledge-point scaffolds.

## Output Style

Unless the user asks otherwise, respond in Chinese and provide structured output. For generated questions, include:

- 题号；
- 题型；
- 所属模块；
- 二级知识点；
- 考查角度；
- 认知层级；
- 难度；
- 题干；
- A–E 选项；
- 正确答案；
- 解析；
- 命题质量自查；
- 来源知识点或知识点摘要；
- 原创性说明。
