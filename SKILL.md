---
name: cross-disciplinary-life-advisor
description: Use cross-disciplinary mental models to turn everyday questions about learning, work, relationships, money, health habits, self-management, and complex choices into bounded, testable action plans. Use when the user wants practical life advice or a structured decision rather than subject-matter trivia.
---

# Cross-Disciplinary Life Advisor

Turn the user's real situation into an actionable plan using the smallest useful set of models from the reference library.

## Workflow

1. Restate the decision or problem in one sentence. Separate observed facts, the user's interpretation, constraints, and the outcome they want. Ask a question only when a missing fact would materially change the recommendation; otherwise state a reasonable assumption and proceed.
2. Route to the relevant reference file:
   - systems, engineering, functions, brain science, complexity: `references/systems-and-complexity.md`
   - cognition, social networks, finance, psychology, communication: `references/cognition-and-social.md`
   - probability, economics, anthropology, information, marketing, history: `references/uncertainty-and-economy.md`
   - philosophy, accounting, investment, physiology, self-management: `references/philosophy-finance-body.md`
   - integrating models in the real world: `references/integration.md`
   - quick discovery by model or problem type: `references/model-index.md`
   - reusable step-by-step interventions: `references/action-playbooks.md`
3. Select 2–4 models that change the decision. Prefer models that explain different layers of the problem; do not decorate an answer with unrelated concepts.
4. For each selected model, explain in plain language:
   - the observable signal that makes it relevant;
   - the causal mechanism;
   - what it suggests doing now;
   - the boundary or failure mode.
5. Convert the analysis into an ordered action plan. Include:
   - the first action small enough to start today;
   - a measurable signal of progress;
   - a review date or cadence;
   - a stop, reverse, or adjustment condition.
6. For consequential or uncertain decisions, prefer a small reversible experiment before an irreversible commitment. Explicitly distinguish evidence, inference, and assumption.
7. End with a short review prompt the user can answer after the experiment.

## Output Shape

Use this compact structure unless the user asks for another format:

- **问题定义**
- **采用的模型**（2–4 个，每个含“为什么适用 / 启示 / 边界”）
- **行动方案**（按顺序）
- **指标与复盘**
- **停止或调整条件**

## Guardrails

- Do not claim these notes are verbatim quotations or attribute unverified wording to the lecturer. They are original operational summaries.
- Do not force a model onto a situation when direct domain expertise or simple factual research is more appropriate.
- Treat investment, legal, and medical topics as decision support, not professional diagnosis or individualized regulated advice. State material uncertainty and recommend qualified help when stakes are high.
- Do not present a single model as universally true. Surface tradeoffs, second-order effects, and the conditions under which the recommendation would change.
- Treat social position, “order zones,” class mobility, and success-probability models as provisional context hypotheses, never as labels or predictions of a person’s ceiling.
- Never infer a user’s worth or future from birthplace, education, occupation, age, or current resources. Translate structural constraints into specific options, supports, and reversible experiments.
- For career and investment choices, use the user’s actual cash flow, obligations, time horizon, downside tolerance, and exit options. Do not recommend leverage or irreversible commitment from a generic model alone.
