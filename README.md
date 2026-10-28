# Hi, I'm Amenah Saleh 

**Systems engineer focused on database engines, storage systems, compilers, interpreters and static analysis. Rust and Go.**

I like the layer below the application: storage engines, consensus, crash recovery, language implementations, and the invariants that keep programs and data correct. Every project here is built from first principles, without wrapping an existing engine, and tested against the failure modes it claims to handle (crashes, partitions, torn writes).

![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![C](https://img.shields.io/badge/C%20%2F%20eBPF-A8B9CC?style=flat&logo=c&logoColor=black)
![gRPC](https://img.shields.io/badge/gRPC-244c5a?style=flat&logo=grpc&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

---

## Storage engines (Rust)

| Project | What it is |
|---|---|
| [**lsmdb**](https://github.com/monaaoua9/lsmdb) | LSM-tree engine: WAL, skiplist memtable, mmap SSTables, leveled compaction, MVCC |
| [**pagedb**](https://github.com/monaaoua9/pagedb) | Page-based engine: buffer pool, on-disk B+ tree, ARIES-style WAL recovery, 2PL transactions |
| [**hiis**](https://github.com/monaaoua9/hiis) | Full-text search engine in safe Rust: BM25, positional index, FoR/VByte compression, immutable segments with background merging, WAND |
| [**vecdb**](https://github.com/monaaoua9/vecdb) | Embedded vector database: HNSW, SIMD kernels (AVX-512 / AVX2 / NEON), SQ8 quantization, mmap snapshots, gRPC |
| [**columnar-tsdb**](https://github.com/monaaoua9/columnar-tsdb) | Columnar time-series store: Gorilla compression, immutable chunks, WAL, background compaction |
| [**cas-engine**](https://github.com/monaaoua9/cas-engine) | Content-addressed dedup object store: Rabin chunking, BLAKE3, Merkle proofs, crash-safe GC |

## Distributed systems (Go)

| Project | What it is |
|---|---|
| [**kvcoord**](https://github.com/monaaoua9/kvcoord) | Strongly consistent KV and coordination store: Raft, WAL, leases, locks, watches, linearizability-checked |
| [**dtask**](https://github.com/monaaoua9/dtask) | Distributed task scheduler: from-scratch Raft, fencing tokens, phi-accrual failure detection, chaos tests |
| [**objstore**](https://github.com/monaaoua9/objstore) | Fault-tolerant object storage: Reed-Solomon erasure coding, Raft metadata, S3 API |
| [**streamdb**](https://github.com/monaaoua9/streamdb) | Stream processing engine: event-time windows, backpressure, Chandy-Lamport checkpoints, exactly-once, automatic recovery |
| [**edgemesh**](https://github.com/monaaoua9/edgemesh) | Edge IoT gateway: MQTT + gRPC, WAL store-and-forward, anomaly detection, fleet management |
| [**xdpshield**](https://github.com/monaaoua9/xdpshield) | XDP load balancer / DDoS filter: Maglev and WRR in-kernel, Go control plane, Prometheus metrics |

---

## What I work on

- **Compilers, interpreters and static analysis**: parsing, IRs, program analysis, tooling that reasons about code
- **Durability and recovery**: write-ahead logging, crash-safe compaction and GC, ARIES-style redo/undo
- **Consensus and coordination**: Raft, leases with fencing tokens, failure detection, linearizability checking
- **Performance**: mmap I/O, SIMD, compression (Gorilla, FoR, VByte), lock-free and cache-aware structures
- **Correctness under failure**: chaos tests, fault injection, invariant checks

## Tech

**Languages:** Rust · Go · C · C++ · Shell
**Systems:** parsers · IRs · static analysis · Raft · LSM trees · B+ trees · MVCC · WAL · HNSW · XDP/eBPF · erasure coding
**Tooling:** gRPC · Prometheus · Docker · Make

---

## Open to

Database-engine, compiler/language-tooling, and infrastructure roles where systems depth matters.

📫 monaaoua9@gmail.com

