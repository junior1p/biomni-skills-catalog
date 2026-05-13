# Contributing to Biomni Skills Catalog

Thank you for your interest in contributing! This guide explains how to add new skills,
update existing documentation, and submit pull requests.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How to Contribute](#how-to-contribute)
- [Adding a New Skill](#adding-a-new-skill)
- [Documentation Format](#documentation-format)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)

---

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).
By participating, you agree to uphold a respectful and inclusive environment.

---

## How to Contribute

There are several ways to contribute:

| Type | Description |
|---|---|
| **New Skill** | Document a new analytical skill available on the Biomni platform |
| **Update** | Improve or correct existing skill documentation |
| **Bug Report** | Report broken links, outdated information, or formatting issues |
| **Translation** | Help translate documentation into additional languages |

---

## Adding a New Skill

### Step 1 — Verify the skill exists on Biomni

Confirm the skill is available on the Biomni platform by loading it:

```python
Skill(action="load", name="<skill-name-or-id>")
```

### Step 2 — Choose the right category file

Add your skill entry to the appropriate file in `skills/`:

| File | Category |
|---|---|
| `skills/01_single_cell.md` | Single-Cell & Spatial Transcriptomics |
| `skills/02_bulk_omics.md` | Bulk Omics Analysis |
| `skills/03_epigenomics.md` | Epigenomics |
| `skills/04_genetics.md` | Genetics & Variant Analysis |
| `skills/05_drug_discovery.md` | Drug Discovery & Clinical |
| `skills/06_other_skills.md` | Sequence, Structural Biology, Data Management |

### Step 3 — Follow the documentation template

Each skill entry must include the following sections:

```markdown
## N. Skill Display Name

- **Skill ID**: `skill-id-here`
- **Applicable Scenarios**: When to use this skill
- **Key Features**:
  - Feature 1
  - Feature 2
  - Feature 3
- **Dependencies**: Tool A, Tool B, Language/Framework
```

### Step 4 — Update the summary tables

After adding the skill entry in the category file, also update:

1. The summary table in `README.md` (English)
2. The summary table in `README_CN.md` (Chinese)
3. The skill count badges at the top of both README files

---

## Documentation Format

### General Rules

- Use **Markdown** for all documentation
- Keep descriptions **concise and factual** — one sentence per feature
- Use **backticks** for all Skill IDs, code, and technical terms
- Use **sentence case** for headings (not Title Case for body text)
- Avoid marketing language; focus on what the skill actually does

### Skill ID Format

Skill IDs use lowercase letters, numbers, and hyphens only:

```
scrnaseq-scanpy-core-analysis    ✅
scRNAseq_Scanpy_Core_Analysis    ❌
```

### Language

- `README.md` — English only
- `README_CN.md` — Chinese only
- `skills/*.md` — English (primary); Chinese translation welcome as a separate PR

---

## Pull Request Process

1. **Fork** this repository and create a feature branch:
   ```bash
   git checkout -b feat/add-new-skill-name
   ```

2. **Make your changes** following the documentation format above.

3. **Verify** all links and Skill IDs are correct.

4. **Commit** with a clear, conventional commit message:
   ```
   docs: add <skill-name> to <category>
   docs: update <skill-name> description
   fix: correct broken link in 03_epigenomics.md
   ```

5. **Open a Pull Request** against the `main` branch with:
   - A clear title describing the change
   - A brief description of what was added or changed
   - Reference to any related issue (if applicable)

6. A maintainer will review your PR within **5 business days**.

---

## Reporting Issues

Found a broken link, outdated information, or a missing skill?

Please [open an issue](https://github.com/junior1p/biomni-skills-catalog/issues) with:

- **Issue type**: Bug / Outdated content / Missing skill / Other
- **Location**: File name and section
- **Description**: What is wrong and what it should say
- **Suggested fix** (optional)

---

*Thank you for helping make Biomni Skills Catalog better for the entire research community!*
