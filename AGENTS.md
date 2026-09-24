# AGENTS.md

## Project Overview

This repository is the source of truth for Muanai Khalifah Revindo's master CV.

The CV is maintained as a structured LaTeX project and is intended to generate multiple targeted CV variants from one factual master source.

Primary positioning:

> Applied AI Engineer focusing on Risk Intelligence and Operational Analytics

The repository should preserve a complete and accurate inventory of the user's education, experience, projects, research, publications, achievements, leadership, certifications, and technical skills.

---

## Core Principles

### 1. Factual accuracy is the highest priority

Never invent, infer, inflate, or embellish:

- job titles
- company or organization names
- dates
- responsibilities
- metrics
- technical implementations
- project outcomes
- competition rankings
- publication status
- certifications
- technologies used
- business impact

If information is missing or ambiguous, mark it as `TODO` or ask for clarification.

Do not convert an implication into a factual claim.

For example:

- Do not turn "worked with a team" into "led a team".
- Do not turn "built a prototype" into "deployed in production".
- Do not turn "used AI" into "developed an AI system" without supporting context.

---

## 2. Master CV is the source of truth

The master CV should contain the user's complete relevant professional inventory, even when some items will not appear in a particular 1–2 page CV.

Targeted CVs should be created by selecting and reordering existing information.

Do not create contradictory versions of the same experience.

If a targeted version requires a claim that does not exist in the master content, flag it instead of inventing it.

---

## 3. Optimize for evidence, not buzzwords

Prefer:

- concrete technical work
- measurable results
- meaningful scale
- engineering decisions
- business or operational context
- research methodology
- demonstrated outcomes

Avoid generic claims such as:

- passionate AI enthusiast
- highly motivated
- results-driven
- innovative problem solver
- AI expert
- machine learning ninja

unless the wording is directly supported by context and genuinely useful.

Let the work demonstrate capability.

---

## 4. Preserve the user's voice

CV language should be:

- concise
- professional
- technically credible
- specific
- understated
- readable

Avoid excessive corporate language and exaggerated achievement framing.

Do not make the CV sound like generic AI-generated recruiting copy.

---

# Repository Structure

The repository should follow this general structure:

```text
muanai-cv/
├── AGENTS.md
├── README.md
├── .gitignore
│
├── main.tex
│
├── config/
│   ├── packages.tex
│   ├── layout.tex
│   └── commands.tex
│
├── content/
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
├── versions/
│   ├── ai-risk.tex
│   ├── ai-engineering.tex
│   ├── data-analytics.tex
│   └── general.tex
│
├── assets/
│
└── output/
```

The exact structure may evolve as the project grows, but unnecessary complexity should be avoided.

---

# Content Organization

## Profile

Keep the professional positioning concise.

The profile should communicate the user's direction rather than attempting to summarize the entire CV.

Current positioning:

> Applied AI Engineer focusing on Risk Intelligence and Operational Analytics

Do not automatically include this exact wording in every CV variant. Adapt it when a specific application requires a more precise positioning.

---

## Experience

Each experience should ideally contain:

```text
Role
Organization
Location (if useful)
Date
Context
Responsibilities
Technical work
Measured outcomes
```

Prioritize bullets with concrete evidence.

Avoid repeating the same information across multiple bullets.

---

## Projects

Projects should emphasize:

1. Problem
2. Technical approach
3. Engineering decisions
4. Result or evaluation

For technical projects, include metrics when they are meaningful and verified.

Examples of useful evidence include:

- model performance
- latency
- throughput
- dataset scale
- optimization gains
- user evaluation
- system constraints
- operational impact

Do not include metrics merely to make a project appear impressive.

---

## Education

Include:

- institution
- degree/program
- dates
- GPA when useful
- relevant academic information when it strengthens the target CV

Avoid listing every course by default.

---

## Research and Publications

Clearly distinguish:

- published
- accepted
- submitted
- ongoing research
- thesis

Never imply publication status that has not been confirmed.

---

## Achievements

Use precise descriptions.

For competitions, preserve the actual stage/ranking.

For example:

```text
Finalist
Runner-up
Top 24
Top 8%
Semi-finalist
```

Do not transform these into subjective labels such as "elite", "top-tier", or "award-winning" unless the source itself establishes that wording.

