<h1 align="center">
  <br>
  Awesome Agent Skills
  <br>
</h1>

<p align="center">
  <strong>The universal skill repository for AI coding agents.</strong><br>
  One command. Works everywhere.
</p>

<p align="center">
  <a href="https://awesome.re">
    <img src="https://awesome.re/badge.svg" alt="Awesome" />
  </a>
  <img src="https://img.shields.io/badge/skills-50+-blue?style=flat-square" alt="Skills" />
  <img src="https://img.shields.io/badge/agents-6+-green?style=flat-square" alt="Compatible Agents" />
  <a href="https://www.apache.org/licenses/LICENSE-2.0">
    <img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=flat-square" alt="License: Apache-2.0" />
  </a>
  <img src="https://img.shields.io/npm/v/ai-agent-skills?style=flat-square&color=red" alt="npm" />
</p>

<p align="center">
  <a href="https://skillcreator.ai/discover"><strong>Browse Skills</strong></a> ·
  <a href="https://skillcreator.ai/build"><strong>Create Skills</strong></a> ·
  <a href="https://agentskills.io"><strong>Specification</strong></a> ·
  <a href="https://x.com/skillcreatorai"><strong>Follow Updates</strong></a>
</p>

---

## Quick Start

```bash
# Install any skill to any agent
npx ai-agent-skills install frontend-design
npx ai-agent-skills install pdf --agent cursor
npx ai-agent-skills install mcp-builder --agent vscode
```

That's it. The skill installs to the right location for your agent automatically.

## Why This Exists

Every major AI coding agent now supports skills. But they're scattered everywhere.

