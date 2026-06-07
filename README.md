# engineering

A Claude Code plugin marketplace of engineering skills, built on the open Agent Skills standard - so the same skills work in Claude Code, GitHub Copilot CLI, and other compatible agents.

## Skills

- **terraform-engineer** - Terraform on Azure: modules, state management, multi-environment workflows.
- **fastapi-expert** - async FastAPI, Pydantic v2, SQLAlchemy async, auth, testing.
- **mcp-developer** - build and debug MCP servers/clients (TypeScript and Python SDKs).
- **python-pro** - type-safe, async modern Python (PEP 695 generics, TaskGroup, uv, Pydantic v2).
- **exploratory-data-analysis** - EDA across 200+ scientific data formats with quality metrics.

## Install in Claude Code (plugin)

```
/plugin marketplace add corticalstack/engineering
/plugin install engineering@engineering
```

Restart Claude Code. The skills then appear in autocomplete as `/engineering:<name>` (e.g. `/engineering:terraform-engineer`).

## Install in GitHub Copilot CLI (and other agents)

The skills live in `.claude/skills/`, which Copilot CLI reads. Install them with the `gh skill` command (GitHub CLI **v2.90.0+**):

```
# all skills from this repo, available everywhere (user scope):
gh skill install corticalstack/engineering --agent github-copilot --scope user

# or just one skill:
gh skill install corticalstack/engineering terraform-engineer --agent github-copilot --scope user
```

In a Copilot CLI session: reload with `/skills reload`, confirm with `/skills info terraform-engineer`, then invoke by name, e.g. *"Use the /terraform-engineer skill to refactor this module."*

`gh skill` also accepts `--agent claude-code`, `cursor`, `gemini-cli`, `codex`, and many others, so the same repo serves any Agent-Skills-compatible tool. (Alternatively, copy a skill's folder into your project `.claude/skills/` or personal `~/.copilot/skills/` and run `/skills reload`.)

## Licensing

Repository scaffolding (manifests, README) is MIT. Individual skills retain their own licenses: all five are MIT (`exploratory-data-analysis` is authored by K-Dense Inc.).
