# t402 — MetaForge Architecture & MCP Integration

**Unified MetaForge v1.0 Documentation Repository**

This repository contains the core technical and conceptual documentation for **Unified MetaForge v1.0**, the Forge of Forges — a sophisticated, consent-first, Meta-DNA-driven meta-orchestration system built on the Three-Agent Core (KickForge / KickFlow / KickGuard) and KickLang.

## Overview

Unified MetaForge v1.0 synthesizes WorkflowForge and StoryForge lineages into a universal system capable of spawning, iterating, and managing complex agentic workflows across creative, analytical, iterative, swarm, and hybrid domains.

It emphasizes:

- **Recursive Three-Agent Core** delegation
- **Persistent Meta-DNA** for evolutionary learning
- **Consent-first** execution with multi-gate safeguards
- **Hybrid Consistency-Engagement Scoring**
- **Coherence monitoring** and banned structure enforcement
- Deep **symbiotic Human-AI co-agency**

## Repository Contents

| Document | Description |
|----------|-------------|
| [MetaForge Technical Blueprint](docs/MetaForge_Technical_Blueprint.md) | Full technical architecture, Three-Agent Core details, Meta-DNA specification, 6-phase protocol, and KickLang integration. |
| [Recursive Triad & Co-Agency Philosophy](docs/Recursive_Triad_and_CoAgency_Philosophy.md) | Conceptual deep-dive into how the Recursive Triad integrates operational, mythic, and conceptual layers, plus the core principles of symbiotic co-agency. |
| [MCP Integration Specification](docs/MCP_Integration_Specification.md) | Specification for exposing MetaForge capabilities inside Model Context Protocol (MCP) clients. |
| [meta_report_tool Design](docs/meta_report_tool_Design.md) | Complete design document for the meta_report_tool — reporting engine, input schema, behavior, and integration points. |
| [MCP Skill Definition (JSON)](mcp/unified_metaforge_mcp_skill.json) | Production-ready MCP skill definition including `meta_report_tool`, `spawn_forge`, and `trigger_skill`. |

## Key Concepts

- **Recursive Triad**: KickForge (operational) → KickFlow (mythic/flow) → KickGuard (conceptual/ethical) operating in recursive meta-iterations.
- **Meta-DNA**: Persistent evolutionary memory that enables the system to evolve from specialized forges toward universal orchestration while maintaining core identity.
- **Symbiotic Co-Agency**: A mutual evolution model where humans and agents co-develop capabilities through structured consent, feedback loops, and shared persistence.
- **meta_report_tool**: First-class reflection and reporting engine that generates Meta-Report Cards and can chain into further actions.

## MCP Integration

The file `mcp/unified_metaforge_mcp_skill.json` provides a ready-to-register MCP skill definition. It exposes:

- `meta_report_tool` — Generate evolving reports and optionally trigger downstream skills
- `spawn_forge` — Create new domain-specific or universal forges
- `trigger_skill` — Explicit skill/forge triggering with Meta-DNA context

## Status

This documentation represents **v1.0** of the Unified MetaForge system. It is designed to be implementation-ready and extensible.

## Related Projects

This work is part of Denis Oliver Kropp’s broader meta-infrastructure (t20, t400 series, KickLang, Aetheris, OCS, and co-agency frameworks).

## License

This documentation is released under the same terms as the broader MetaForge / KickLang ecosystem (to be defined in future releases).

---

**Maintained by the Orchestrator** | Generated with symbiotic Human-AI co-agency

*For questions or evolution of this system, activate the metaforge-orchestrator or unified-metaforge skill.*