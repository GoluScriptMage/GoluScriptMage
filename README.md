<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,20&height=220&section=header&text=Yo,%20I'm%20Golu!%20👋&fontSize=50&fontAlignY=35&desc=Systems%20&%20Backend%20Engineer%20in%20Training%20|%20golu.dev&descAlignY=65&descSize=20&animation=fadeIn" width="100%" />
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=1000&color=36BCF7FF&center=true&vCenter=true&random=false&width=500&lines=Building+Raw+TCP+Servers...;Orchestrating+Docker+Networks...;Writing+Custom+VCS+Engines...;Becoming+Undeniable+🚀" alt="Typing SVG" />
</div>

---

<div align="center">
  <img src="https://count.getloli.com/get/@GoluScriptMage?theme=rule34" alt="Moe Counter" />
  
  <br/><br/>
  
  <a href="https://github.com/GoluScriptMage?tab=followers">
    <img src="https://img.shields.io/github/followers/GoluScriptMage?label=Followers&style=for-the-badge&color=2ecc71" alt="GitHub Followers" />
  </a>
  <img src="https://img.shields.io/github/stars/GoluScriptMage?label=Total%20Stars&style=for-the-badge&color=f1c40f" alt="GitHub Stars" />
</div>

---

## 👨💻 The Lore (About Me)

```text
┌────────────────────────────────────────────────────────┐
│  $ ssh golu@golu.dev                                   │
│  Connecting to backend core...                         │
│  [OK] TCP Sockets connected.                           │
│  [OK] RESP Parser initialized.                         │
│  [OK] Node.js Streams piping...                        │
│                                                        │
│  "Abstractions are cool, but raw network sockets       │
│   and byte streams make me feel alive."                │
└────────────────────────────────────────────────────────┘
```

I don't just write simple API wrappers; I build HTTP servers from scratch using raw `net` sockets, write my own Git engines to understand plumbing, and implement RESP parsers to check TCP stream fragmentation. I once crashed my own OS kernel trying to hold 1,000,000 concurrent TCP connections. It was worth it.

```text
$ show --affinity --interface
├── frontend/ (React, Next.js, TailwindCSS)
│   └── "Yes, I build clean client interfaces when needed..."
└── backend/ (Node.js, Express, Sockets, Databases)
    └── "...but this is where my heart beats and threads spawn." [HEART_STATUS: ACTIVE]
```

**Current Status:**
- 🔭 **Building:** A multi-tenant Webhook Relayer & Tunnel SaaS (custom TCP routing, dynamic Docker bridges).
- 🧠 **Grinding:** DSA (Linked Lists and Monotonic Stacks are falling one by one).
- ⚡ **Fun Fact:** I crashed my OS with 1M TCP connections.

