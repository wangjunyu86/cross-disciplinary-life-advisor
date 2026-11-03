# Cross-Disciplinary Life Advisor

一个面向 Codex / AI Agent 的跨学科生活决策 Skill。它会把学习、工作、关系、金钱、健康习惯、自我管理和复杂选择，转化为有边界、可验证、可复盘的行动方案。

## 能做什么

- 区分事实、解释、约束和目标
- 从系统论、认知心理学、概率统计、经济学、金融学、哲学、生理学等领域选择真正相关的模型
- 分析因果机制、机会成本、风险与第二阶影响
- 优先设计低成本、可逆的小实验
- 设置进度指标、复盘节奏以及停止或调整条件

## 适用场景

- 职业选择、转行与换城市
- 学习规划与习惯养成
- 人际关系与沟通
- 消费、储蓄和投资决策支持
- 压力、情绪与健康生活管理
- 多目标冲突和高不确定性选择

## 安装

### Codex

将仓库克隆到 Codex Skills 目录：

```bash
git clone https://github.com/wangjunyu86/cross-disciplinary-life-advisor.git \
  ~/.codex/skills/cross-disciplinary-life-advisor
```

重新启动或刷新 Codex 后即可自动发现该 Skill。

## 使用方式

直接描述现实问题即可，例如：

- “我是否应该换工作？”
- “这个项目已经投入半年，还要不要继续？”
- “帮我设计一个能够坚持的学习计划。”
- “我有三个选择，怎样判断哪个更适合我？”

Skill 默认按照以下结构回答：

1. 问题定义
2. 采用的模型
3. 行动方案
4. 指标与复盘
5. 停止或调整条件

## 文件结构

```text
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── model-index.md
    ├── action-playbooks.md
    ├── systems-and-complexity.md
    ├── cognition-and-social.md
    ├── uncertainty-and-economy.md
    ├── philosophy-finance-body.md
    └── integration.md
```

## 内容说明

仓库内容是面向实际决策的原创操作化整理，不是任何课程、书籍或讲师内容的逐字转载。投资、医疗和法律相关内容仅用于一般决策支持，不能替代持证专业人士的个性化建议。

## 开源许可

本项目采用 [MIT License](LICENSE)，可以免费使用、修改和分发。
