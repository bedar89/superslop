# Contributing

Superslop has one job: turn recognizable AI writing habits into a deliberate parody.
Changes should improve that parody without losing the original message.

## Make a change

Edit [SKILL.md](SKILL.md). Keep the numbered pattern catalog readable on its own.
Examples should demonstrate a writing habit, not merely add length.

Include a short before-and-after example with your proposal. Explain what the
current skill gets wrong and how your change improves the result. Avoid adding
a universal rule to fix one model's single awkward sentence.

## Check the behavior

Use a fresh agent conversation for each case in [evals/cases.json](evals/cases.json).
Provide the current skill and the case's prompt. Do not supply a desired answer.
These cases require an actual model response; reading the examples in the skill
does not count as running them.

Assess the response against that case's criteria. For a skill change, compare the
previous and proposed versions on the same model and settings. Record the model,
date, prompts, outputs, and any failures in your review. Differences between
models are expected. One successful run is not a compatibility guarantee.

A good result preserves the facts, sounds like familiar assistant prose, and
makes the excess itself funny. A longer answer is not automatically a better
parody. Exact wording and keyword counts are poor quality measures.

For purely visual or documentation changes, inspect the affected rendering and
check local links. Model evaluations are unnecessary unless the skill changes.

## Keep it portable

The skill is a Markdown file. It must not depend on the author's machine,
personal settings, another installed skill, a paid service, or a particular model.
Keep examples fictional and free of personal information.

Retain the upstream notice in [LICENSE](LICENSE) and credit in [NOTICE.md](NOTICE.md).
Contributions are provided under the same MIT license.
