---
name: medical-imaging-exam
description: >-
  Generate, audit, and restructure original practice questions for the China Medical Imaging Technology professional title examination. Use this skill for Chinese medical imaging technology exam preparation, including single-best-answer questions, A2 shared-stem questions, and B1 shared-option questions. This skill focuses on medical imaging technology roles rather than general medicine, physician diagnosis, nursing, or clinical treatment exams.
---

# Medical Imaging Technology Professional Title Exam Skill

## Purpose

This skill is dedicated to the **China Medical Imaging Technology professional title examination**.

Use it to generate, audit, transform, or structure original practice questions for medical imaging technology exam preparation. The focus is not general medicine. The focus is the professional knowledge and workplace competence expected of medical imaging technologists in China.

The skill should emphasize:

- X-ray radiography technology
- CT examination technology
- MRI examination technology
- DSA and interventional imaging technology basics
- Ultrasound and nuclear medicine fundamentals when relevant to the exam scope
- Imaging anatomy and imaging physics basics
- Image quality control
- Imaging equipment fundamentals
- Radiation protection
- Contrast media safety
- Patient preparation and examination workflow
- Professional practice ability of medical imaging technologists

## When to Use This Skill

Use this skill when the user asks to:

- Generate original practice questions for 中国医学影像技术职称考试
- Create A1, A2, or B1 style questions for medical imaging technology
- Convert reference materials into exam-style practice items
- Audit generated questions for quality, scope, ambiguity, or exam fit
- Produce structured JSON, Markdown, Word-ready, or table-ready question content
- Design shared-stem or shared-option question groups for this exam

Do not use this skill for:

- General medical licensing exams
- Clinical physician diagnosis or treatment decision exams
- Nursing qualification exams
- Radiologist board-style diagnostic interpretation exams
- Copying, restoring, paraphrasing, or imitating real exam questions
- Claiming generated content is official exam material

## Core Principles

Generated questions must be original. They must not copy, paraphrase, restructure, or closely imitate real exam questions, official question banks, or proprietary materials.

Each question should be exam-oriented but not clinically overextended. For medical scenario questions, the task should reflect a medical imaging technologist's role, such as patient preparation, parameter selection, positioning, image quality analysis, equipment operation, safety management, or workflow handling.

Avoid overemphasizing physician-only decisions, final clinical diagnosis, clinical treatment plans, drug treatment selection, surgical management, or disease prognosis.

## Supported Item Types

### Single-best-answer questions

Use for A1 or ordinary single-choice questions. Each item has one stem, five options, one best answer, explanation, metadata, and quality check.

### A2 shared-stem questions

Use for case-based or examination-scenario-based question groups. Each group has one shared stem and multiple subquestions. Each subquestion has its own A-E options and one best answer.

### B1 shared-option questions

Use for matching-style groups. Each group has one set of shared A-E options and multiple subquestions. Each subquestion selects one best answer from the shared options.

## Required Quality Standards

For every generated item, check:

1. Only one best answer exists.
2. The item matches the intended module.
3. The item is within the China Medical Imaging Technology professional title exam scope.
4. The stem is not ambiguous.
5. Distractors are plausible and not obviously weak.
6. The item is suitable for medical imaging technology exam preparation.

Use the detailed checklist in `references/quality-checklist.md`.

## Exam Scope Guidance

Use `references/exam-scope.md` for the subject boundary.

The four broad modules are:

1. 基础知识
2. 相关专业知识
3. 专业知识
4. 专业实践能力

Try to distribute questions across these modules unless the user requests a specific topic.

## Item Writing Rules

Use `references/item-writing-rules.md` for general writing rules.

Important rules:

- Use clear Chinese exam-style wording.
- Keep A-E options grammatically parallel.
- Avoid giving away the answer through option length, specificity, or wording.
- Avoid “all of the above” and “none of the above” unless explicitly requested.
- Do not create unsafe clinical advice.
- Explain both the correct answer and key distractors.

## A2 and B1 Rules

Use `references/a2-b1-patterns.md` when generating shared-stem or shared-option groups.

A2 questions should be anchored in a realistic imaging technology scenario.

B1 options should be same-category, parallel, and confusable, such as imaging positions, imaging sequences, scan parameters, artifacts, safety actions, or quality control concepts.

## Output Formats

Use `references/output-formats.md` for JSON and Markdown-ready formats.

When the user does not specify a format, produce a readable Markdown format.

When the user asks for machine-readable output, use strict JSON.

## Safety and Copyright Boundary

This skill must not reproduce copyrighted question banks or official exam questions. If the user provides real exam questions and asks to rewrite them, do not generate close variants. Instead, extract high-level knowledge points and create new original questions with different scenarios, structures, wording, and options.

Generated content is for study and teaching support only. It is not official exam material.
