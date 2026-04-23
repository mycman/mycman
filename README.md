<div align="center">

# Michael Thorpe · `mycman`

**IT Infrastructure Engineer** · **BS Information Technology** (Middle Georgia State University, April 2027)

Edge retrieval · agent memory · containerized services · autonomous-system governance

[![Email](https://img.shields.io/badge/email-mycman%40outlook.com-0078D4?style=flat-square&logo=microsoftoutlook&logoColor=white)](mailto:mycman@outlook.com)
![Location](https://img.shields.io/badge/based%20in-south%20georgia-555555?style=flat-square)
![Status](https://img.shields.io/badge/open%20to-remote%20%7C%20on--site-2e7d32?style=flat-square)

</div>

---

## What I'm building

**Production-grade retrieval infrastructure that fits in a single file.** I design and run self-hosted Linux services — SQLite-backed hybrid retrieval, vector+keyword fusion, containerized embedding workers, three-node Tailscale mesh, launchd/systemd supervision — with a focus on low-latency edge inference and operational simplicity. If Pinecone costs $70/month and adds 50 ms of network latency, I'm the engineer who replaces it with a `.sqlite` file and a shell script.

Current stack:

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Tailscale](https://img.shields.io/badge/Tailscale-242424?style=flat-square&logo=tailscale&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## Featured project

### 🔍 [`sqlite-vec-benchmark`](https://github.com/mycman/sqlite-vec-benchmark)

Hybrid retrieval benchmark: SQLite + `sqlite-vec` + FTS5 + Reciprocal Rank Fusion vs FAISS, Qdrant, Weaviate on BEIR SciFact. Real reproducible numbers, CI-published, single-file index.

| Backend | nDCG@10 | Recall@10 | p50 latency | Index size |
|---|---:|---:|---:|---:|
| sqlite-vec only | 0.721 | 0.840 | 1.05 ms | 9 MB |
| sqlite-fts5 only | 0.681 | 0.816 | 1.45 ms | 15 MB |
| **SQLite hybrid (RRF)** | **0.736** | **0.866** | 3.51 ms | 24 MB |

Thesis: agent memory and line-of-business retrieval are small-data problems. Vector DBs over-solve them. For workloads under ~1 M documents, a single SQLite file with `sqlite-vec` + FTS5 + RRF matches or beats managed services at 1/100th the cost and zero network round-trip.

### 📘 [`Tibero 7 vs Oracle 19c — reading notes`](https://gist.github.com/mycman/379ffff0c308bb04aee0ed8f7f6eebfb)

Developer-level comparison of TmaxSoft's Tibero (the Oracle-compatible RDBMS used by Hyundai Motor Group, Samsung, and the Korean public sector) against Oracle 19c. Covers SQL/PL/SQL compatibility, data type mapping edge cases, TAC vs RAC architecture, migration tooling (T-UP, Table Migrator, DB Link, tbLoader), Exadata-equivalent columnar compression, licensing model differences, and honest "where Oracle still wins" analysis.

---

## Focus areas

- **Retrieval systems** — hybrid vector + keyword ranking, reciprocal rank fusion, sub-10 ms latency budgets, edge deployment
- **Agent memory infrastructure** — MCP (Model Context Protocol) servers, persistent knowledge graphs, embedding pipeline migration (cutover without downtime)
- **Autonomous-system governance** — behavioral hooks, retry-storm detection, epistemic labeling, length/length-preamble discipline for LLM outputs
- **Linux fleet operations** — launchd, systemd, Tailscale mesh, Syncthing, durable write queues with replay semantics

---

## Background

Fifteen years of commercial operations leadership before pivoting full-time to infrastructure engineering. Deployed $75 K+ in capital to design and build production facilities from concrete to commissioning. Scaled teams and processes 4× in two months. Led organic certification audits. Trained operators across every phase of production.

That discipline — sourcing, process standardization, compliance, and owning outcomes — is what I'm applying to infrastructure work now.

---

## Currently

- Finishing BS Information Technology at MGSU (graduating April 2027)
- Publishing retrieval & infrastructure benchmarks that others can reproduce
- Open to full-time IT infrastructure roles — remote or Southeast US on-site

---

<div align="center">

**[📦 sqlite-vec-benchmark](https://github.com/mycman/sqlite-vec-benchmark)** · **[✉ mycman@outlook.com](mailto:mycman@outlook.com)**

*Infrastructure you can fit in a single file.*

</div>