This repo curates the best in one place. Quality over quantity. All skills follow the [Agent Skills spec](https://agentskills.io).

## Compatible Agents

| Agent | Flag | Install Location |
|-------|------|------------------|
| Claude Code | `--agent claude` (default) | `~/.claude/skills/` |
| VS Code / Copilot | `--agent vscode` | `.github/skills/` |
| Cursor | `--agent cursor` | `.cursor/skills/` |
| Amp | `--agent amp` | `~/.amp/skills/` |
| Goose | `--agent goose` | `~/.config/goose/skills/` |
| OpenCode | `--agent opencode` | `~/.opencode/skills/` |
| Portable | `--agent project` | `.skills/` (works with any agent) |

## Contents

- [Skills](#skills)
  - [Document Processing](#document-processing)
  - [Development & Code Tools](#development--code-tools)
  - [Data & Analysis](#data--analysis)
  - [Business & Marketing](#business--marketing)
  - [Communication & Writing](#communication--writing)
  - [Creative & Media](#creative--media)
  - [Productivity & Organization](#productivity--organization)
  - [Collaboration & Project Management](#collaboration--project-management)
  - [Security & Systems](#security--systems)
- [Installation](#installation)
- [Creating Skills](#creating-skills)
- [Contributing](#contributing)
- [Resources](#resources)

## Skills

### Document Processing

| Skill | Description | Install |
|-------|-------------|---------|
| [docx](./document-skills/docx) | Create, edit, analyze Word docs with tracked changes, comments, formatting | `npx ai-agent-skills install docx` |
| [pdf](./document-skills/pdf) | Extract text, tables, metadata, merge & annotate PDFs | `npx ai-agent-skills install pdf` |
| [pptx](./document-skills/pptx) | Read, generate, and adjust slides, layouts, templates | `npx ai-agent-skills install pptx` |
| [xlsx](./document-skills/xlsx) | Spreadsheet manipulation: formulas, charts, data transformations | `npx ai-agent-skills install xlsx` |
| [Markdown to EPUB](https://github.com/smerchek/claude-epub-skill) | Converts markdown documents into professional EPUB ebook files | External |

### Development & Code Tools

| Skill | Description | Install |
|-------|-------------|---------|
| [artifacts-builder](./artifacts-builder) | Create elaborate HTML artifacts using React, Tailwind CSS, shadcn/ui | `npx ai-agent-skills install artifacts-builder` |
| [mcp-builder](./mcp-builder) | Create MCP servers for integrating external APIs with LLMs | `npx ai-agent-skills install mcp-builder` |
| [skill-creator](./skill-creator) | Guide for creating effective agent skills | `npx ai-agent-skills install skill-creator` |
| [webapp-testing](./webapp-testing) | Test web applications using Playwright automation | `npx ai-agent-skills install webapp-testing` |
| [changelog-generator](./changelog-generator) | Create user-facing changelogs from git commits | `npx ai-agent-skills install changelog-generator` |
| [frontend-design](https://github.com/skillcreatorai/Ai-Agent-Skills) | Production-grade UI components and styling | `npx ai-agent-skills install frontend-design` |
| [code-review](https://github.com/skillcreatorai/Ai-Agent-Skills) | Automated PR review patterns | `npx ai-agent-skills install code-review` |
| [code-refactoring](https://github.com/skillcreatorai/Ai-Agent-Skills) | Systematic code improvement techniques | `npx ai-agent-skills install code-refactoring` |
| [backend-development](https://github.com/skillcreatorai/Ai-Agent-Skills) | APIs, databases, server architecture | `npx ai-agent-skills install backend-development` |
| [python-development](https://github.com/skillcreatorai/Ai-Agent-Skills) | Modern Python 3.12+ patterns | `npx ai-agent-skills install python-development` |
| [javascript-typescript](https://github.com/skillcreatorai/Ai-Agent-Skills) | ES6+, Node, React, TypeScript | `npx ai-agent-skills install javascript-typescript` |
| [aws-skills](https://github.com/zxkane/aws-skills) | AWS development with CDK best practices | External |
| [D3.js Visualization](https://github.com/chrisvoncsefalvay/claude-d3js-skill) | D3 charts and interactive data visualizations | External |
| [Playwright Automation](https://github.com/lackeyjb/playwright-skill) | Browser automation for testing web apps | External |
| [iOS Simulator](https://github.com/conorluddy/ios-simulator-skill) | Interact with iOS Simulator for testing | External |

### Data & Analysis

| Skill | Description | Install |
|-------|-------------|---------|
| [CSV Summarizer](https://github.com/coffeefuelbump/csv-data-summarizer-claude-skill) | Analyze CSV files and generate insights with visualizations | External |
| [database-design](https://github.com/skillcreatorai/Ai-Agent-Skills) | Schema design and optimization | `npx ai-agent-skills install database-design` |

### Business & Marketing

| Skill | Description | Install |
|-------|-------------|---------|
| [brand-guidelines](./brand-guidelines) | Apply brand colors and typography to artifacts | `npx ai-agent-skills install brand-guidelines` |
| [competitive-ads-extractor](./competitive-ads-extractor) | Extract and analyze competitors' ads | `npx ai-agent-skills install competitive-ads-extractor` |
| [domain-name-brainstormer](./domain-name-brainstormer) | Generate domain name ideas and check availability | `npx ai-agent-skills install domain-name-brainstormer` |
| [internal-comms](./internal-comms) | Write internal communications and status reports | `npx ai-agent-skills install internal-comms` |
| [lead-research-assistant](./lead-research-assistant) | Identify and qualify high-quality leads | `npx ai-agent-skills install lead-research-assistant` |
| [job-application](https://github.com/skillcreatorai/Ai-Agent-Skills) | Cover letters and applications using your CV | `npx ai-agent-skills install job-application` |

### Communication & Writing

| Skill | Description | Install |
|-------|-------------|---------|
| [content-research-writer](./content-research-writer) | Research and write high-quality content with citations | `npx ai-agent-skills install content-research-writer` |
| [meeting-insights-analyzer](./meeting-insights-analyzer) | Analyze meeting transcripts for behavioral patterns | `npx ai-agent-skills install meeting-insights-analyzer` |
| [code-documentation](https://github.com/skillcreatorai/Ai-Agent-Skills) | Generate docs from code | `npx ai-agent-skills install code-documentation` |

### Creative & Media

| Skill | Description | Install |
|-------|-------------|---------|
| [canvas-design](./canvas-design) | Create visual art in PNG and PDF documents | `npx ai-agent-skills install canvas-design` |
| [image-enhancer](./image-enhancer) | Improve image quality, resolution, sharpness | `npx ai-agent-skills install image-enhancer` |
| [slack-gif-creator](./slack-gif-creator) | Create animated GIFs optimized for Slack | `npx ai-agent-skills install slack-gif-creator` |
| [theme-factory](./theme-factory) | Apply professional font and color themes | `npx ai-agent-skills install theme-factory` |
| [video-downloader](./video-downloader) | Download videos from YouTube and other platforms | `npx ai-agent-skills install video-downloader` |
| [algorithmic-art](https://github.com/skillcreatorai/Ai-Agent-Skills) | Generative art with p5.js | `npx ai-agent-skills install algorithmic-art` |

### Productivity & Organization

| Skill | Description | Install |
|-------|-------------|---------|
| [file-organizer](./file-organizer) | Intelligently organize files and find duplicates | `npx ai-agent-skills install file-organizer` |
| [invoice-organizer](./invoice-organizer) | Organize invoices and receipts for tax prep | `npx ai-agent-skills install invoice-organizer` |
| [raffle-winner-picker](./raffle-winner-picker) | Randomly select winners for giveaways | `npx ai-agent-skills install raffle-winner-picker` |
| [jira-issues](https://github.com/skillcreatorai/Ai-Agent-Skills) | Create and manage Jira issues from natural language | `npx ai-agent-skills install jira-issues` |
| [qa-regression](https://github.com/skillcreatorai/Ai-Agent-Skills) | Automated regression testing with Playwright | `npx ai-agent-skills install qa-regression` |
| [llm-application-dev](https://github.com/skillcreatorai/Ai-Agent-Skills) | Build LLM-powered applications | `npx ai-agent-skills install llm-application-dev` |

### Collaboration & Project Management

| Skill | Description | Install |
|-------|-------------|---------|
| [git-pushing](https://github.com/mhattingpete/claude-skills-marketplace) | Automate git operations and repository interactions | External |
| [review-implementing](https://github.com/mhattingpete/claude-skills-marketplace) | Evaluate code implementation plans | External |
| [test-fixing](https://github.com/mhattingpete/claude-skills-marketplace) | Detect failing tests and propose fixes | External |

### Security & Systems

| Skill | Description | Install |
|-------|-------------|---------|
| [computer-forensics](https://github.com/mhattingpete/claude-skills-marketplace) | Digital forensics analysis and investigation | External |
| [threat-hunting](https://github.com/jthack/threat-hunting-with-sigma-rules-skill) | Hunt for threats using Sigma detection rules | External |

## Installation

### One Command (Recommended)

```bash
# Install for Claude Code (default)
npx ai-agent-skills install <skill-name>

# Install for other agents
npx ai-agent-skills install <skill-name> --agent cursor
npx ai-agent-skills install <skill-name> --agent vscode
npx ai-agent-skills install <skill-name> --agent amp
```

### Manual Install

```bash
# Clone the repo
git clone https://github.com/skillcreatorai/Awesome-Agent-Skills.git

# Copy a skill to your skills directory
cp -r Awesome-Agent-Skills/canvas-design ~/.claude/skills/
```

### CLI Commands

```bash
npx ai-agent-skills list              # List all skills
npx ai-agent-skills search <query>    # Search skills
npx ai-agent-skills info <name>       # Get skill details
npx ai-agent-skills install <name>    # Install a skill
```

## Creating Skills

### Skill Structure

```
skill-name/
├── SKILL.md          # Required: Instructions and metadata
├── scripts/          # Optional: Helper scripts
├── templates/        # Optional: Document templates
└── resources/        # Optional: Reference files
```

### Basic Template

```markdown
---
name: my-skill-name
description: A clear description of what this skill does.
---

# My Skill Name

Detailed description of the skill's purpose.

## When to Use This Skill

- Use case 1
- Use case 2

## Instructions

[Detailed instructions for the AI agent]

## Examples

[Real-world examples]
```

### Two Ways to Create Skills

1. **Generate in 30 seconds**: [skillcreator.ai/build](https://skillcreator.ai/build)
2. **Build manually**: Follow the [Agent Skills spec](https://agentskills.io/specification)

## Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

### Quick Steps

1. Fork this repo
2. Add your skill folder with `SKILL.md`
3. Test across multiple agents
4. Submit PR with clear documentation

## Resources

### Official Documentation

- [Agent Skills Spec](https://agentskills.io) - The open standard
- [Anthropic Skills](https://github.com/anthropics/skills) - Official example skills
- [VS Code Skills Guide](https://code.visualstudio.com/docs/copilot/customization/agent-skills) - VS Code integration

### Tools

- [SkillCreator.ai](https://skillcreator.ai/build) - Generate skills from plain English
- [Browse Skills](https://skillcreator.ai/discover) - Visual skill gallery
- [npm Package](https://github.com/skillcreatorai/Ai-Agent-Skills) - CLI installer (`npx ai-agent-skills`)

## License

Apache License 2.0. Individual skills may have different licenses.

---

<p align="center">
  <sub>Curated by <a href="https://skillcreator.ai">SkillCreator.ai</a> · Originally forked from <a href="https://github.com/ComposioHQ/awesome-claude-skills">ComposioHQ/awesome-claude-skills</a></sub>
</p>
