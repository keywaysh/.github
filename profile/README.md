<div align="center">
  <h1>Keyway</h1>
  <p><strong>Stop sharing .env files in Slack.</strong></p>
  <p>3 commands. Your whole team has the secrets.</p>

  <p>
    <a href="https://docs.keyway.sh">Docs</a> ·
    <a href="https://keyway.sh">Website</a> ·
    <a href="https://app.keyway.sh">Dashboard</a> ·
    <a href="https://github.com/keywaysh/cli">CLI</a>
  </p>
</div>

---

```bash
brew install keywaysh/tap/keyway
keyway login
keyway push
```

Your teammate runs `keyway pull`. Done.

---

## Before Keyway

1. Find the .env in Slack / Notion / 1Password
2. Copy-paste, hope it's the right one
3. New dev joins → repeat for each project
4. Dev leaves → hope they deleted everything

## With Keyway

```bash
keyway run -- npm start
```

No .env file. Secrets injected at runtime.

---

## Why Keyway?

- **3 commands** — Install, push, run. That's it.
- **Zero onboarding** — New dev? `keyway pull`. Dev leaves? Revoke repo access, done.
- **AI-safe** — Secrets never in files, never in AI context.
- **Deploy sync** — Push to Vercel, Netlify, Railway with `keyway sync`.

## AI-Safe Secrets

Secrets should never end up in your AI context. Keyway keeps them out.

```bash
# Inject secrets at runtime, never in files
keyway run -- npm start

# MCP server for AI assistants (Claude, Cursor, etc.)
keyway mcp
```

With `keyway run`, secrets are injected as environment variables at runtime — they never touch disk. The MCP server lets AI assistants help you manage secrets safely, without exposing values in the conversation.

## Integrations

Sync secrets to Vercel, Netlify, Railway — one command.

```bash
keyway sync vercel
```

## Repositories

| Repo | Description |
|------|-------------|
| [cli](https://github.com/keywaysh/cli) | Go CLI (Homebrew, npm) |
| [keyway-backend](https://github.com/keywaysh/keyway-backend) | Fastify API |
| [keyway-crypto](https://github.com/keywaysh/keyway-crypto) | Go gRPC encryption service (open-sourcing soon) |
| [keyway-action](https://github.com/keywaysh/keyway-action) | GitHub Action |
| [keyway-mcp](https://github.com/keywaysh/keyway-mcp) | MCP server for AI assistants |
| [keyway-docs](https://github.com/keywaysh/keyway-docs) | Documentation |

---

<div align="center">
  <a href="https://docs.keyway.sh"><strong>Get Started →</strong></a>
  <br><br>
  <sub>Built by <a href="https://github.com/NicolasRitouet">@NicolasRitouet</a></sub>
</div>
