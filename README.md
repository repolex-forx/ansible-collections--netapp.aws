# Repolex Knowledge Graph of ansible-collections/netapp.aws

RDF knowledge graph data for [ansible-collections/netapp.aws](https://github.com/ansible-collections/netapp.aws), parsed by [repolex](https://repolex.ai).

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
rlex download ansible-collections/netapp.aws
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 435befc587c333dec75afceec81c06924ee5f807
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 435befc587c333dec75afceec81c06924ee5f807
│           └── chunk-001.nq.gz
├── blob
│   ├── 09190b39e394b317ddc300f9e055e98925155f0c.nq.gz
│   ├── 0972cd2e8e58d51f20c6b0d23d8f89154c7ac076.nq.gz
│   ├── 11be8dbab51bcbee8be484a58d8fd8f15f022523.nq.gz
│   ├── 19ba55d8d75665773005b04fe29a93bd8ac4e9ce.nq.gz
│   ├── 26e822de7bc6d8a8b173635c8f8e7e7d5f081608.nq.gz
│   ├── 2767dba53bab42f6ce2c76dd1217450f69409c44.nq.gz
│   ├── 2c7e83f3137721c18cd4840161095a853200b5e9.nq.gz
│   ├── 315d71a13ac11b7e0753da3145332074a289e519.nq.gz
│   ├── 3e31ae98943df9355398cb26a4a158d9159fc44b.nq.gz
│   ├── 3f764c1c9f8f8c49e5979d76b4d448e1b8d56962.nq.gz
│   ├── 546ebfe7a23b08ef2004165106807568e999a9ce.nq.gz
│   ├── 5723daa110e595bb7320a95f25d55fe736559557.nq.gz
│   ├── 5f649c68c8d718d2ce49b9cf0393cdaf1ef792e1.nq.gz
│   ├── 663bd1f6a2ae02f29df59fb4963c17934034f731.nq.gz
│   ├── 6b4b660a0627a7e4d86ac70d8e522d86796d52f0.nq.gz
│   ├── 73a20cf8c240972154f2e3f34bbd7079373da0d3.nq.gz
│   ├── 86932068d2480de15e64be08d19b2b9b18492f09.nq.gz
│   ├── 94a9ed024d3859793618152ea559a168bbcbb5e2.nq.gz
│   ├── 98755b939b44e5fc8eeef8961cd04a5c0be79828.nq.gz
│   ├── aff60719f06c7b32cb7fe16247316e8904ad30b9.nq.gz
│   ├── b5a4bad84f34b6e94a2e1176c7459a435b2a232d.nq.gz
│   ├── b64c877b4867aa399a01f1c235fa8d8ec55bb2e6.nq.gz
│   ├── b754473a9959db13bde4c9a0077880918087784d.nq.gz
│   ├── ba907fcd52fc2564c906d702c4d1e14d949b7366.nq.gz
│   ├── bb825a2eebd2dd203fd46f6867bee7da4c7b994a.nq.gz
│   ├── c0506a059ec799e6f95b46b3872877ca53ffbbb2.nq.gz
│   ├── c7328c5eb84e63283ceb8df22f12c9d175c10ab7.nq.gz
│   ├── c92e9e41b65d1a7f45ed3c3a2a382192471d13d8.nq.gz
│   ├── d254e6081df9672773354975878856d9153fb50a.nq.gz
│   ├── d485eedc2f7df9ccf0049f8c601e153334cc9ea6.nq.gz
│   ├── d6fe89c96b7576b80edfc3a1dfda41f585cfd05f.nq.gz
│   ├── e59624ece49f1a9132bc0a19d9446c5f2390ecab.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ee4f8f481838c08f0ff9243997c61583d186d2ff.nq.gz
│   ├── f23b7e06e2d254c2157632d527340c7940c95025.nq.gz
│   ├── fa4818a3b4cce338170ee2a27a3ce3b07eaad04a.nq.gz
│   ├── fa5c5f87c30c21a0813fb52268112fba052863e6.nq.gz
│   └── fcd0d11ee39b6ad9b3cc14e4b26c64dda05cd18c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 435befc587c333dec75afceec81c06924ee5f807.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 46 files
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

[ansible-collections/netapp.aws](https://github.com/ansible-collections/netapp.aws)

---
*Parsed on 2026-11-07 by [repolex](https://repolex.ai)*
