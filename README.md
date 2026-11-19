<img src="assets/hero-light.svg#gh-light-mode-only" width="100%" alt="Pushkar Kirange. Computer Engineering student, class of 2027. I fix bugs in open-source infrastructure and ship AI products end to end.">
<img src="assets/hero-dark.svg#gh-dark-mode-only" width="100%" alt="Pushkar Kirange. Computer Engineering student, class of 2027. I fix bugs in open-source infrastructure and ship AI products end to end.">

[Portfolio](https://pushkar-portfolio-mu.vercel.app) &nbsp;·&nbsp; [LinkedIn](https://linkedin.com/in/pushkar-kirange) &nbsp;·&nbsp; [LeetCode](https://leetcode.com/u/pushkarkirange/) &nbsp;·&nbsp; [pdkirange236@gmail.com](mailto:pdkirange236@gmail.com)

<br>

<img src="assets/open-source-light.svg#gh-light-mode-only" width="100%" alt="Open source. Bugs I fixed in libraries other teams depend on.">
<img src="assets/open-source-dark.svg#gh-dark-mode-only" width="100%" alt="Open source. Bugs I fixed in libraries other teams depend on.">

| Project | What was broken | What I changed | Pull request |
|:--|:--|:--|:--|
| **[platformatic/kafka](https://github.com/platformatic/kafka)**<br><sub>432 stars</sub> | A consumer stream died when partition leadership moved during a fetch retry: every retry hit another request's fetch session or the old leader. | A retry that no longer fits its node now returns empty, so the stream regroups the partitions by their current leaders. | <img src="assets/mark-merged.svg" width="10" alt="">&nbsp;[#502](https://github.com/platformatic/kafka/pull/502)<br><sub>merged, v2.17.0</sub> |
| **[testcontainers-node](https://github.com/testcontainers/testcontainers-node)**<br><sub>2.6k stars</sub> | The Dockerfile parser misread `FROM` lines with `--platform`, tabs, line continuations or `ARG` defaults. | Parsed all four the way Docker does, with fixtures for each case. | <img src="assets/mark-merged.svg" width="10" alt="">&nbsp;[#1646](https://github.com/testcontainers/testcontainers-node/pull/1646)<br><sub>merged</sub> |
| **[testcontainers-node](https://github.com/testcontainers/testcontainers-node)**<br><sub>2.6k stars</sub> | The `TestContainer` interface lacked five builder methods that `GenericContainer` has. | Added them, plus a type test that fails whenever the two drift apart. | <img src="assets/mark-merged.svg" width="10" alt="">&nbsp;[#1655](https://github.com/testcontainers/testcontainers-node/pull/1655)<br><sub>merged</sub> |
| **[prettier-eslint](https://github.com/prettier/prettier-eslint)**<br><sub>4.1k stars</sub> | `tabWidth` was inferred from the line length that `max-len` takes as its first argument. | Read `tabWidth` from the `max-len` options the way ESLint resolves them. | <img src="assets/mark-merged.svg" width="10" alt="">&nbsp;[#1227](https://github.com/prettier/prettier-eslint/pull/1227)<br><sub>merged, v17.1.3</sub> |

<img src="assets/mark-review.svg" width="10" alt=""> **In review**

- **[nats.js](https://github.com/nats-io/nats.js/pull/529)**: a slow `for await` loop over a JetStream consumer queued one extra pull per missed heartbeat, so `max_messages: 1` held many unacknowledged messages.
- **[http-proxy-3](https://github.com/sagemathinc/http-proxy-3/pull/75)**: the proxy left client connections open when the target died mid-response, so SSE clients (Vite's dev proxy) never reconnected.
- **[connect-es](https://github.com/connectrpc/connect-es/pull/1886)**: `universalResponseToNodeResponse()` never settled after the response finished.
- **[electron-builder](https://github.com/electron-userland/electron-builder/pull/10625)**: spawn output corrupted UTF-8 characters split across chunks.
- **[verdaccio](https://github.com/verdaccio/verdaccio/pull/6475)**: an S3 "already exists" conflict cut off concurrent tarball downloads.
- **[whatwg-node](https://github.com/ardatan/whatwg-node/pull/3806)**: `node-fetch` deviated from native fetch on form data, Blobs and `Request` init ([#3806](https://github.com/ardatan/whatwg-node/pull/3806), [#3807](https://github.com/ardatan/whatwg-node/pull/3807)).
- **[shiki](https://github.com/shikijs/shiki/pull/1352)**: ANSI highlighting garbled escape sequences that are not colour codes.

<br>

<img src="assets/products-light.svg#gh-light-mode-only" width="100%" alt="Products. Built and shipped end to end.">
<img src="assets/products-dark.svg#gh-dark-mode-only" width="100%" alt="Products. Built and shipped end to end.">

| Product | What it does | Built with | |
|:--|:--|:--|:--|
| **HireArena** | Assessment-first hiring for early-career software roles: AI prepares the assessment, recruiters approve it, candidates show their skills. | Next.js, Postgres, Better Auth, Anthropic API, Docker | [Live](https://hirearena-tan.vercel.app) |
| **Cert Bricks** | Company-led learning that turns practical proof into verified skills and hiring. | Next.js 16, Prisma 7, Postgres, Clerk | [Live](https://cert-bricks-platform.vercel.app) |
| **DiaGO** | Learn software design and draw UML, ER and architecture diagrams, in the browser and on Windows. | Next.js 16, Prisma 7, desktop app | [Live](https://diagoo.vercel.app) · [Desktop](https://diagoo.vercel.app/desktop) |
| **[SIGNAL](https://github.com/Pushkar236/signal)** | Earnings and filings intelligence: Whisper speech recognition, hybrid RAG and LangGraph agents, with eval-gated CI. | Python, LangGraph, Whisper | [Code](https://github.com/Pushkar236/signal) |
| **[Traffic incident system](https://github.com/Pushkar236/distributed-traffic-incident-system)** | Distributed real-time incident detection, coordination and response. | Python, gRPC, FastAPI, WebSocket, WebRTC, Docker | [Code](https://github.com/Pushkar236/distributed-traffic-incident-system) |
| **[CanteenGrid](https://github.com/Pushkar236/canteengrid)** | A distributed canteen order network: RPC, message queues, SSE streaming and peer-to-peer nodes. | Python, Flask | [Code](https://github.com/Pushkar236/canteengrid) |

Client and studio sites: [ISDIC](https://isdic-website.vercel.app) · [BBNA](https://bbna-swart.vercel.app) · [OnGo](https://ongo-mauve.vercel.app)

<br>

<img src="assets/toolkit-light.svg#gh-light-mode-only" width="100%" alt="Toolkit. What I build with.">
<img src="assets/toolkit-dark.svg#gh-dark-mode-only" width="100%" alt="Toolkit. What I build with.">

| | |
|:--|:--|
| **Languages** | TypeScript, JavaScript, Python, Java |
| **Web** | React, Next.js, Tailwind CSS |
| **Back end** | Node.js, Express, FastAPI, gRPC, Prisma |
| **Data** | PostgreSQL, MongoDB, MySQL |
| **AI** | Anthropic API, LangGraph, RAG, Whisper |
| **Tools** | Docker, Git, Linux, Framer, Photoshop |

<br>

<img src="assets/shipped-light.svg#gh-light-mode-only" width="100%" alt="Latest repos. Refreshed automatically every night.">
<img src="assets/shipped-dark.svg#gh-dark-mode-only" width="100%" alt="Latest repos. Refreshed automatically every night.">

<!-- ONGO:START -->
### 🚀 Featured Projects

| Project | Stack | Links |
| --- | --- | --- |
| **pushkar-portfolio** | TypeScript | [Live](https://pushkar-portfolio-mu.vercel.app) · [Code](https://github.com/Pushkar236/pushkar-portfolio) |
| **ongo** | TypeScript | [Live](https://ongo-mauve.vercel.app) · [Code](https://github.com/Pushkar236/ongo) |
| **diagoo-desktop-releases** | — | [Live](https://diagoo.vercel.app/desktop) · [Code](https://github.com/Pushkar236/diagoo-desktop-releases) |
| **Browse-History-Simulation** | CSS | [Code](https://github.com/Pushkar236/Browse-History-Simulation) |
| **canteengrid** | HTML | [Code](https://github.com/Pushkar236/canteengrid) |
| **JavaScript-Game-2048** | JavaScript | [Code](https://github.com/Pushkar236/JavaScript-Game-2048) |
| **whatsapp-chat-simulation** | CSS | [Code](https://github.com/Pushkar236/whatsapp-chat-simulation) |
| **pccoe-management-app** | JavaScript | [Code](https://github.com/Pushkar236/pccoe-management-app) |

<sub>↻ Auto-curated by <a href="https://ongo-mauve.vercel.app">OnGo</a> · updated 2026-11-18</sub>
<!-- ONGO:END -->
