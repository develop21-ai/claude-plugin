# Develop21 Jobs — Claude Plugin

Develop21 is a job search planner and application tracker for Claude. With it, Claude searches for jobs across Indeed, LinkedIn, company careers pages and more, gathers new ones into one shortlist, and tracks each job you pursue through applications, interviews and offers.

It starts with your Career Profile. Claude turns your resume or CV and your conversation into a 20-dimension profile: experience highlights, strengths, skills, target roles, career goals, location, remote preferences and more. It loads whenever you use Develop21, so you never start over.

From that profile, Develop21 builds precise searches for the job search connectors you add here: Indeed, JobDataLake, ZipRecruiter, Dice, Aquent and Snagajob. It also builds searches on LinkedIn.com, HiringCafe.com, USAJOBS.gov and Naukri.com that you open and capture with the Develop21 Chrome extension, pulls openings from the careers pages of companies on your watchlist, and takes in forwarded job alerts.

From the shortlist you pick the jobs worth a look and bring in the full description with one click, a link or a paste. Claude then reviews your fit honestly, in both directions: are you right for the job, and is the job right for you?

Every job you take forward stays in your tracker, from application to interviews and offers, or a decision to pass. Your Develop21 Dashboard shows it all in one place. See the demo at https://mcp.develop21.ai

Resumes and cover letters are tailored job by job, in the employer's language and built from your own words. Truthful reframing only, never invented experience. Before you send anything, a free AI-writing check with Pangram shows whether it reads as yours.

Develop21 never applies for you or contacts employers. Your resume, documents and job descriptions are encrypted at rest (AES-256-GCM), and we don't sell your data or use it for ads. Your account is created when you first connect and is free within storage limits; Develop21 Storage at $4.95/month removes them.

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
