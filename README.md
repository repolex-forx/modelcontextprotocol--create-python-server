# Repolex Knowledge Graph of modelcontextprotocol/create-python-server

RDF knowledge graph data for [modelcontextprotocol/create-python-server](https://github.com/modelcontextprotocol/create-python-server), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download modelcontextprotocol/create-python-server
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── b07744de4f10e92cfd1a98b51f7aac8ee5805d69
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── b07744de4f10e92cfd1a98b51f7aac8ee5805d69
│           └── chunk-001.nq.gz
├── blob
│   ├── 05c32c6053c1edd9a2faaf1b6ebf565c6650fa28.nq.gz
│   ├── 15170e59a50c9d8a471ef8e43b8f00089d9f7829.nq.gz
│   ├── 37a2a5ad2991c15f862556b86b733afd9101f240.nq.gz
│   ├── 3d48435454b105021b4f777c11b6b07d8d2ffea3.nq.gz
│   ├── 50073fa0558919f827734bf19794e9e64a911071.nq.gz
│   ├── 5e0d240c493a8555d4188bba6c07a433e3c08a5f.nq.gz
│   ├── 6293767d67a46b2d8c76330d20dc062dffd2dd5f.nq.gz
│   ├── 82f927558a3dff0ea8c20858856e70779fd02c93.nq.gz
│   ├── a66ea9a7f804c5084b45a30794ad976286d2cfef.nq.gz
│   ├── a7e7a8bf13236f9da3e5e6ccfe5916e9e16db35d.nq.gz
│   ├── b54038da0dff76103fb87c83338de21b1aa65eb7.nq.gz
│   ├── bc39f5cb127e6c1b87818982bdd84e333bced96f.nq.gz
│   ├── c35655dd2cc66b91798af12882f116bcff2ddf63.nq.gz
│   ├── c679ff384d7e7f313aebf670445ab80b0747c3ac.nq.gz
│   ├── c8cfe3959183f8e9a50f83f54cd723f2dc9c252d.nq.gz
│   ├── d6d45650a50268beffa75270e42e518272fde08c.nq.gz
│   ├── fddf83fa767819f66715778de7133ad2e8d0b457.nq.gz
│   └── fe64dba0c061980789add1ac4cbaf1428aedee8a.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── b07744de4f10e92cfd1a98b51f7aac8ee5805d69.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 26 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[modelcontextprotocol/create-python-server](https://github.com/modelcontextprotocol/create-python-server)

---
*Parsed on 2026-10-09 by [repolex](https://repolex.ai)*
