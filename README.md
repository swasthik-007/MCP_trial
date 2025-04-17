# ✨ Cursor MCP Agent Setup

Welcome to your **Multi-Agent Configuration** for [Cursor](https://www.cursor.sh)! This setup integrates three powerful agents: Playwright, Airbnb, and DuckDuckGo Search—bringing automation, search, and real estate APIs to your editor. 🧠💻

---

## 🔧 Configuration Overview

Here's how your `.cursor/mcp.json` file is structured:

```json
{
  "mcpServers": {
    "playwright": {
      "command": "npx",
      "args": ["@playwright/mcp@latest"]
    },
    "airbnb": {
      "command": "npx",
      "args": ["-y", "@openbnb/mcp-server-airbnb"]
    },
    "duckduckgo-search": {
      "command": "npx",
      "args": ["-y", "duckduckgo-mcp-server"]
    }
  }
}
```

---

## 🤖 Playwright Agent - Browser Automation

![Playwright Agent](https://user-images.githubusercontent.com/3477155/171980802-36ad4e8d-8cb4-4f8d-a3db-bc101c66597c.gif)

This agent enables:
- 🌐 Navigation
- 🖱️ Element Clicking
- ⌨️ Typing into fields
- 📸 Screenshots
- 📄 PDF saving

**Usage Example:**
```js
// browser_navigate to https://example.com
```

---

## 🏡 Airbnb Agent - Real Estate Search

![Airbnb](https://media.giphy.com/media/xT0xeJpnrWC4XWblEk/giphy.gif)

Use this agent to:
- 🔍 Search Airbnb listings
- 📝 Fetch listing details

**Command:**
```bash
npx -y @openbnb/mcp-server-airbnb
```

---

## 🔎 DuckDuckGo Search Agent

![DuckDuckGo](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e4/DuckDuckGo_-_The_search_engine_that_doesn't_track_you.png/800px-DuckDuckGo_-_The_search_engine_that_doesn't_track_you.png)

Your private search buddy within the IDE. 🔐

**Use Cases:**
- 📖 Web search queries
- 🧠 Quick answers without leaving your editor

**Command:**
```bash
npx -y duckduckgo-mcp-server
```

---

## 🚀 How to Use Agents

1. **Open Cursor IDE**
2. Highlight a comment like:
```js
// browser_navigate to https://github.com
```
3. Press `Ctrl + I` (or use the command palette)
4. Boom 💥 — the agent runs!

> Tip: Keep the `.cursor/mcp.json` file in your project root to persist your agent setup.

---

## 📚 Helpful Links

- 🌍 [Cursor IDE](https://www.cursor.sh)
- 🧠 [MCP Agent Registry](https://github.com/cursor-ide/agent-registry)
- 💬 [Join the Discord](https://discord.gg/cursor)

---

## 🦾 Level Up Your Dev Workflow

With these agents, you can:
- Automate UI testing with Playwright
- Search listings with Airbnb
- Query the web with DuckDuckGo

> Happy hacking, dev! 💡🚀
