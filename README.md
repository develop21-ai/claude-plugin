# Develop21 — Claude Plugin

Develop21 tools help your AI assistant plan and run your job search. Get AI's help to search all the job boards, short-list results, manage your opportunities, create your resume and write applications.

This is the official Claude plugin for [Develop21](https://develop21.ai). It bundles:

- **The Develop21 connector** (`.mcp.json`) — a remote MCP server at `mcp.develop21.ai` that keeps your career profile, saved jobs, and documents, and carries Develop21's method for each task. Connecting creates your free account inside the OAuth flow — no forms, no card.
- **The career-coach skill** (`skills/develop21-career-coach/`) — teaches Claude when and how to use the connector: profile building, job search planning and execution, honest job-fit reviews, resumes and cover letters in the employer's language, application tracking.

## Install

**claude.ai (all plans):** follow the guided steps at [develop21.ai/start](https://develop21.ai/start) — pick Claude, download the plugin zip, upload it under Settings → Plugins, and connect.

**Claude Code** (once this plugin is listed in the community marketplace):

```
/plugin marketplace add anthropics/claude-plugins-community
/plugin install develop21@claude-community
```

To try it straight from source: `claude --plugin-dir ./claude-plugin` from a clone of this repository.

## Your data

Your career record lives in your Develop21 account, not in this plugin. View, download, or delete everything at [mcp.develop21.ai/account](https://mcp.develop21.ai/account). [Terms](https://develop21.ai/terms) · [Privacy](https://develop21.ai/privacy).

## Support

[support@develop21.com](mailto:support@develop21.com) — this repository is the published mirror of the plugin source, so issues and questions by email, please.
