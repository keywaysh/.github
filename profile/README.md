<div align="center">
  <img src="https://keyway.sh/logo.svg" alt="Keyway" width="80" />
  <h1>Keyway</h1>
  <p><strong>GitHub-native secrets management for dev teams</strong></p>
  <p>If you have repo access, you have secret access. It's that simple.</p>

  <p>
    <a href="https://www.npmjs.com/package/@keywaysh/cli"><img src="https://img.shields.io/npm/v/@keywaysh/cli?color=blue&label=CLI" alt="npm version" /></a>
    <a href="https://keyway.sh"><img src="https://img.shields.io/badge/status-beta-yellow" alt="Status: Beta" /></a>
    <a href="https://docs.keyway.sh"><img src="https://img.shields.io/badge/docs-docs.keyway.sh-blue" alt="Documentation" /></a>
  </p>

  <p>
    <a href="https://keyway.sh">Website</a> ·
    <a href="https://docs.keyway.sh">Documentation</a> ·
    <a href="https://www.npmjs.com/package/@keywaysh/cli">NPM</a>
  </p>
</div>

---

## The Problem

Every team deals with this:

- "Can you send me the .env file?"
- "Which version is the right one?"
- Hours wasted onboarding new developers
- Nobody knows which secrets are up to date

## The Solution

```bash
npm install -g @keywaysh/cli
keyway pull
```

If you have access to the GitHub repo, you have access to its secrets. No invites, no separate accounts.

## How It Works

```
┌─────────────┐     push      ┌─────────────┐     pull      ┌─────────────┐
│  Your .env  │ ────────────► │   Keyway    │ ◄──────────── │  Teammate   │
│   file      │               │   (AES-256) │               │   machine   │
└─────────────┘               └─────────────┘               └─────────────┘
                                     │
                                     ▼
                              GitHub API
                           (access control)
```

1. **GitHub-native access** — Repo access = secret access
2. **Zero config** — Keep using `.env` files
3. **Encrypted at rest** — AES-256-GCM encryption

## Quick Start

```bash
# Install the CLI
npm install -g @keywaysh/cli

# Authenticate with GitHub
keyway login

# Initialize your project (from a Git repo)
keyway init

# Push your local secrets
keyway push

# New teammate joins? They just run:
keyway pull
```

## Features

| Feature | Description |
|---------|-------------|
| **Environments** | Separate secrets for `development`, `staging`, `production` |
| **Auto-detect** | Automatically detects your Git repo |
| **Dashboard** | Web UI to manage secrets and team access |
| **Audit log** | Track who accessed what and when |
| **CLI-first** | Designed for developers who live in the terminal |

## Open Source

| Repository | Description |
|------------|-------------|
| [@keywaysh/cli](https://github.com/keywaysh/cli) | Command-line interface |
| [keyway-docs](https://github.com/keywaysh/keyway-docs) | Documentation (Docusaurus) |

## Status

**Beta** — Keyway is production-ready but still evolving. Breaking changes may occur.

- Free for unlimited public repositories
- 1 private repository on free plan
- No credit card required

---

<div align="center">
  <p>
    <a href="https://keyway.sh"><strong>Get Started →</strong></a>
  </p>
  <p>
    <sub>Built by <a href="https://github.com/NicolasRitouet">@NicolasRitouet</a></sub>
  </p>
</div>
