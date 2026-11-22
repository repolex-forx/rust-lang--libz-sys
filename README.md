# Repolex Knowledge Graph of rust-lang/libz-sys

RDF knowledge graph data for [rust-lang/libz-sys](https://github.com/rust-lang/libz-sys), parsed by [repolex](https://repolex.ai).

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
rlex download rust-lang/libz-sys
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c589ac52bdf9f735dfc2858487e9b1f33b40c5cd
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── c589ac52bdf9f735dfc2858487e9b1f33b40c5cd.nq.gz
│   └── repolex
│       └── c589ac52bdf9f735dfc2858487e9b1f33b40c5cd
│           └── chunk-001.nq.gz
├── blob
│   ├── 16e58248714763f59b42817231312d15ca42985b.nq.gz
│   ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
│   ├── 213dbf618c4bda73358a0b26b69bea48a0f19740.nq.gz
│   ├── 3f4f0b9252c1133bbcf819a80010ff7280bf492a.nq.gz
│   ├── 44a935b21f7e10aa53498dd4cfb0fdde910d71f7.nq.gz
│   ├── 4ad13ebe699c307d1b2076e4daddd64eacb13f68.nq.gz
│   ├── 55a2ddf978f39039b3e4e6b6d5bd984661043004.nq.gz
│   ├── 5ddcbaf4c7286b562d6c7e7ea3acdf5b2a3ff3f9.nq.gz
│   ├── 614bf946d63f8eda135a4fe779a247fac026c3a5.nq.gz
│   ├── 6cdad14c56b64471be52d07cd1f15f03d77f0be7.nq.gz
│   ├── 73a0847d558a1b9c562eb5cb23955947b1b5b3aa.nq.gz
│   ├── 7d4bd67fb914b7caad08513313e021ff1847dd71.nq.gz
│   ├── 87cd9d98cbc039c0d370854fd47dc391aaa0e638.nq.gz
│   ├── 960ff42342aa541e967e334da1b5e04167d309cc.nq.gz
│   ├── 981b43ca0d452ddfd2483094f75a89ed43d13c1c.nq.gz
│   ├── a69f1c9a8a087744c1856c4cf1b737e93837e239.nq.gz
│   ├── a6d547fefe8c350566f37246a7199c3e6476a39f.nq.gz
│   ├── a7cebb22539f8f10989523ff2cba3e754f08730a.nq.gz
│   ├── a9d37c560c6ab8d4afbf47eda643e8c42e857716.nq.gz
│   ├── ae00583fcbf2aba5f25eadfe9d77b72f9d288bbb.nq.gz
│   ├── bb5a3d9089f168b0138179e9747d2177ff096019.nq.gz
│   ├── d3996691a95ec02ed25bfb920a4d1bf3be6e7efe.nq.gz
│   ├── d822cd56f8b53a3b74590fbf19563ec10e6c6f9f.nq.gz
│   ├── de1d77041c13660ac9beb3e8cd196fae4c0a65ba.nq.gz
│   ├── ed40f58cff7dc4be6bfa3b8debe9505687f5160e.nq.gz
│   ├── f659aa77c4572b5ccfd17e935887b661a3cecb5e.nq.gz
│   └── f7f4d3b71d3a176496cd7920f5190b6f76545351.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── c589ac52bdf9f735dfc2858487e9b1f33b40c5cd.nq.gz
├── filetree
│   └── c589ac52bdf9f735dfc2858487e9b1f33b40c5cd.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 37 files
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

[rust-lang/libz-sys](https://github.com/rust-lang/libz-sys)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
