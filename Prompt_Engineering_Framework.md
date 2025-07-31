# 提示词工程框架指南
# A Guide to Prompt Engineering Frameworks

## 简介 Introduction

提示词工程框架 (Prompt Engineering Frameworks) 是用于构建有效、可靠且一致的提示词 (Prompts) 的结构化方法。它们通过提供一个经过验证的模板，帮助用户明确地向大型语言模型 (LLM) 传达意图，从而显著提升输出结果的质量和可预测性。

Prompt Engineering Frameworks are structured approaches for building effective, reliable, and consistent prompts. They provide proven templates to help users clearly communicate their intent to Large Language Models (LLMs), thereby significantly improving the quality and predictability of the output.

---

## 核心框架 Core Frameworks

以下是一些业界常用且效果显著的提示词框架。
Here are some of the most common and effective prompt frameworks used in the industry.

### 1. CO-STAR 框架

**最适用于 (Best For):** 内容创作、角色扮演、需要明确风格和受众的任务。
Content creation, role-playing, and tasks requiring a specific style and audience.

**结构 (Structure):**
- **C - 上下文 (Context):** 提供背景信息。 (Provide background information.)
- **O - 目标 (Objective):** 你希望模型完成什么具体任务？ (What specific task do you want the model to accomplish?)
- **S - 风格 (Style):** 你希望模型模仿什么样的写作风格？ (What writing style should the model imitate?)
- **T - 语气 (Tone):** 应该采用什么样的情感基调？ (What emotional tone should be adopted?)
- **A - 受众 (Audience):** 这个回答是写给谁看的？ (Who is the intended audience for this response?)
- **R - 回复格式 (Response Format):** 指定输出的格式，如 Markdown、JSON、列表等。 (Specify the output format, e.g., Markdown, JSON, list.)

**示例 (Example):**
- **C:** 我是一家销售环保咖啡豆的初创公司。 (I am a startup selling eco-friendly coffee beans.)
- **O:** 为我们的新产品“雨林联盟”咖啡豆撰写一篇社交媒体推广文案。 (Write a social media post to promote our new "Rainforest Alliance" coffee beans.)
- **S:** 模仿一位充满激情的咖啡博主。 (In the style of a passionate coffee blogger.)
- **T:** 热情、真诚、鼓舞人心。 (Enthusiastic, sincere, and inspiring.)
- **A:** 关心环境和生活品质的年轻消费者。 (Young consumers who care about the environment and quality of life.)
- **R:** 一段 150 字左右的文本，包含 3 个相关的 #标签。 (A text of about 150 words with 3 relevant #hashtags.)

### 2. RISEN 框架

**最适用于 (Best For):** 复杂的问题分解、流程指导、需要详细步骤的任务。
Complex problem decomposition, process guidance, and tasks that require detailed steps.

**结构 (Structure):**
- **R - 角色 (Role):** 指定 AI 扮演的专家角色。 (Specify the expert role for the AI to play.)
- **I - 指令 (Instruction):** 给出需要执行的核心指令。 (Provide the core instruction to be executed.)
- **S - 步骤 (Steps):** 列出完成任务需要遵循的具体步骤。 (Outline the specific steps to follow to complete the task.)
- **E - 期望 (Expectation):** 描述一个高质量输出应该是什么样子。 (Describe what a high-quality output should look like.)
- **N - 窄化 (Narrowing):** 提出约束条件，缩小范围，或要求进行澄清。 (Add constraints, narrow the scope, or ask clarifying questions if needed.)

**示例 (Example):**
- **R:** 你是一位经验丰富的市场分析师。 (You are an experienced market analyst.)
- **I:** 分析当前电动汽车市场的竞争格局。 (Analyze the competitive landscape of the current electric vehicle market.)
- **S:** 1. 识别主要竞争对手。 2. 分析各家的优势和劣势。 3. 总结市场趋势。 (1. Identify major competitors. 2. Analyze the strengths and weaknesses of each. 3. Summarize market trends.)
- **E:** 输出应为一份简洁的报告，包含关键数据点和图表建议。 (The output should be a concise report with key data points and suggestions for charts.)
- **N:** 仅关注北美市场，不要包含混合动力汽车。 (Focus only on the North American market and do not include hybrid vehicles.)

### 3. CLEAR 框架

**最适用于 (Best For):** 结构化研究、信息提取、需要逻辑和精确性的任务。
Structured research, information extraction, and tasks requiring logic and precision.

**结构 (Structure):**
- **C - 上下文与角色 (Context and Role):** 提供背景并设定 AI 的角色。 (Provide background and set the AI's role.)
- **L - 逻辑 (Logic):** 描述解决问题的逻辑或推理过程。 (Describe the logic or reasoning process for solving the problem.)
- **E - 期望 (Expectations):** 明确输出的具体要求和标准。 (Clarify the specific requirements and standards for the output.)
- **A - 行动 (Action):** 明确指示 AI 需要执行的核心任务。 (Clearly state the core task for the AI to perform.)
- **R - 精炼 (Refinement):** 要求 AI 对结果进行审查和优化。 (Ask the AI to review and refine the result.)

**示例 (Example):**
- **C:** 你是一位法律助理，正在为一起专利侵权案件整理资料。 (You are a legal assistant preparing materials for a patent infringement case.)
- **L:** 你需要按时间线梳理所有相关的公开文件和新闻报道。 (You need to sort all relevant public documents and news reports chronologically.)
- **E:** 输出一个 Markdown 格式的表格，包含日期、事件摘要和来源链接。 (Output a Markdown table with columns for date, event summary, and source link.)
- **A:** 开始搜索并整理从 2020 年到 2023 年的相关信息。 (Start searching and compiling relevant information from 2020 to 2023.)
- **R:** 检查时间线的准确性，并高亮显示最重要的三个里程碑事件。 (Verify the accuracy of the timeline and highlight the three most important milestone events.)

### 4. GUIDE 框架

**最适用于 (Best For):** 系统性研究、分步探索、需要持续对话和迭代的任务。
Systematic research, step-by-step exploration, and tasks requiring continuous dialogue and iteration.

**结构 (Structure):**
- **G - 目标 (Goal):** 明确最终希望实现的大目标。 (Clearly state the ultimate high-level goal.)
- **U - 理解 (Understanding):** 确认 AI 对背景和约束的理解。 (Confirm the AI's understanding of the context and constraints.)
- **I - 信息 (Information):** 提供所有必要的信息、数据和示例。 (Provide all necessary information, data, and examples.)
- **D - 方向 (Direction):** 给出完成任务的具体指引和步骤。 (Give specific directions and steps to complete the task.)
- **E - 评估 (Evaluation):** 建立评估输出质量的标准。 (Establish criteria for evaluating the quality of the output.)


## 框架对比总结 Framework Comparison Summary

| 框架 (Framework) | 核心要素 (Key Elements) | 最适用场景 (Best For) |
| :--- | :--- | :--- |
| **CO-STAR** | C-O-S-T-A-R | 内容创作，需要风格和受众定义 (Content creation, needs style/audience) |
| **RISEN** | R-I-S-E-N | 复杂问题分解，流程化任务 (Complex problem-solving, process tasks) |
| **CLEAR** | C-L-E-A-R | 精确的信息提取和结构化研究 (Precise info extraction, structured research) |
| **GUIDE** | G-U-I-D-E | 系统性、迭代式研究和探索 (Systematic, iterative research) |