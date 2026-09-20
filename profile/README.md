## Give AI agents the *why* of your organisation

Your tracker knows what is being built. Your code knows how. Why — the goals,
the constraints, who you build for and what you have learned — lives in
documents, meetings and people's heads. People cope. Agents cannot.

**Org Context Spec** is an open standard for writing that down: plain Markdown
in a Git repository you own, laid out so that any agent can read it and any
person can review it. The model recommends, a human decides.

| | |
|---|---|
| **[orgspec](https://github.com/org-spec/orgspec)** | The specification, a starter template and Parkway — a small fictional organisation filled in end to end. Start here. |
| **[orgspec-mcp](https://github.com/org-spec/orgspec-mcp)** | The reference MCP server. Serves a context repository to Claude, ChatGPT, Cursor, VS Code and other MCP clients, turns proposed changes into pull requests, audits what the context does not say yet. `npx orgspec` |
| **[app.orgspec.org](https://app.orgspec.org)** | The same server, hosted. Install the GitHub App on a repository and connect your agent — nothing to run. |

### Try it in a minute

```sh
git clone https://github.com/org-spec/orgspec
claude mcp add parkway -- npx -y orgspec --context "$PWD/orgspec/example/org-context"
```

Then ask your agent what Parkway's constraints are, and why the app team is
building what it builds.

<sub>Extracted from daily use, not designed up front: in use since January 2026, in
software teams and in organisations with no engineers at all. MIT licensed.</sub>
