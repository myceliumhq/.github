# myceliumhq

Agent-facing, CLI-first tooling for personal knowledge systems — Trilium, paperless-ngx, and optional local semantic search over them.

| Repo | What it is |
|---|---|
| [`tri`](https://github.com/myceliumhq/tri) | CLI for TriliumNext notes |
| [`ppl`](https://github.com/myceliumhq/ppl) | CLI for paperless-ngx |
| [`semanticd`](https://github.com/myceliumhq/semanticd) | Generic semantic-search sidecar — optional, source-agnostic |
| [`toolkit`](https://github.com/myceliumhq/toolkit) | Shared CLI conventions, local embeddings, and vector index used by the CLIs above |
| [`dev-config`](https://github.com/myceliumhq/dev-config) | Shared TypeScript/Biome config |

Each CLI is designed for coding agents first: token-cheap `--help`, deterministic exit codes, file-path-based binary I/O, and no interactive prompts. MCP servers are also available where a shell isn't.
