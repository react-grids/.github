<h1 align="center">React Grids</h1>

<p align="center">
  <strong>Build enterprise React data-grid apps faster with Ignite UI for React + AI-assisted workflows.</strong>
</p>

<p align="center">
  Demos, how-to guides, and complete projects showing how to combine
  <a href="https://www.infragistics.com/products/ignite-ui-react"><strong>Ignite UI for React</strong></a>,
  the <a href="https://github.com/IgniteUI/igniteui-cli"><strong>Ignite UI CLI</strong></a>,
  <a href="https://www.anthropic.com/claude-code"><strong>Claude Code</strong></a>,
  and <a href="https://modelcontextprotocol.io/"><strong>MCP servers</strong></a>
  to build production-ready React Data Grid, Tree Grid, and Hierarchical Grid applications.
</p>

<p align="center">
  <a href="https://www.infragistics.com/products/ignite-ui-react"><img alt="Ignite UI for React" src="https://img.shields.io/badge/Ignite%20UI-React-22d3ee?style=flat-square"></a>
  <a href="https://www.anthropic.com/claude-code"><img alt="Claude Code" src="https://img.shields.io/badge/Built%20with-Claude%20Code-8b5cf6?style=flat-square"></a>
  <a href="https://modelcontextprotocol.io/"><img alt="MCP" src="https://img.shields.io/badge/MCP-enabled-34d399?style=flat-square"></a>
</p>

---

## 📺 Watch the walkthroughs

| | |
|---|---|
| [<img src="https://img.youtube.com/vi/yfMnSccmQqU/hqdefault.jpg" width="320">](https://youtu.be/yfMnSccmQqU) | **Build a React Data Grid from the Ignite UI CLI with Claude Code**<br>Scaffolds the React app with the Ignite UI CLI, wires up MCP servers and Agent Skills, and uses Claude Code to build the full enterprise grid experience.<br><br>▶️ <https://youtu.be/yfMnSccmQqU> |

## 📝 Read the blog

**[Build a React Data Grid with Claude Code, Ignite UI CLI, and MCP Servers](https://www.infragistics.com/blogs/react-data-grid-claude-code)**

Walks through two AI-assisted workflows — adding Ignite UI to an existing React app, and starting from the Ignite UI CLI — and explains how Agent Skills and MCP servers feed real component context to the agent so it generates code that actually works.

---

## 🗂 Repositories

| Repo | What it shows |
|---|---|
| [**ignite-ui-react-data-grid-cli**](https://github.com/react-grids/ignite-ui-react-data-grid-cli) | Full enterprise React Data Grid built with the Ignite UI CLI + Claude Code: 26 columns, grouping, Excel-style filtering, paging, multi-row selection, pinning (left + right), Excel export, custom cell templates, eight built-in themes, a custom **Aurora Ops** theme, and a portal-rendered customer tooltip with a sparkline. |
| [**ignite-ui-react-data-grid-mcp-how-to**](https://github.com/react-grids/ignite-ui-react-data-grid-mcp-how-to) | Step-by-step how-to for wiring up the Ignite UI CLI MCP server and Theming MCP server with Claude Code (and other AI clients) so the agent has live access to component docs, API references, and design tokens. |
| [**igr-datagrid-treegrid**](https://github.com/react-grids/igr-datagrid-treegrid) | Side-by-side comparison of the Ignite UI React **Data Grid** and **Tree Grid** — when to pick each, and how their APIs overlap. |
| [**igr-datagrid-hierarchical**](https://github.com/react-grids/igr-datagrid-hierarchical) | **Data Grid** versus **Hierarchical Grid** — master/detail patterns, child row islands, and remote loading. |
| [**igr-treegrid-hierarchical**](https://github.com/react-grids/igr-treegrid-hierarchical) | **Tree Grid** versus **Hierarchical Grid** — flat self-referencing data vs nested per-level schemas. |

---

## 🧩 What you'll find in these demos

- **Real Ignite UI for React APIs** — `IgrGrid`, `IgrColumn`, `IgrPaginator`, `IgrGridToolbar*`, Excel-style filtering, grouping, pinning, column moving, row selection, Excel export
- **Cell templates** — typed `IgrCellTemplateContext`, custom indicators, avatars, and rich content
- **Theming** — eight prebuilt themes (Material / Indigo / Bootstrap / Fluent × Light / Dark) plus a fully custom theme layered via documented Ignite UI CSS variables
- **Production patterns** — async data fetching with `AbortController`, deterministic mock data, portal-rendered tooltips, virtualization-aware positioning
- **AI-assisted workflows** — Claude Code, Ignite UI Agent Skills, Ignite UI CLI MCP, and Ignite UI Theming MCP working together

---

## 🚀 How to use these demos

```bash
# 1. Clone the repo you want to explore
git clone https://github.com/react-grids/ignite-ui-react-data-grid-cli
cd ignite-ui-react-data-grid-cli

# 2. Install + run
npm install
npm start
```

Each repo's own README has the full quick-start, project layout, and notes specific to that demo.

### Wire up the Ignite UI MCP servers in Claude Code

Drop this into `.mcp.json` (or your client's equivalent) to give the agent live access to Ignite UI component docs, APIs, and design tokens:

```jsonc
{
  "mcpServers": {
    "igniteui-cli": { "command": "npx", "args": ["-y", "@infragistics/igniteui-cli-mcp"] },
    "igniteui-theming": { "command": "npx", "args": ["-y", "@infragistics/igniteui-theming-mcp"] }
  }
}
```

See [ignite-ui-react-data-grid-mcp-how-to](https://github.com/react-grids/ignite-ui-react-data-grid-mcp-how-to) for the full setup, including VS Code, Cursor, JetBrains, and Claude Desktop.

---

## 🛠 Stack the demos use

| | |
|---|---|
| Framework | React 19 + TypeScript |
| UI components | [`igniteui-react`](https://www.npmjs.com/package/igniteui-react), [`igniteui-react-grids`](https://www.npmjs.com/package/igniteui-react-grids) |
| Bundler | Vite |
| Scaffolding | [Ignite UI CLI](https://github.com/IgniteUI/igniteui-cli) |
| Agent | [Claude Code](https://www.anthropic.com/claude-code) |
| Context | [Ignite UI CLI MCP](https://www.infragistics.com/products/ignite-ui-react/cli-mcp) + [Ignite UI Theming MCP](https://www.infragistics.com/products/ignite-ui-react) + Agent Skills |

---

## 📚 Learn more

- 🌐 [Ignite UI for React](https://www.infragistics.com/products/ignite-ui-react)
- 📊 [React Data Grid documentation](https://www.infragistics.com/products/ignite-ui-react/react/components/grids/data-grid.html)
- 🌳 [React Tree Grid documentation](https://www.infragistics.com/products/ignite-ui-react/react/components/grids/tree-grid/overview)
- 🪜 [React Hierarchical Grid documentation](https://www.infragistics.com/products/ignite-ui-react/react/components/grids/hierarchical-grid/overview)
- ⚙️ [Ignite UI CLI](https://github.com/IgniteUI/igniteui-cli)
- 🤖 [Claude Code](https://www.anthropic.com/claude-code)
- 🧩 [Model Context Protocol](https://modelcontextprotocol.io/)

---

<p align="center"><sub>
  Built with ❤️ and Claude Code by the Infragistics team. Ignite UI for React components are licensed under the
  <a href="https://www.infragistics.com/legal/ultimate/license/">Ignite UI license</a>.
</sub></p>
