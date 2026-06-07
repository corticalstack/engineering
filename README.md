# engineering

A Claude Code plugin marketplace of engineering skills.

## Skills

- **terraform-engineer** - Terraform on Azure: modules, state management, multi-environment workflows.
- **fastapi-expert** - async FastAPI, Pydantic v2, SQLAlchemy async, auth, testing.
- **mcp-developer** - build and debug MCP servers/clients (TypeScript and Python SDKs).
- **python-pro** - type-safe, async modern Python (PEP 695 generics, TaskGroup, uv, Pydantic v2).
- **exploratory-data-analysis** - EDA across 200+ scientific data formats with quality metrics.

## Install

```
/plugin marketplace add corticalstack/engineering
/plugin install engineering@engineering
```

Restart Claude Code; the skills then appear as `/engineering:<name>` (e.g. `/engineering:terraform-engineer`).

## Licensing

The repository scaffolding (manifests, README) is MIT licensed. Individual skills retain their own licenses (all five are MIT; `exploratory-data-analysis` is by K-Dense Inc.).