---

## Skills

Skills should represent technologies and methods the user can substantively discuss.

Avoid creating enormous keyword lists solely for ATS optimization.

Skills should be grouped logically, for example:

```text
Languages
Machine Learning
Data / Analytics
Backend / Engineering
Infrastructure / Tools
```

The exact categories can evolve with the CV.

---

# AI Agent Workflow

Before making substantial changes:

1. Inspect the relevant files.
2. Understand the existing structure.
3. Identify factual dependencies.
4. Make the smallest reasonable change.
5. Compile the affected LaTeX document.
6. Check for LaTeX errors and warnings.
7. Review the resulting PDF when visual layout matters.
8. Report what changed.

Do not rewrite unrelated sections.

---

# LaTeX Rules

## Compilation

The final project must compile successfully.

Do not introduce packages unnecessarily.

Prefer standard, well-supported LaTeX packages.

Keep formatting decisions centralized in:

```text
config/packages.tex
config/layout.tex
config/commands.tex
```

Avoid duplicating formatting logic across content files.

---

## Content vs Presentation

Content files should primarily contain CV information.

Presentation logic should live in configuration and reusable commands.

For example, prefer:

```latex
\experience{Role}{Organization}{Date}{...}
```

over repeatedly writing custom formatting for every experience.

---

## Links

Use hyperlinks for:

- GitHub
- LinkedIn
- portfolio
- project repositories
- publications

Use readable link text where appropriate.

Do not expose unnecessarily long raw URLs in the visible CV.

---

# Targeted CV Variants

Targeted CVs should be derived from the master content.

Potential variants include:

### AI / Risk Intelligence

Emphasize:

- machine learning
- risk modeling
- explainability
- regulatory-aware systems
- decision support
- data analysis

### AI Engineering

Emphasize:

- model integration
- backend engineering
- APIs
- data pipelines
- performance optimization
- Docker
- system design

### Data / Operational Analytics

Emphasize:

- analytics
- business processes
- automation
- reporting
- operational decision support
- data transformation

### General

Use a balanced representation of the strongest relevant experience.

Do not create a separate factual database for each variant.

---

# Editing Rules

When editing an existing bullet:

- preserve factual meaning
- improve clarity before adding sophistication
- prefer shorter sentences
- remove redundant words
- retain meaningful technical details
- retain meaningful metrics

When shortening content, remove low-value information rather than deleting evidence from stronger achievements.

When expanding content, add context only when it is factually supported.

---

# Review Checklist

Before considering a CV version complete, verify:

### Facts

- [ ] Dates are correct
- [ ] Titles are correct
- [ ] Organizations are correct
- [ ] Metrics are correct
- [ ] Technologies are actually used
- [ ] Competition results are accurate
- [ ] Publication status is accurate

### Content

- [ ] Strongest relevant experiences are prioritized
- [ ] Bullets communicate contribution rather than job descriptions
- [ ] Metrics are meaningful
- [ ] No unnecessary buzzwords
- [ ] No unsupported claims

### LaTeX

- [ ] Compiles successfully
- [ ] No broken references
- [ ] No unintended overflow
- [ ] No awkward page breaks
- [ ] Links work
- [ ] Typography is consistent

### Output

- [ ] Target page count is satisfied
- [ ] Content remains readable at normal PDF zoom
- [ ] Important information is visually easy to find
- [ ] The PDF filename is descriptive

---

# AI Agent Boundaries

The AI agent may:

- reorganize CV content
- improve wording
- propose stronger bullet structures
- create targeted CV variants
- refactor LaTeX
- improve layout
- identify inconsistencies
- identify missing information
- compile and inspect the document

The AI agent must not:

- fabricate achievements
- fabricate metrics
- fabricate responsibilities
- fabricate employment dates
- fabricate technical implementations
- claim production deployment without evidence
- claim leadership without evidence
- change competition rankings
- change publication status
- silently remove factual information from the master CV

When uncertain, ask rather than assume.

---

# Definition of Done

A CV change is considered complete only when:

1. The content is factually supported.
2. The LaTeX source is maintainable.
3. The document compiles successfully.
4. The generated PDF has been visually checked when layout was changed.
5. The change does not unnecessarily break other CV variants.