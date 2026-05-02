# 中国医学影像技术职称考试 Skill

这是一个面向 **Codex / Agent Skill 上传与使用** 的纯 Skill 包。

本仓库不提供 Python 脚本、不绑定任何模型 API，也不依赖本地运行环境。核心内容是 `medical-imaging-exam/SKILL.md` 以及配套参考规则，用于指导智能体生成、审校和整理 **中国医学影像技术职称考试** 的原创练习题。

## Skill 目录

```text
medical-imaging-exam/
├── SKILL.md
├── README.md
├── references/
│   ├── exam-scope.md
│   ├── item-writing-rules.md
│   ├── a2-b1-patterns.md
│   ├── output-formats.md
│   └── quality-checklist.md
└── examples/
    ├── single-choice-request.md
    ├── a2-b1-request.md
    └── audit-request.md
```

## 使用方式

将 `medical-imaging-exam/` 文件夹上传或复制到支持 Skills 的环境中即可。

推荐上传对象是：

```text
medical-imaging-exam/
```

而不是整个仓库根目录。

## 项目定位

本 Skill 专注于 **中国医学影像技术职称考试**，不是通用医学题库 Skill。

它重点关注医学影像技术岗位能力，包括检查准备、体位摆放、扫描参数、图像质量控制、设备基础、辐射防护、造影剂安全、患者流程和专业实践能力。

## 合规声明

本 Skill 用于生成原创练习题和教学辅助内容，不用于复制、还原、改写、仿写真实考试题，也不代表任何官方考试机构。
