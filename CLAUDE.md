# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**tube-forge-agents-team** is a YouTube content production pipeline using specialized Claude Code agents. The system orchestrates multiple AI agents to produce complete video assets for a YouTube channel focused on AI automation for Italian small businesses.

**Current Status**: Niche validated (STRONG GO) - see `niche-analysis-ai-automations-small-business.md` for the complete market research.

## Agent Architecture

The project uses a multi-agent workflow where each agent handles a specific phase of content production:

| Agent | Role | Input | Output | Status |
|-------|------|-------|--------|--------|
| **niche-scout-alpha** | Market research & niche validation | Topic/theme | GO/NO-GO verdict + competitor analysis | ✅ Defined |
| **content-strategos** | Content planning | Approved niche + feedback | 10-video content roadmap | 📋 Planned |
| **narrative-forge** | Script & asset writing | Video plan | Script, NotebookLM source, video prompts | 📋 Planned |
| **media-synth-core** | Technical production | Script + prompts | Production workflow, audio/video guides | 📋 Planned |
| **broadcast-ops** | SEO & publishing | Final video | YouTube metadata, upload process | 📋 Planned |
| **metric-loop-sentinel** | Analytics feedback | Published video metrics | Performance insights for strategy refinement | 📋 Planned |

### Invoking Agents

Agents are invoked using the Task tool with `subagent_type` matching the agent name:

```
Task(subagent_type="niche-scout-alpha", prompt="Analyze the niche: AI tools for restaurants")
```

### Agent Definition Location

Agent configurations are stored in `.claude/agents/` as markdown files with YAML frontmatter:

```yaml
---
name: agent-name
description: Agent purpose
model: sonnet
color: red
---
```

Agents have WebSearch permission enabled via `.claude/settings.local.json`.

### Creating New Agents

To add a new agent, create a markdown file in `.claude/agents/` with:
1. YAML frontmatter specifying `name`, `description`, `model`, and `color`
2. System prompt instructions defining the agent's behavior and output format

## Output Structure

All production assets are organized under `output/` by video:

```
output/
  video1-ai-automazioni/
    00-production-summary.md    # Overview and checklists
    01-script-completo.md       # Full Italian script with timestamps
    02-notebooklm-source.md     # Source for NotebookLM audio generation
    03-video-prompts.md         # AI video generation prompts (Kling/Sora)
    04-youtube-assets.md        # Titles, descriptions, tags
    05-lead-magnet.md           # Checklist PDF concept + email sequence
    06-audio-instructions.md    # Voice recording/AI narration guide
    07-video-generation-guide.md # Detailed AI scene generation instructions
    08-production-workflow.md   # Complete editing workflow (DaVinci/CapCut)
    09-asset-checklist.md       # Pre-flight checklist for all deliverables
```

## Typical Workflow

1. Run **niche-scout-alpha** to validate topic viability
2. If GO, run **content-strategos** to plan video series
3. For each video, run **narrative-forge** to create scripts and prompts
4. Run **media-synth-core** to generate production guides
5. After manual video production, run **broadcast-ops** for SEO/upload
6. Post-publish, run **metric-loop-sentinel** for analytics feedback

### Workflow Data Flow

Research outputs (like `niche-analysis-*.md`) feed into subsequent agents. Always reference prior analysis when invoking downstream agents:

```
# Example: After niche-scout-alpha produces analysis
Task(subagent_type="content-strategos",
     prompt="Create 10-video plan based on niche-analysis-ai-automations-small-business.md")
```

### Agent Chaining Pattern

Each agent reads outputs from previous agents and writes to specific files:

```
niche-scout-alpha → niche-analysis-*.md (root)
       ↓
content-strategos → content-roadmap.md (root)
       ↓
narrative-forge → output/videoN-*/01-05.md
       ↓
media-synth-core → output/videoN-*/06-09.md
       ↓
broadcast-ops → YouTube upload process
       ↓
metric-loop-sentinel → feedback loop to content-strategos
```

## Key Conventions

- **Language**: Primary content is in Italian; metadata supports bilingual (IT/EN) strategy
- **Target Audience**: Italian SME owners, 28-55 years, non-technical
- **Video Format**: 12-15 minute tutorials with timestamps
- **Tone**: Friendly expert, practical, ROI-focused, no hype
- **Currency**: Always EUR, not USD
- **Tools Referenced**: Focus on Italian-compatible tools (Fatture in Cloud, etc.)

## External Tools in Workflow

- **NotebookLM**: Audio narration generation from source documents
- **Kling AI / Sora / Runway**: AI video scene generation
- **DaVinci Resolve / CapCut**: Video editing
- **Canva**: Thumbnails and graphics
- **YouTube Studio**: Publishing and analytics

## Creating New Videos

When creating assets for a new video:

1. Create a new folder under `output/` with pattern `videoN-short-name/` (e.g., `video2-chatbot-whatsapp/`)
2. Generate all numbered asset files (00 through 09)
3. Start with `00-production-summary.md` as the overview document
4. Each agent writes to specific numbered files in the sequence

## File Naming Conventions

- Agent definitions: `.claude/agents/{agent-name}.md`
- Niche analysis: `niche-analysis-{topic-slug}.md` (root directory)
- Video folders: `output/video{N}-{short-kebab-name}/`
- Video assets: `{NN}-{asset-name}.md` (numbered 00-09)
