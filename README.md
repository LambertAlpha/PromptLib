# 🧠 PromptLib - 个人提示词知识库

这是一个结构化的prompt提示词知识库，帮助你组织和管理各种AI对话的提示词模板。

## 📁 目录结构

```
PromptLib/
├── 📁 10_research_and_summary/      # 学术研究和信息总结
│   ├── summarize-whitepaper-ELI5.yaml           # ELI5风格总结
│   ├── summarize-whitepaper-technical.v2.yaml   # 技术性总结
│   └── extract-key-methodologies.yaml           # 提取核心方法论
│
├── 📁 20_strategic_thinking/        # 策略思考和头脑风暴  
│   ├── brainstorm-swot-analysis.yaml           # SWOT分析
│   ├── red-team-my-idea.yaml                   # 红队演练
│   └── compare-strategies-pro-con.yaml         # 策略对比
│
├── 📁 30_coding_assistant/          # 编码辅助
│   ├── refactor-python-code.yaml               # Python代码重构
│   └── explain-code-snippet.yaml               # 代码解释
│
├── 📁 99_archive/                   # 归档区
│   └── old-prompt.yaml                         # 旧提示词示例
│
└── 📁 _snippets/                    # 可重用片段
    ├── persona-expert-researcher.txt           # 专家研究员人设
    └── format-markdown-table.txt               # Markdown格式化指令
```

## 🚀 使用方法

### 1. YAML文件结构
每个提示词文件都包含以下部分：
- `description`: 功能描述 
- `usage_notes`: 使用说明和最佳实践
- `model_parameters`: 推荐的模型参数设置
- `prompt_template`: 提示词模板（支持变量替换）

### 2. 变量替换
在提示词模板中使用 `{{variable_name}}` 语法：
- `{{paper_text}}` - 论文文本
- `{{persona-expert-researcher}}` - 引用_snippets中的专家人设
- `{{format-markdown-table}}` - 引用格式化指令

### 3. 片段复用
`_snippets/` 文件夹包含可重用的文本片段：
- **persona-expert-researcher.txt**: 专业研究员角色设定
- **format-markdown-table.txt**: 标准Markdown格式要求

## 📋 最佳实践

1. **版本管理**: 重要提示词修改时使用版本号（如 v2, v3）
2. **参数记录**: 记录效果最好的模型参数组合
3. **实际测试**: 新提示词要在实际场景中测试效果
4. **定期整理**: 将过时的提示词移到 `99_archive/`
5. **个性化调整**: 根据个人使用习惯调整temperature等参数

## 🔧 扩展建议

随着使用经验的积累，可以考虑添加：
- `40_content_creation/` - 内容创作相关提示词
- `50_data_analysis/` - 数据分析提示词  
- `60_learning_assistant/` - 学习辅助提示词
- 更多领域特定的专家persona片段

## 💡 使用技巧

1. **组合使用**: 可以组合多个片段创建复杂提示词
2. **A/B测试**: 对同一任务创建多个版本比较效果
3. **上下文长度**: 注意控制提示词长度，避免超出模型限制
4. **持续优化**: 根据使用反馈不断优化提示词效果

---
*最后更新: 2025年7月*