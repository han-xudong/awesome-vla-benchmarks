# Contributing to Awesome VLA Benchmarks

Thank you for your interest in contributing! This list aims to be the most comprehensive and up-to-date collection of benchmarks for evaluating **Vision-Language-Action (VLA)** models.

## Table of Contents

- [What to Contribute](#what-to-contribute)
- [How to Contribute](#how-to-contribute)
- [Entry Format](#entry-format)
- [Quality Guidelines](#quality-guidelines)
- [Pull Request Checklist](#pull-request-checklist)
- [Code of Conduct](#code-of-conduct)

---

## What to Contribute

We welcome additions of:

- **Benchmarks** for evaluating VLA models in any of the covered domains (robotics, driving, GUI agents, game environments, multimodal perception, etc.)
- **Datasets** used for training or evaluating VLA models
- **Simulation environments or platforms** relevant to VLA research
- **Leaderboards or evaluation services** for VLA tasks

We are **not** looking for:

- General-purpose LLM or vision-only benchmarks with no actionable or embodied component
- Duplicates of existing entries
- Benchmarks that are not publicly accessible or described in a paper/report

---

## How to Contribute

1. **Fork** this repository.
2. **Create a branch** from `main` with a descriptive name, e.g. `add-<benchmark-name>`.
3. **Edit `README.md`** to add your entry in the appropriate section table, following the [Entry Format](#entry-format) below.
4. **Submit a pull request** against the `main` branch.

A GitHub Actions workflow will automatically check your PR for formatting issues. Please address any failures before requesting a review.

---

## Entry Format

Each entry must be a row in the relevant Markdown table. The table has three columns:

```markdown
| Name | Highlights | References |
|------|-----------|------------|
| [Benchmark Name](https://official-website.com/) | [Venue Year] One-sentence description of what makes this benchmark notable | [arXiv](https://arxiv.org/abs/XXXX.XXXXX) · [GitHub](https://github.com/org/repo) · [Website](https://official-website.com/) |
```

### Column rules

| Column | Required | Description |
|--------|----------|-------------|
| **Name** | ✅ | A Markdown link `[Name](URL)` pointing to the benchmark's official website or primary resource |
| **Highlights** | ✅ | `[Venue Year]` tag (if published) followed by a single concise sentence describing what distinguishes this benchmark |
| **References** | ✅ | At least one reference link (arXiv, GitHub, or Website). Multiple links separated by ` · ` |

### Reference link labels

Use these standard labels for consistency:

- `[arXiv](...)` — preprint or paper
- `[GitHub](...)` — source code / dataset repository
- `[Website](...)` — official project page
- `[HF](...)` — HuggingFace model/dataset card
- `[PDF](...)` — direct PDF link when no arXiv page exists

---

## Quality Guidelines

- **Relevance**: The benchmark must evaluate or train VLA models or closely related embodied-AI systems.
- **Accessibility**: The benchmark (or at minimum its paper/description) must be publicly available.
- **Conciseness**: The Highlights column should be one sentence. Avoid marketing language.
- **Accuracy**: Double-check all links before submitting. Broken links will cause the automated check to fail.
- **Placement**: Add the entry to the most appropriate existing section. If no section fits, propose a new one in your PR description and we will discuss it.
- **Alphabetical / chronological order**: Within a table, entries do not need to be sorted, but try to group logically related entries together.

---

## Pull Request Checklist

Before submitting your PR, confirm the following:

- [ ] The benchmark is relevant to VLA or embodied AI evaluation
- [ ] The entry follows the three-column table format exactly
- [ ] The **Name** column contains a valid Markdown link
- [ ] The **References** column contains at least one working link
- [ ] The **Highlights** description is one sentence and starts with a `[Venue Year]` tag (if applicable)
- [ ] No existing entry for this benchmark is present in the list
- [ ] All links in your addition are reachable (not 404)
- [ ] The PR title clearly describes what is being added, e.g. `Add FooBench to Robot Manipulation`

---

## Code of Conduct

This project follows the [Contributor Covenant](https://www.contributor-covenant.org/) Code of Conduct. By participating, you agree to uphold a welcoming and respectful environment for everyone.

If you have questions or suggestions that are not suitable for a pull request, feel free to open an [issue](https://github.com/han-xudong/awesome-vla-benchmarks/issues).
