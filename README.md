# Repolex Knowledge Graph of django-commons/dj-database-url

RDF knowledge graph data for [django-commons/dj-database-url](https://github.com/django-commons/dj-database-url), parsed by [repolex](https://repolex.ai).

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
rlex download django-commons/dj-database-url
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 9e2eab246532e6faa3037ebc0ffb433ea9eb2356
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 9e2eab246532e6faa3037ebc0ffb433ea9eb2356
│           └── chunk-001.nq.gz
├── blob
│   ├── 00d3cc9c1dcf4ef1fba69c594536e712d71182d6.nq.gz
│   ├── 3aaf15160fdd8c073080582783ad1207ec9cf598.nq.gz
│   ├── 4385f7353abc7d3b505825dae3a5c063737fe870.nq.gz
│   ├── 44540c8ef06d4b56760c11058f368c2265de532c.nq.gz
│   ├── 4a0c37517ffbc49902c9f2ecfd5c156ad0f6e4fc.nq.gz
│   ├── 7b49b475f9dafa1d385497220471baf77bb1374c.nq.gz
│   ├── 88e457a64b144b15ba36b3ec6e14fc67d0561590.nq.gz
│   ├── 8bf0c461d9c9f7d1b128463ba3c00e3ef307c2f4.nq.gz
│   ├── 8c592a2e54427fbd741ff1dd6eea1d2bfd52737e.nq.gz
│   ├── 9157693fb54d850348583e530580203bfce50b01.nq.gz
│   ├── 998421d93aae6b4ec31b237953cdbe0290458aaa.nq.gz
│   ├── a332e24c9f3665853457fce1d0bca685105d93c8.nq.gz
│   ├── b9a7560fa83c5554142c6ffa2b2d648a3ba443b0.nq.gz
│   ├── c7520c8217137780b17f902a4071d532184ab423.nq.gz
│   └── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 9e2eab246532e6faa3037ebc0ffb433ea9eb2356.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 23 files
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

[django-commons/dj-database-url](https://github.com/django-commons/dj-database-url)

---
*Parsed on 2026-11-02 by [repolex](https://repolex.ai)*
