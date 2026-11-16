# Behavioral evaluation

The goal is not to force identical wording. The evaluation checks whether the skill improves the decision process and produces a safe, observable next step.

## Test set

Use the 10 prompts in [`../examples/README.md`](../examples/README.md). Run each prompt once with the skill and, when useful, once without it for comparison.

## Scoring rubric

Score each dimension from 0 to 2:

| Dimension | 0 | 1 | 2 |
|---|---|---|---|
| Problem framing | Mixes facts and assumptions | Partly separates them | Clearly separates facts, interpretations, constraints, and goal |
| Model relevance | Decorative or unrelated models | Some useful relevance | Every selected model changes the decision |
| Actionability | Generic advice | Some concrete actions | Ordered first action, owner/time, and observable result |
| Reversibility | Pushes commitment too early | Mentions testing | Designs a bounded test before irreversible action |
| Measurement | No progress signal | Vague metric | Metric, review cadence, and decision threshold |
| Exit conditions | No stopping logic | General warning | Explicit continue, adjust, reverse, or stop condition |
| Boundaries | Overconfident or unsafe | Partial caveat | Material uncertainty and professional-help boundary are clear |
| Cognitive load | Overlong and unfocused | Mostly usable | Compact enough to act on without losing necessary nuance |

**Recommended release threshold:** no dimension scored 0, and at least 12/16 overall for every case.

## Failure patterns to report

- model-name decoration without a decision consequence;
- asking unnecessary questions instead of proceeding with stated assumptions;
- irreversible advice without testing or downside limits;
- vague actions such as “think carefully” or “communicate more”;
- metrics with no review date or decision threshold;
- medical, legal, or investment certainty beyond the available evidence.
