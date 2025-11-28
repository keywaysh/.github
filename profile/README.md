<div align="center">
  <h1>Keyway</h1>
  <p><strong>Environment variables that sync like Git</strong></p>
  <p>Clone the repo. Pull the secrets. Start coding.</p>

  <a href="https://keyway.sh">Website</a> ·
  <a href="https://docs.keyway.sh">Documentation</a> ·
  <a href="https://www.npmjs.com/package/@keywaysh/cli">NPM</a>
</div>

---

## The Problem

Every team deals with this:

- 🔄 "Can you send me the .env file?"
- 💬 "Which version is the right one?"
- ⏰ Hours wasted onboarding new developers
- 🤷 Nobody knows which secrets are up to date

## The Solution

```bash
npm install -g @keywaysh/cli
keyway pull
```

That's it. If you have access to the repo, you have access to the secrets.

## How It Works

1. **GitHub-native access** — No invites, no separate accounts. Repo access = secret access.
2. **Zero config** — Keep using `.env` files. Keyway syncs them.
3. **Encrypted at rest** — AES-256-GCM. Your secrets stay secret.

## Quick Start

```bash
# Install
npm install -g @keywaysh/cli

# Authenticate with GitHub
keyway login

# Initialize your project
keyway init

# Push your secrets
keyway push

# New teammate joins? They just run:
keyway pull
```

## Repositories

| Repo | Description |
|------|-------------|
| [cli](https://github.com/keywaysh/cli) | Command-line interface |
| [keyway-site](https://github.com/keywaysh/keyway-site) | Marketing site & dashboard |
| [keyway-backend](https://github.com/keywaysh/keyway-backend) | API server |
| [keyway-docs](https://github.com/keywaysh/keyway-docs) | Documentation |

## Status

🟡 **Alpha** — Keyway is in active development. Data loss may occur during this phase.

Free for public repos. No credit card required.

---

<div align="center">
  <a href="https://keyway.sh">Get Started</a> ·
  <a href="mailto:hello@keyway.sh">Contact</a>
</div>
