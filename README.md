# The Claude Code Missing Manual

A single-page recipe book of battle-tested Claude Code patterns — loops, hooks, agents, skills, and more. No framework, no build step. Open it and go.

🔗 **Live site:** [700799.github.io/claudecodey](https://700799.github.io/claudecodey)

---

## What's inside

11 categories, 200+ copy-paste examples organised by difficulty:

| # | Category | What it covers |
|---|----------|----------------|
| 🔄 | **Loops** | Recurring tasks, polling, long-running workflows with `/loop` and shell patterns |
| 🪝 | **Hooks** | PreToolUse, PostToolUse, Stop, and Notification hooks — automation at the event level |
| 📡 | **Monitoring** | The Monitor tool and background process patterns — stream live output without polling |
| 🤖 | **Agents** | Spawn subagents, run work in parallel, chain specialists, orchestrate multi-agent systems |
| 🚫 | **Never Hit Limits** | Token budgeting, context compaction, chunking, staying under rate limits while doing more |
| ⏰ | **Run 24 Hours** | Long-running autonomous workflows: persistence, checkpointing, error recovery |
| 🎯 | **Skills** | Custom slash commands that package multi-step workflows — build, chain, and share |
| 🏗️ | **Design Patterns** | Pipelines, observers, factories, circuit breakers, and other Claude-powered architectures |
| 🏆 | **Hall of Fame** | The most powerful, elegant, and surprising Claude Code patterns ever discovered |
| 📝 | **Markdown Essentials** | CLAUDE.md mastery, ADRs, runbooks, and the writing patterns that save the most tokens |
| 🔐 | **Secure Code** | Injection prevention, secrets management, auth, input validation, OWASP Top 10 |

Each example includes:
- A **difficulty badge** (Simple / Advanced / Expert / Over-Engineer / Avoid)
- A **"Why this matters"** explanation
- A **copy button** for the code snippet

---

## Using it

Filter by difficulty, search by keyword, or jump straight to a category pill. Everything runs client-side — no server, no login, no tracking.

**Keyboard shortcut:** Focus the search box and start typing.

---

## Running locally

```bash
git clone https://github.com/700799/claudecodey
cd claudecodey
python3 -m http.server 8080
# open http://localhost:8080
```

No dependencies, no `npm install`. It's one HTML file.

---

## Contributing

Found a pattern that saved your project? Open a PR and add it to the right category. Follow the existing example object shape:

```js
{
  title: 'Short descriptive title',
  difficulty: 'simple' | 'advanced' | 'expert' | 'overengineer' | 'mistakes',
  why: 'One sentence on why this pattern matters.',
  lang: 'bash' | 'javascript' | 'python' | 'sql' | ...,
  code: `your code here`,
}
```

---

## Tech

Pure HTML + CSS + vanilla JS. Syntax highlighting via [highlight.js](https://highlightjs.org/). No build toolchain, no framework, no bundler. Deploys to GitHub Pages on push to `main`.

---

## License

MIT
