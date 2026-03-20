# Contributing

Thanks for helping improve this list.

This repository is benchmark-first. It does not try to be a general model index, paper list, or simulator catalog.

## Scope

This repository collects publicly accessible benchmarks for VLA and closely related embodied agents, plus directly relevant supporting resources that make those benchmarks usable.

Good additions usually have all of the following:

1. A public benchmark release, leaderboard, challenge page, evaluation codebase, or stable hosting link.
2. A primary reference such as a paper, project page, or official repository.
3. Clear relevance to agent evaluation: manipulation, navigation, driving, GUI control, multimodal reasoning for action, or another embodied decision-making setting.

Do not add:

- Model papers with no benchmark, evaluation suite, or released task definition.
- General CV, NLP, or multimodal benchmarks with no meaningful VLA or embodied-agent relevance.
- Simulators or tooling with no direct benchmark role, released tasks, or evaluation significance.
- Private benchmarks behind institutional or commercial access with no public description or stable reference.

## Contribution Flow

For routine additions or metadata fixes:

1. Find the most specific section in `README.md`.
2. Add or update the row using the repository style rules below.
3. Open a pull request using the repository template.

Open an issue before a pull request if the change involves any of the following:

- renaming or merging sections
- moving many entries across sections
- changing repository-wide formatting conventions
- reclassifying an entry whose placement is ambiguous
- proposing a new top-level section

## Placement

Place each entry in the most specific section that matches its primary evaluation use.

Examples:

- Manipulation suites go under the embodied robotics sections, not general resources.
- Driving evaluation suites go under autonomous driving, even if they include perception-only subtasks.
- GUI or operating-system task suites go under GUI and computer-use agents.
- Simulators, model hubs, and leaderboards belong under infrastructure and resources when they primarily support benchmark execution or comparison.

If an entry could fit multiple sections, choose one primary location and mention the overlap in the description only if it materially helps readers.

## Row Format

Use the existing table format:

```text
| [Benchmark Name](project-url) | [Venue 2025] One-sentence description: what agent setting, what tasks, what scale, and what makes the benchmark practically useful. | [arXiv](arxiv-url) · [GitHub](github-url) · [website](project-url) |
```

Write concise descriptions. Prefer concrete facts over marketing language.

Use this default information order in `Highlights`:

1. primary agent setting or task family
2. scale such as tasks, scenarios, questions, hours, or environments
3. major modalities or evaluation dimensions
4. why the benchmark is practically useful, if that is still not obvious

Include, when known:

- agent domain or embodiment
- task family
- scale such as tasks, scenes, scenarios, hours, or questions
- major modalities such as RGB, video, language, actions, depth, proprioception, or tactile signals

## Style Rules

Keep naming and formatting consistent with the rest of the repository.

- Use the official benchmark or project name when possible.
- Prefer canonical venue names such as `RA-L`, `RSS`, `CoRL`, `ICRA`, `IROS`, `NeurIPS`, `ICLR`, `CVPR`, `ICCV`, and `ECCV`.
- Prefer `GitHub` and `website` as the default reference labels for repository and project-page links.
- Use `Hugging Face` in prose and use `HF` only when an existing table row already uses that shorthand or brevity materially helps readability.
- Prefer canonical project pages over mirrors when both are available.
- Keep section descriptions to a single short scope sentence when editing repository structure.
- Write `Highlights` as one sentence unless a second sentence is necessary to avoid ambiguity.
- Prefer factual wording over evaluative claims such as `state-of-the-art`, `powerful`, or `highly impactful`.

For entries under resource-oriented sections such as simulation platforms, model hubs, or evaluation platforms:

- describe the supporting role of the resource, not as if it were a benchmark itself
- make it clear whether the item provides benchmark code, released tasks, data access, model artifacts, or leaderboard results
- avoid dataset-style wording for resources whose main purpose is hosting, execution, or comparison

## Sorting Rules

Keep every markdown table sorted using these rules:

1. Sort by year in descending order.
2. For entries in the same year, sort by venue strength with formal publications before weaker or informal releases.
3. For entries in the same year and similar venue level, preserve the existing relative order unless there is a clear reason to change it.

Use this practical venue priority as the default tie-breaker:

- Journal and top-tier archival venues first, such as `IJRR`, `TPAMI`, `IJCV`
- Major conference venues next, such as `NeurIPS`, `ICLR`, `CVPR`, `ICCV`, `ECCV`
- Robotics venues after that, such as `RSS`, `CoRL`, `ICRA`, `IROS`, `RA-L`
- Informal or non-archival releases last, such as `arXiv`, `GitHub`, `website`

This rule is intentionally pragmatic rather than perfectly exhaustive. Favor consistency over overfitting edge cases.

## Verification Checklist

Before opening a pull request, check that:

1. Links resolve to the official source or a stable mirror.
2. The venue and year label is accurate and consistent with the rest of the list.
3. The entry is placed in the correct section.
4. The table remains correctly sorted after your change.
5. The markdown renders cleanly.

If you are unsure whether an entry belongs, open an issue first.

## Maintainer Review Checklist

Maintainers should review each contribution against the following criteria:

1. The proposed item is actually a benchmark or a directly relevant supporting resource.
2. The item is not primarily a model-only paper, generic dataset, or tool with no benchmark role.
3. The chosen section is the most specific valid location.
4. Naming, venue style, and reference labels match repository conventions.
5. The `Highlights` sentence is concrete, concise, and free of marketing language.
6. Large taxonomy changes were discussed in an issue first.

If a contribution is directionally useful but misplaced, prefer asking for reclassification or wording changes rather than rejecting it outright.
