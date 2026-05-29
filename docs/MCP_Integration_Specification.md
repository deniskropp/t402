# MCP Integration Specification for Unified MetaForge v1.0

## Purpose

This document defines how to expose the Unified MetaForge system (including Three-Agent Core, Meta-DNA, and meta_report_tool) as first-class capabilities inside Model Context Protocol (MCP) enabled clients.

## Recommended MCP Tool Structure

### Primary Skill/Tool: `unified_metaforge`

**Description**: Domain-agnostic meta-orchestration engine with persistent Meta-DNA, consent-first gates, and recursive Three-Agent Core delegation.

### Core Tools to Expose

1. `meta_report_tool` (detailed in separate design doc)
2. `spawn_forge`
3. `trigger_skill`

## Integration Requirements

- All tools must declare `meta_consent_level` handling.
- Hybrid scoring results should be surfaceable.
- Meta-DNA context should be injectable into tool calls when relevant.
- Chained triggering (`trigger_next` parameter) must be supported.
- Banned structure validation must occur before any chained execution.

## Security & Consent Considerations

- Explicit consent gates must be mirrored in the MCP client UX when possible.
- High-impact actions (swarm/hybrid modes, external triggers) should require secondary confirmation.
- All persistent state changes must be auditable.

## Recommended MCP Client Registration

Register the skill definition JSON (see `mcp/unified_metaforge_mcp_skill.json`) with your MCP host (Claude Desktop, Cursor, custom agents, etc.).