# myceliumhq

Agent-facing, CLI-first tooling for personal knowledge systems and messaging — Trilium, paperless-ngx, Signal, and optional local semantic search over them.

| Repo | What it is |
|---|---|
| [`tri`](https://github.com/myceliumhq/tri) | CLI for TriliumNext notes |
| [`ppl`](https://github.com/myceliumhq/ppl) | CLI for paperless-ngx |
| [`sig`](https://github.com/myceliumhq/sig) | CLI + remote server for Signal messenger (built on signal-cli) |
| [`semanticd`](https://github.com/myceliumhq/semanticd) | Generic semantic-search sidecar — optional, source-agnostic |
| [`toolkit`](https://github.com/myceliumhq/toolkit) | Shared CLI conventions, local embeddings, and vector index used by the CLIs above |
| [`dev-config`](https://github.com/myceliumhq/dev-config) | Shared TypeScript/Biome config |

Each CLI is designed for coding agents first: token-cheap `--help`, deterministic exit codes, file-path-based binary I/O, and no interactive prompts. `tri`/`ppl` also ship standalone MCP servers where a shell isn't available; `sig` instead exposes a bearer-token-gated remote HTTP API (`sig-server`) that the CLI itself talks to, so the same `sig` binary works identically whether it's running next to its daemon or on a different machine entirely.
