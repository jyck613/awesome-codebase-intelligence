# Awesome Codebase Intelligence Tools

**🔗 Live page: https://jyck613.github.io/awesome-codebase-intelligence/**

A curated, self-contained single-page site listing 60+ GitHub tools, MCP servers, and
knowledge-graph engines that help AI agents and developers understand any codebase and
onboard faster. Star counts are pulled live from GitHub via shields.io.

## What Makes This Different

- Curated for codebase understanding and onboarding, not general "awesome" breadth.
- Focused on practical tools for AI-agent workflows: repository analysis, indexing, MCP integrations, and graph-based context.
- Live GitHub star badges provide quick social proof without manual updates.
- Single-page, self-contained delivery keeps the project easy to fork, host, and modify.

## Contribution Guide (lightweight)

- Open an issue or PR with: tool name, repo URL, one-line value proposition, and category suggestion.
- Prefer actively maintained tools with clear docs and real codebase-intelligence utility.
- Keep descriptions concise and verifiable; avoid marketing copy.
- For PRs, update both the source Markdown and the embedded Markdown in `index.html` so the page and source stay in sync.

## License + Attribution

- License: no LICENSE file is currently included in this repository.
- Repository links and metadata reference GitHub-hosted projects.
- Live star badges are powered by shields.io.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The page. Renders the embedded Markdown with a custom layout + live GitHub star badges. Fully self-contained (works offline and on GitHub Pages). |
| `styles.css` | Custom dark theme + styling. |
| `awesome-codebase-intelligence.md` | The raw Markdown source (kept for reference / easy editing). |
| `og-image.html` | Source used to render the social preview image. |
| `og-image.png` | 1200×630 Open Graph / Twitter social preview image. |

> The Markdown is embedded inside `index.html` (in a `<script type="text/markdown">`
> block) so the page needs no server and has no CORS issues. If you edit
> `awesome-codebase-intelligence.md`, paste the updated content into that block too.

