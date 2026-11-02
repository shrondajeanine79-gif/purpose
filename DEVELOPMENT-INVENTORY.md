# DEVELOPMENT INVENTORY — Shronda Studio AI

_Snapshot generated 2026-11-02 at migration time. See the post-migration update below for the owner-approved cleanup and current Git state._

## Post-migration update (2026-11-02)

- Local cleanup commit created on `main`; nothing was pushed.
- Removed tracked `.vs/` IDE state, `index.html.local-backup`, `src/main.rs.backup`, `index-changes.patch`, and zero-byte `dir`, `git`, `main)`.
- Removed an exposed `HIVE_API_KEY` line from `.gitignore`; the owner reports the key was rotated. The old value remains in Git history.
- Added ignore rules for regenerated IDE/backup artifacts.
- The working tree is clean and the branch is ahead of `origin/main` by the local cleanup commit(s).

## Overview

| Field | Value |
|---|---|
| Project | Shronda Studio AI |
| Purpose | Rust/Axum web application that serves a creative-workspace frontend and proxies chat requests to the Hive AI API. |
| GitHub | https://github.com/shrondajeanine79-gif/shronda-studio-ai.git |
| Visibility | PUBLIC |
| Local path | /home/shr/Projects/01-AI-PROJECTS/Shronda-Studio-AI |
| Active branch | main |
| Local commit | `990e4cf` (990e4cf676a8f820f3983714601c28210aa0d9bd) |
| Upstream | origin/main |
| Remote commit | `990e4cf` (990e4cf676a8f820f3983714601c28210aa0d9bd) |
| Synchronization | Up to date with origin/main |
| Working tree | 1 changed/untracked entries |
| Git history | Preserved in local `.git` |

## Build / Test / Run

```bash
cd /home/shr/Projects/01-AI-PROJECTS/Shronda-Studio-AI
cargo build
cargo run                       # serves on PORT, default 5500
cargo test                       # no test modules present
```

Runtime requirements: `HIVE_API_KEY` must be set (for example in a local `.env` read by `dotenvy`). `PORT` is optional.

## Configuration & environment files

- No `.env` or `.env.example` is present in the repository.
- Referenced variables: `HIVE_API_KEY` (required), `PORT` (optional, default 5500).
- `.gitignore` exists; a previously tracked key line was removed during cleanup and the owner reports the key was rotated.

## Important files

- `src/main.rs` — Axum server, CORS allow-list, static `index.html` serving, `/api/chat` proxy.
- `index.html` — single-page studio interface.
- `Cargo.toml` / `Cargo.lock` — Rust build definition and locked dependencies.

## Duplicates / potentially obsolete files

- Resolved during cleanup: `index.html.local-backup`, `src/main.rs.backup`, `index-changes.patch`, zero-byte `dir`, `git`, `main)`, and tracked `.vs/` (about 2.6 MB) were removed. They remain in Git history.

## Missing files / dependencies

- No `README.md`, no `.env.example`, no tests.
- Runtime cannot start without `HIVE_API_KEY`.

## Notes

Repository was clean and synced with `origin/main` at migration time.
## Directory tree

```text
.
|-- .gitignore
|-- Cargo.lock
|-- Cargo.toml
|-- DEVELOPMENT-INVENTORY.md
|-- dir
|-- git
|-- index-changes.patch
|-- index.html
|-- index.html.local-backup
|-- main)
`-- src
    |-- main.rs
    `-- main.rs.backup

2 directories, 12 files
```

_Excluded from display: `.git` internals, IDE caches, dependency caches, build outputs. Secret values are never displayed._

## Uncommitted local work

```text
## main...origin/main [ahead of origin by local cleanup commit(s)]
```

Working tree is clean.

