# Output Formats / 输出格式

## 单项选择题推荐 JSON 字段

```json
{
  "question_number": 1,
  "question_type": "单项最佳选择题",
  "module": "专业实践能力",
  "secondary_knowledge_point": "CT 扫描基线",
  "assessment_angle": "根据检查部位选择合适扫描基线",
  "cognitive_level": "应用",
  "difficulty": "中等",
  "stem": "题干内容",
  "option_a": "选项A",
  "option_b": "选项B",
  "option_c": "选项C",
  "option_d": "选项D",
  "option_e": "选项E",
  "correct_answer": "A",
  "explanation": "解析内容",
  "source_module": "专业实践能力",
  "source_knowledge_point": "知识点摘要",
  "originality_note": "基于知识点重新构造，未复制原文或真实考试题",
  "quality_check": {
    "only_one_best_answer": "是，理由为……",
    "matches_module": "是，理由为……",
    "out_of_scope": "否，理由为……",
    "stem_ambiguity": "否，理由为……",
    "weak_distractors": "否，理由为……",
    "suitable_for_exam": "是，理由为……",
    "not_over_clinical": "是，主要考查技术岗位能力",
    "not_direct_copy": "是，未直接复制知识点原文",
    "human_review_needed": "建议人工复核医学准确性"
  }
}
```

## A2 共用题干推荐结构

```json
{
  "group_number": 1,
  "question_type": "A2共用题干",
  "shared_stem": "新构造的共用检查场景题干",
  "questions": []
}
```

## B1 共用选项推荐结构

```json
{
  "group_number": 1,
  "question_type": "B1共用选项",
  "shared_options_intro": "本组共用选项主题说明",
  "option_a": "共用选项A",
  "option_b": "共用选项B",
  "option_c": "共用选项C",
  "option_d": "共用选项D",
  "option_e": "共用选项E",
  "questions": []
}
```

## Markdown 输出建议

如果用户不要求 JSON，可使用 Markdown 表格或编号格式，但仍应包含：

- 题号；
- 题型；
- 模块；
- 题干；
- 选项；
- 正确答案；
- 解析；
- 质量自查；
- 来源知识点摘要；
- 原创性说明。