> Check my daily progress logs here: [**Daily-logs Repo**](https://github.com/GoluScriptMage/Daily-logs)

---

## 🛠️ SYSTEM_DEPENDENCIES (THE ARSENAL)

```text
$ show --dependencies --verbose
├── runtime/
│   ├── typescript (v5.4)
│   └── javascript (ESNext)
├── backend/
│   ├── nodejs (LTS)
│   └── express
├── storage/
│   ├── postgresql
│   ├── redis (RESP parser)
│   └── mongodb
└── operations/
    ├── docker
    ├── linux
    └── git
```

<div align="center">

| **Core** | **Backend** | **Frontend** | **Database** | **Tools** |
| :---: | :---: | :---: | :---: | :---: |
| <img src="https://skillicons.dev/icons?i=ts,js" /> | <img src="https://skillicons.dev/icons?i=nodejs,express" /> | <img src="https://skillicons.dev/icons?i=react,nextjs,html,css,tailwind" /> | <img src="https://skillicons.dev/icons?i=postgres,redis,mongo,mysql" /> | <img src="https://skillicons.dev/icons?i=git,docker,linux,vscode,postman" /> |

</div>

<div align="center">
  <code>const Golu = { code: "Coffee", sleep: false, errors: "StackOverflow" };</code>
</div>

---

## 🚧 ACTIVE_MODULES (PROJECTS)

### 📂 [git-lite](https://github.com/GoluScriptMage/git-lite)
```text
+----------------------------------------------------------------------+
| TYPE: VCS Core Engine | LANG: TypeScript | PROTOCOL: Local FS        |
+----------------------------------------------------------------------+
```
*   **Description:** A custom Git-like version control engine built from scratch in TypeScript/Node.
*   **Key Features:** Generates Merkle trees to serialize project directories, compresses and stores objects securely in local db, and manages DAG history node traversals.
*   **Terminal Simulation:**
    ```bash
    $ git-lite commit -m "feat: ignore tracking changes"
    [index] hashing files...
    [tree]  created tree object: 7f89c02d1844b2a3c74900
    [status] write complete (0.002s). Repository synced.
    ```

### 📂 [proto-redis](https://github.com/GoluScriptMage/proto-redis)
```text
+----------------------------------------------------------------------+
| TYPE: RESP In-Memory Database | LANG: TypeScript | PROTOCOL: TCP/IP  |
+----------------------------------------------------------------------+
```
*   **Description:** An in-memory TCP socket cache database mimicking Redis server specifications.
*   **Key Features:** Implements a custom RESP parser to handle TCP stream fragmentation, manages command pipelining, and schedules key eviction using active TTL storage limits.
*   **Terminal Simulation:**
    ```text
    $ proto-redis --port 6379
    [INFO] Listening on TCP://127.0.0.1:6379...
    > PING
    < +PONG
    > SET db_status "STABLE_OVERLOAD"
    < +OK
    ```

### 📂 [video-streamer](https://github.com/GoluScriptMage/video-streamer)
```text
+----------------------------------------------------------------------+
| TYPE: JIT HLS Segmenter | LANG: TypeScript | PROTOCOL: HTTP/WebRTC   |
+----------------------------------------------------------------------+
```
*   **Description:** A high-performance media server that segments and streams video files dynamically on-the-fly.
*   **Key Features:** Uses promise-based deduplication to prevent cache stampedes, supports seek-safe GOP boundary alignment, and generates dynamic AES-128 segment encryption keys.
*   **Terminal Simulation:**
    ```text
    $ video-streamer --input test.mp4 --encrypt=aes128
    [stream] demuxing input video stream (H.264/AAC)...
    [segment] writing segment #0429 [██████████████░] 98%
    [stream] Active viewers: 142 | latency: 14ms (avg)
    ```

### 📂 [sync-cli](https://github.com/GoluScriptMage/sync-cli) (shadow-docs)
```text
+----------------------------------------------------------------------+
| TYPE: AI Documentation Sync | LANG: TypeScript | PROTOCOL: HTTPS API |
+----------------------------------------------------------------------+
```
*   **Description:** An AI-powered local documentation synchronizer CLI utility that watches git diff states.
*   **Key Features:** Tracks repository diff logs, integrates directly with the Google Gemini LLM API, and generates/appends codebase architecture changes to documentation files.
*   **Terminal Simulation:**
    ```text
    $ sync-cli sync --watch
    [watcher] git commit event detected
    [analyzer] building diff matrix...
    [gemini] generating update prompts...
    [sync] updated STRUCTURE.md successfully (0.84s).
    ```

### 📂 [nostalgia-playground](https://github.com/GoluScriptMage/nostalgia-playground)
```text
+----------------------------------------------------------------------+
| TYPE: Git History Monorepo | LANG: Git Subtree | PROTOCOL: Git Trees |
+----------------------------------------------------------------------+
```
*   **Description:** A consolidated historical repository preserving 9 early project milestones from 2023-2025.
*   **Key Features:** Merged using Git subtree commands to preserve 100% of the original commit timestamps and logs, providing a clean developer growth timeline.
*   **Terminal Simulation:**
    ```text
    $ cd nostalgia-playground && git log --no-merges
    commit a997f592842104c2c06307163ab2
    Author: GoluScriptMage
    Date:   Sun Dec 17 21:46:31 2023 +0530
        Initial commit: LoveCalculator
    ```

---

## 🏆 The Trophy Room

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=GoluScriptMage&theme=radical&no-frame=true&no-bg=true&margin-w=4" alt="GitHub Trophies" />
</div>

## 📊 The Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=GoluScriptMage&show_icons=true&theme=radical&hide_border=true&bg_color=00000000" height="170" />
  <img src="https://streak-stats.demolab.com/?user=GoluScriptMage&theme=radical&hide_border=true&background=00000000" height="170" />
</div>
<br/>
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=GoluScriptMage&layout=compact&theme=radical&hide_border=true&bg_color=00000000" />
</div>

---

<div align="center">
  <h3>Connect?</h3>
  <a href="https://linkedin.com/in/yourusername">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://twitter.com/yourusername">
    <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" />
  </a>
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer" width="100%" />
</div>
