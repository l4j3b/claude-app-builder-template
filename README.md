# Claude App Builder: workspace template

> [!WARNING]
> ⚠️ **Archived proof of concept (July 2025).** Kept here as a record. It is not maintained.

The starter Next.js app for Claude App Builder workspaces, set up as a GitHub template repository. It is a Next.js 15, React 19 and Tailwind 4 app with a single page for Claude to edit. `next.config.ts` adds permissive CORS headers so the builder website can call the app from another origin.

## Part of Claude App Builder

Claude App Builder was a Lovable-style tool that built web apps from a prompt.

| Repo | Role | Ran on |
| --- | --- | --- |
| [`claude-app-builder-frontend`](https://github.com/l4j3b/claude-app-builder-frontend) | The website and user entry point, with a chat panel that streams Claude's work next to a live preview of the user's app | Vercel |
| [`claude-app-builder-backend`](https://github.com/l4j3b/claude-app-builder-backend) | The user workspaces, each running the Claude Code API and the user's Next.js app | Gitpod, then Fly.io |
| `claude-app-builder-template` (this repo) | The starter Next.js app for a workspace | GitHub template |

## Running it

```bash
pnpm install
pnpm dev
```

Then open http://localhost:3000.
