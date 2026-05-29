# meta_report_tool Design Document v1.0

## Overview

`meta_report_tool` is a first-class, persistent reporting and reflection engine tightly integrated with Unified MetaForge. It generates structured Meta-Report Cards, tracks Meta-DNA evolution, and can trigger downstream skills.

## Core Responsibilities

- Generate rich Meta-Report Cards (metrics, narrative, evolution delta, next options)
- Track and surface Meta-DNA changes across sessions
- Compute and display Hybrid Consistency-Engagement Scores
- Support multiple output formats (KickLang, Markdown, JSON, structured text)
- Enable chained execution via `trigger_next` parameter
- Persist reports for historical analysis

## Input Schema

```json
{
  "scope": "current_session" | "last_meta_iteration" | "full_meta_history",
  "include_dna_diff": boolean,
  "include_hybrid_score": boolean,
  "format": "kicklang" | "markdown" | "json" | "structured_text",
  "trigger_next": string | null
}
```

## Behavior

1. Loads current Meta-DNA + session state
2. Computes evolution delta and key metrics
3. Assembles coherent report
4. Persists report artifact
5. Optionally delegates to `trigger_next` via KickFlow
6. KickGuard validates before any chained trigger

## Persistence

Reports are stored under:
`/home/workdir/artifacts/meta-workflow-profiles/meta_reports/`

## Integration Points

- Automatically invoked at Phase 6 of the MetaForge protocol
- Manually invocable via `⫻cmd/trigger:meta_report_tool`
- Exposed as MCP tool for external clients