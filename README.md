# AI-Native Salesforce SDLC

An interactive, single-page explainer on how GenAI, Claude, Claude Code and Claude Cowork fit into the complete software development lifecycle and Scrum process for a Salesforce development environment.

Open `index.html` in any browser. It is one self-contained file with inline CSS, JavaScript and SVG. The only external request is Google Fonts, and the page falls back to system fonts without it.

## What is inside

| Section | What it covers |
| --- | --- |
| Toolkit | GenAI foundations, Claude, Claude Code and Claude Cowork, plus a role-by-tool matrix (Product Owner, BA, Architect, Developer, Admin, QA, Release Manager, Scrum Master) |
| Reference architecture | AI-augmented Salesforce dev environment: humans, AI tools, MCP layer, org pipeline (scratch org to production), Git and CI/CD, guardrails |
| SDLC explorer | Six phases (Discover and Plan, Design, Build, Test, Deploy and Release, Operate and Improve) with what each tool does, Salesforce tasks, artifacts and the human checkpoint |
| Scrum explorer | Backlog refinement, sprint planning, daily standup, sprint review, retrospective and Definition of Done, with what AI assists and what stays human |
| Sprint timeline | A two-week sprint with Product Owner, dev team and AI agent lanes |
| Agent concepts | The agent loop, tools and MCP, context and memory (`CLAUDE.md`), skills, subagents, hooks, permissions, headless mode, evals, human-in-the-loop |
| Multi-agent pipeline | An orchestrator with 11 Salesforce specialist roles and a review loop |
| Hands-on snippets | A `CLAUDE.md` excerpt, a subagent definition, a GitHub Actions step using `claude -p`, and a bulk-safe Apex trigger handler |
| Worked example | One user story (auto-escalate Cases when SLA is at risk) walked through all six phases |
| Governance | Guardrail table and an autonomy ladder from assist to autonomous in a sandbox |
| Roadmap | 30/60/90-day adoption plan and qualitative measures |

The page has seven inline SVG diagrams, a light and dark theme toggle, copy buttons on code blocks, and a layout that works down to phone width.

## Run it

```bash
git clone https://github.com/srinipusuluri/ai-native-salesforce-sdlc.git
cd ai-native-salesforce-sdlc
open index.html        # macOS; use xdg-open on Linux, or just double-click the file
```

No build step and no dependencies.

## Notes

- The code samples are illustrative. Review them and compile them in a sandbox or scratch org before use. The Apex handler has not been compiled in an org.
- The page contains no performance numbers. Adoption measures are qualitative on purpose.
- Tooling changes quickly. Check current Claude Code and Salesforce CLI documentation before copying commands into a pipeline.

## Author

Srini Pusuluri, Salesforce Architect.
