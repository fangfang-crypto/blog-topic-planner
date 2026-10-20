# Blog Topic Planner Skill

一套产品无关的 Blog 选题研究与内容提纲 skill。它从使用者提供的产品资料出发，研究候选主题、检查与现有内容的重复和关键词冲突，排序并输出可交给作者执行的 H1/H2/H3 简报。它不会自动撰写或发布文章。

This product-agnostic skill researches, deduplicates, scores, and briefs blog topics from **your own product information**. It creates writer-ready H1/H2/H3 outlines; it does not draft or publish articles.

## 安装 / Install

将本仓库克隆到 Codex 的 skills 目录，保留目录名 `blog-topic-planner`：

```bash
git clone https://github.com/fangfang-crypto/blog-topic-planner.git ~/.codex/skills/blog-topic-planner
```

重新打开 Codex 会话后，可以在请求中写 `$blog-topic-planner`。也可以把仓库放在其他支持 `SKILL.md` 的 skills 目录。

Clone the repository into a Codex skills directory, then start a new session and invoke `$blog-topic-planner`.

## 使用前必须提供你的产品信息 / Provide your product information first

至少告诉 skill：

- 产品或服务是什么、能做什么、不能做什么；
- 目标读者及其问题或任务；
- 目标国家或地区、语言；
- Blog 要支持的业务目标。

网站、现有 Blog/选题表、竞品、内容分类、发布频率、关键词数据和输出位置也很有帮助。详见 [产品资料清单](references/product-brief.md)。这些信息由使用者在自己的会话中提供；仓库不包含任何预置产品资料。

At minimum, tell the skill what your product does and cannot do, who it serves, the target market and language, and the blog goal. A website alone does not replace your description. Optional inputs include your existing blog and topic history, competitors, categories, publishing capacity, and keyword data.

## 使用示例 / Example request

```text
Use $blog-topic-planner to plan 5 blog topics for my product.
Product: [name and plain-language description]
Capabilities and limits: [verified features and claims to avoid]
Audience: [readers, problems, buying or usage stage]
Market and language: [country/region and language]
Blog goal: [desired reader action or business outcome]
Website and existing content: [links or exports, if available]
Publishing capacity and output: [optional]
```

缺少必要资料时，skill 会先询问；无法读取完整历史时，会将选题标为临时方案，不会声称已完成去重。没有关键词工具时，会标注定性需求信号，不会编造搜索量。

## 输出 / Output

默认在对话中交付候选主题记录、筛选理由、优先级和完整简报。若指定现有表格或其他目的地，skill 会使用该目的地，并在写入后核对记录。每个正式主题包含目标读者、搜索意图、差异化答案、证据来源、可执行的信息增量、H1/H2/H3、内链建议和三项独立质量检查。

The default output is a reviewable topic pack in chat. With an accessible destination you specify, the skill can update an existing tracker and verify the new records.

## 文件 / Files

- [SKILL.md](SKILL.md) — agent workflow and decision rules.
- [Product brief](references/product-brief.md) — information the user supplies for their own product.
- [Topic pack](references/topic-pack.md) — candidate log and writer-brief fields.

The skill has no product-specific configuration, account credentials, CMS integration, or fixed publishing quota.
