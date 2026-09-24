# Resume

Master CV repository for **Muanai Khalifah Revindo**.

The repository uses LaTeX as the source of truth and is designed to maintain a complete professional inventory while allowing targeted CV variants for different roles.

## Positioning

**Applied AI Engineer focusing on Risk Intelligence and Operational Analytics**

The master CV is intentionally broader than any individual application CV. Targeted versions should select and prioritize existing content rather than maintain separate factual records.

## Repository Structure

```text
.
├── AGENTS.md              # Instructions for AI agents working on the repository
├── README.md              # Repository documentation
├── .gitignore
├── main.tex               # Main LaTeX entry point
│
├── config/                # LaTeX configuration and reusable formatting
│   ├── packages.tex
│   ├── layout.tex
│   └── commands.tex
│
├── content/               # Master CV content
│   ├── profile.tex
│   ├── education.tex
│   ├── experience.tex
│   ├── projects.tex
│   ├── research.tex
│   ├── achievements.tex
│   ├── leadership.tex
│   ├── certifications.tex
│   └── skills.tex
│
├── versions/              # Targeted CV variants
│   ├── ai-risk.tex
│   ├── ai-engineering.tex
│   ├── data-analytics.tex
│   └── general.tex
│
├── assets/                # Images, icons, or other static assets
│
└── output/                # Generated PDF files
```

## Workflow

The intended workflow is:

```text
Master content
      ↓
LaTeX source
      ↓
Targeted CV variant
      ↓
Compile
      ↓
PDF
      ↓
Review
```

The master content should remain the factual source of truth.

Targeted CVs may change:

- section ordering
- project selection
- bullet selection
- profile positioning
- skill emphasis

They should not change factual claims.

## Local Development

The project is intended to be edited using:

- VS Code
- LaTeX Workshop
- TeX Live
- Git

Compile `main.tex` through LaTeX Workshop or the local LaTeX toolchain.

## Version Control

Commit source files and configuration to Git.

Generated build artifacts should generally remain untracked unless there is a specific reason to preserve them.

## Content Principles

The CV prioritizes:

- factual accuracy
- concrete evidence
- meaningful metrics
- technical specificity
- concise writing
- credible positioning

Avoid unsupported claims, inflated descriptions, and generic buzzwords.

See [`AGENTS.md`](AGENTS.md) for detailed editing and AI-agent guidelines.

## Status

This repository is currently being built as a master CV system. Content and visual design are expected to evolve.