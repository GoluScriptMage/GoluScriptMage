```text
  ____  ___  _     _   _  //  ____  _______     __
 / ___|/ _ \| |   | | | |    |  _ \| ____\ \   / /
| |  _| | | | |   | | | |    | | | |  _|  \ \ / / 
| |_| | |_| | |___| |_| |    | |_| | |___  \ V /  
 \____|\___/|_____|\___/     |____/|_____|  \_/   
==================================================
```
> **Chitranshu (Golu) Dhakad** — Systems & Backend Engineer  
> *“Most developers treat the runtime, network, and OS as black boxes. I open the box, break it, and rebuild it from scratch.”*  
> 🌐 [golu.dev](https://golu.dev) • 💼 [LinkedIn](https://www.linkedin.com/in/chitranshu-dhakad-96a1753a1/) • 🐦 [X (@TheWebGolu)](https://twitter.com/TheWebGolu)

---

### 🏛️ The Full-Stack Systems Map

```text
┌──────────────┬─────────────────────────────────────────────────────────────┐
│ LAYER        │ SYSTEM MODULE & IMPLEMENTATION                              │
├──────────────┼─────────────────────────────────────────────────────────────┤
│ 5. Tooling   │ sync-cli      ──► AI AST documentation sync (Published/NPM)│
│ 4. Platform  │ AeroCloud     ──► Multi-tenant PaaS & Linux cgroups runtime │
│ 3. Streaming │ video-streamer──► Concurrency HLS & GOP-aligned transcoding │
│ 2. Storage   │ git-lite      ──► Content-addressable storage & Merkle trees│
│ 1. Network   │ proto-redis   ──► Raw TCP socket server & RESP state machine│
└──────────────┴─────────────────────────────────────────────────────────────┘
```

---

### 🛠️ The Modules

#### ☁️ `Layer 4` • [AeroCloud](https://github.com/GoluScriptMage/aerocloud) — Self-Hosted PaaS Engine
*A terminal-first cloud orchestrator executing zero-config container deployments.*
* **Container Sandboxing:** Hard Linux cgroups runtime enforcement (`512MB RAM` / `1 CPU core`) preventing host memory exhaustion.
* **Go Port Scanner:** Embedded $O(\log N)$ binary resolving machine-global ports via IPC pipes to eliminate race conditions.
* **Zero-Trust Auth:** Constant-time XOR token verification (`crypto.timingSafeEqual`) immune to timing side-channel attacks.

#### 🗄️ `Layer 1` • [proto-redis](https://github.com/GoluScriptMage/proto-redis) — TCP Key-Value Engine
*An in-memory database implementing Redis wire specifications over raw TCP sockets.*
* **RESP Protocol Parser:** Low-level state machine handling TCP packet fragmentation, streaming buffers, and command pipelining.
* **LRU Memory Eviction:** Hash-map index combined with doubly-linked list for $O(1)$ key eviction under memory pressure.

#### 🎥 `Layer 3` • [video-streamer](https://github.com/GoluScriptMage/video-streamer) — Adaptive HLS Pipeline
*A high-concurrency video delivery server with on-the-fly stream encryption.*
* **Deterministic Chunking:** Concurrent FFmpeg child pipelines enforcing GOP-aligned keyframes across multi-bitrate profiles.
* **In-Memory L2 Cache:** Sub-millisecond segment delivery bypassing filesystem reads.

#### 📦 `Layer 2` • [git-lite](https://github.com/GoluScriptMage/git-lite) — Version Control Core
*A Git-compatible version control engine written from binary specifications.*
* **Cryptographic Immutability:** Content-addressable object store (`blobs`, `trees`, `commits`) serializing directory graphs into Merkle trees.

#### ⚡ `Layer 5` • [sync-cli](https://github.com/GoluScriptMage/sync-cli) — Git-Diff Doc Engine `[NPM Package]`
*Developer tooling published on [NPM](https://www.npmjs.com/package/goluscriptmage-sync-cli) to automate architecture synchronization.*
* **AST & Diff Parsing:** Intercepts git staging events and AST tree diffs to reconcile codebase changes with active system architecture docs.

---

### 🔬 Core Toolchain & Invariants

```text
Languages      : Go, TypeScript, C (exploring low-level runtimes)
Infrastructure : Linux (cgroups, namespaces), Docker, Raw TCP/IP, Sockets
Data & State   : SQLite (WAL mode), Redis (RESP), PostgreSQL
Mental Model   : Benchmark everything. Zero closure heap escapes in Go. Memory-conscious by default.
```

---

### 📬 Connect
* Open to systems engineering, infrastructure, and high-performance backend roles.
* Portfolio: **[golu.dev](https://golu.dev)** | GitHub: **[@GoluScriptMage](https://github.com/GoluScriptMage)**
