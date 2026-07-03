# Awesome Codebase Intelligence Tools

**🔗 Live page: https://jyck613.github.io/awesome-codebase-intelligence/**

A curated, self-contained single-page site listing 60+ GitHub tools, MCP servers, and
knowledge-graph engines that help AI agents and developers understand any codebase and
onboard faster. Star counts are pulled live from GitHub via shields.io.

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

## Preview locally

Just open `index.html` in a browser, or serve the folder:

```bash
cd awesome-codebase-intelligence
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Publish to GitHub Pages

1. Create a new **public** repo on GitHub named `awesome-codebase-intelligence`.
2. From this folder, push the files:

   ```bash
   cd awesome-codebase-intelligence
   git init
   git add .
   git commit -m "Publish Awesome Codebase Intelligence Tools"
   git branch -M main
   git remote add origin https://github.com/jyck613/awesome-codebase-intelligence.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment**
   - **Source:** *Deploy from a branch*
   - **Branch:** `main` / `root` → **Save**

4. Wait ~1 minute. Your page will be live at:

   ```
   https://jyck613.github.io/awesome-codebase-intelligence/
   ```

## Repo "About" & Topics (set on GitHub)

The **About** panel (right sidebar of the repo page) is set via GitHub's UI, not files.
Click the ⚙️ gear next to **About** and enter:

- **Description:**
  `A curated list of 60+ GitHub tools, MCP servers & knowledge-graph engines that help AI agents and developers understand any codebase and onboard faster — with live star counts.`
- **Website:**
  `https://jyck613.github.io/awesome-codebase-intelligence/`
- **Topics** (categories — improves discovery/SEO; up to 20):
  `awesome` `awesome-list` `codebase` `codebase-analysis` `code-intelligence` `code-search` `knowledge-graph` `mcp` `mcp-servers` `ai-agents` `ai-tools` `developer-tools` `onboarding` `llm` `copilot` `claude` `cursor`

> Optionally check **"Use your GitHub Pages website"** in the About dialog to auto-fill the Website field once Pages is live.

If you have the GitHub CLI authenticated, you can set these from the terminal:

```bash
gh repo edit jyck613/awesome-codebase-intelligence \
  --description "A curated list of 60+ GitHub tools, MCP servers & knowledge-graph engines that help AI agents and developers understand any codebase and onboard faster — with live star counts." \
  --homepage "https://jyck613.github.io/awesome-codebase-intelligence/" \
  --add-topic awesome --add-topic awesome-list --add-topic codebase --add-topic codebase-analysis \
  --add-topic code-intelligence --add-topic code-search --add-topic knowledge-graph \
  --add-topic mcp --add-topic mcp-servers --add-topic ai-agents --add-topic ai-tools \
  --add-topic developer-tools --add-topic onboarding --add-topic llm \
  --add-topic copilot --add-topic claude --add-topic cursor
```

## Customize

- **Title / subtitle / author:** edit the `<header class="hero">` block in `index.html`.
- **SEO / social:** the `<title>`, meta description, Open Graph, and Twitter tags are in `<head>`; regenerate `og-image.png` from `og-image.html` if you change the branding.
- **Colors:** change the CSS variables at the top of `styles.css` (`:root`).
- **Content:** edit the Markdown inside the `<script id="source">` block in `index.html`.
