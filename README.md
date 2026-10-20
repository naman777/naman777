<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=14&duration=2500&pause=900&color=7C9CFF&center=true&vCenter=true&width=520&height=24&lines=%2F%2F+AI+agents;%2F%2F+distributed+systems;%2F%2F+payments+%26+ledgers;%2F%2F+retrieval+%26+evals;%2F%2F+full-stack+products" alt="What I build" />

# Naman Kundra

### Full-Stack & AI Systems Engineer

Agents you can trust in production, distributed systems that survive failure,<br/>
and the products around them. ECE @ Thapar Institute.

<br/>

<a href="https://namankundra.com/"><img src="https://img.shields.io/badge/namankundra.com-7c9cff?style=for-the-badge&logoColor=0a0c10&labelColor=7c9cff&color=7c9cff" alt="Portfolio" /></a>
<a href="https://drive.google.com/file/d/1p73mr2s7kKy70XsQnDpmVaJ4XhlLY2Vz/view"><img src="https://img.shields.io/badge/Résumé-10131a?style=for-the-badge" alt="Résumé" /></a>
<a href="https://www.linkedin.com/in/naman-kundra-850209281/"><img src="https://img.shields.io/badge/LinkedIn-10131a?style=for-the-badge&logo=linkedin&logoColor=7c9cff" alt="LinkedIn" /></a>
<a href="mailto:naman@namankundra.com"><img src="https://img.shields.io/badge/naman@namankundra.com-10131a?style=for-the-badge&logo=maildotru&logoColor=7c9cff" alt="Email" /></a>
<a href="https://leetcode.com/u/naman_18byte/"><img src="https://img.shields.io/badge/LeetCode-10131a?style=for-the-badge&logo=leetcode&logoColor=7c9cff" alt="LeetCode" /></a>

</div>

<br/>

## `01` Selected work

<sub>Each one is deployed, and each one ships with its own benchmark or eval. Numbers come from the repo READMEs.</sub>

<table>
<tr>
<td width="50%" valign="top">

<a href="https://kosh.namankundra.com/"><img src="https://namankundra.com/projects/kosh.png" alt="Kosh" /></a>

<sub><code>PAYMENTS · DISTRIBUTED SYSTEMS</code></sub>

### Kosh

A payments core whose ledger stays balanced while you kill its processes. Double-entry ledger, idempotent payments, outbox webhooks, a simulated bank and UPI switch, and daily reconciliation.

**10,000** simulation seeds with crashes and bank faults, **0** invariant violations<br/>
**9×** capture throughput from sharding hot ledger accounts (p99 734 → 27 ms)<br/>
**~300** sales/s through the API, 0% errors

<sub>Go · PostgreSQL · Redpanda (Kafka) · Prometheus · Grafana · Next.js</sub>

[Code](https://github.com/naman777/kosh) · [Live](https://kosh.namankundra.com/)

</td>
<td width="50%" valign="top">

<a href="https://nightshift.namankundra.com/"><img src="https://namankundra.com/projects/nightshift.png" alt="Nightshift" /></a>

<sub><code>MULTI-AGENT AI · RELIABILITY</code></sub>

### Nightshift

An AI on-call engineer that survives its own crashes. A commander agent hands one question to each of four specialists, every claim cites evidence, and risky fixes wait for a human.

**96%** root-cause accuracy on held-out incidents<br/>
**0%** unsafe actions · **100%** claims grounded<br/>
**50** injected production failures in the benchmark

<sub>Python · Temporal · Multi-agent LLMs · Next.js · Loki</sub>

[Code](https://github.com/naman777/nightshift) · [Live](https://nightshift.namankundra.com/)

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://fathom.namankundra.com/"><img src="https://namankundra.com/projects/fathom.png" alt="Fathom" /></a>

<sub><code>RAG · AGENTS · EVALUATION</code></sub>

### Fathom

Chat with your documents, and see exactly where every answer came from. Hybrid search, an LLM reranker, a reflecting agent loop, and an eval harness so quality is measured.

**92%** answer accuracy on real docs (IETF RFCs), under 2% unsupported claims<br/>
**4×** multi-part full-hit with the agent loop<br/>
**92** golden questions in the eval harness

<sub>FastAPI · Postgres + pgvector · Next.js · SSE</sub>

[Code](https://github.com/naman777/Fathom) · [Live](https://fathom.namankundra.com/)

</td>
<td width="50%" valign="top">

<a href="https://foreman.namankundra.com/"><img src="https://namankundra.com/projects/foreman.png" alt="Foreman" /></a>

<sub><code>DISTRIBUTED SYSTEMS</code></sub>

### Foreman

A fault-tolerant distributed job scheduler you can try live. Redis-locked scheduling, heartbeat-tracked workers, and every job sandboxed in its own Docker container.

**2.4 s** median time to start a job in production<br/>
**5** guided failure scenarios, public<br/>
**41** automated tests in CI

<sub>TypeScript · Node.js · PostgreSQL · Redis · Docker</sub>

[Code](https://github.com/naman777/Foreman) · [Live](https://foreman.namankundra.com/)

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://meshpay.namankundra.com/"><img src="https://namankundra.com/projects/meshpay.jpg" alt="MeshPay" /></a>

<sub><code>DISTRIBUTED SYSTEMS · CRYPTOGRAPHY</code></sub>

### MeshPay

A payment mesh simulator where money settles exactly once, even offline. Signed, encrypted payments hop across offline devices and reach the internet through whichever bridge gets there first.

**1** settlement when 6 processes deliver the same payment at once<br/>
**4** failure modes it recovers from: loss, partition, delay, outage<br/>
**2** gossip rounds to reach both bridges

<sub>TypeScript · Next.js · PostgreSQL · SQLite · Ed25519</sub>

[Code](https://github.com/naman777/meshpay) · [Live](https://meshpay.namankundra.com/)

</td>
<td width="50%" valign="top">

<a href="https://load-balancer.namankundra.com/"><img src="https://namankundra.com/projects/load-balancer.png" alt="C++ Load Balancer" /></a>

<sub><code>SYSTEMS · NETWORKING</code></sub>

### C++ Load Balancer

An epoll TCP/HTTP load balancer in C++17 with no external libraries. Four algorithms, health checks, a live stats endpoint, and config reload on SIGHUP.

**33.9K** requests/s at 10K concurrent connections<br/>
**~31×** throughput vs. the thread-pool design with a slow backend<br/>
**2–6 MB** RSS at 10K connections

<sub>C++17 · Linux epoll · POSIX sockets · HTTP</sub>

[Code](https://github.com/naman777/Load-Balancer-CPP) · [Live](https://load-balancer.namankundra.com/)

</td>
</tr>
</table>

<table>
<tr>
<td valign="top">

<sub><code>ML FROM SCRATCH · OBSERVABILITY</code></sub>

### LogLens

A log-intelligence model, trained from scratch, that runs on a laptop CPU. It flags the incident window and returns the handful of lines that explain it, with zero LLM API calls.

**140×** fewer tokens for an on-call agent to read · **0.954** BGL anomaly F1 · **37.5 MB** int8 ONNX model

<sub>PyTorch · Transformers · ONNX Runtime · FastAPI</sub> · [Code](https://github.com/naman777/loglens)

</td>
</tr>
</table>

<br/>

## `02` More projects

| Project | What it does | Result |
|---|---|---|
| [**Operator**](https://github.com/naman777/operator) | Work-execution agent that drafts cited job applications and waits for approval before acting | 40-case regression suite, including prompt-injection cases |
| [**HirePrism**](https://github.com/naman777/HirePrism) · [live](https://hireprism-naman.streamlit.app) | Placement intelligence over 654 real campus offers, with a LangGraph agent on top | 305 tests · 93% coverage |
| [**LawVista**](https://github.com/naman777/LawVista) · [live](https://lawvista.namankundra.com/) | Legal research platform with RAG chat and case-outcome prediction | Built for the SIH 2024 finals |
| [**Examina**](https://github.com/naman777/Examina) · [live](https://exam-portal-next-js-eight.vercel.app) | Exam platform used for ACM Thapar recruitment | 10,000+ concurrent users · sub-200 ms responses |

<br/>

## `03` Experience

**Software Developer · [Oracia.ai](https://oracia.ai)** <sub>E-VNTS · Mar 2025 – Jul 2026</sub><br/>
AI real-estate platform. Built an agentic Autopilot with LangGraph that handled 35% of client conversations on WhatsApp by itself, cut manual work by 40%, and helped realtors close about 25% more deals a month.

**Software Developer · [GoVibe.live](https://govibe.live)** <sub>Macaron Ventures · Oct 2024 – Mar 2025</sub><br/>
Microservices social platform for 1,000+ users on Node.js, Kafka, Redis and Kubernetes. WebSockets and Kafka queues cut message delay from 2–3 s to 200–500 ms.

**Technical Executive · ACM TIET** <sub>Sep 2023 – Jan 2026</sub><br/>
Led Hacklipse 4.0, a national hackathon with 500+ participants and a ₹2L prize pool.

<br/>

## `04` Recognition

| | |
|---|---|
| **Smart India Hackathon 2024 Finalist** | Top 2.7% nationally: one of 1,300 finalist teams out of 49,000+ participants |
| **Merit-Based Scholarship** | CGPA 9.08 / 10, top 10% of the branch merit list at Thapar Institute |

<br/>

## `05` Stack

<div align="center">

<img src="https://img.shields.io/badge/Python-10131a?style=flat-square&logo=python&logoColor=7c9cff" alt="Python" />
<img src="https://img.shields.io/badge/TypeScript-10131a?style=flat-square&logo=typescript&logoColor=7c9cff" alt="TypeScript" />
<img src="https://img.shields.io/badge/Go-10131a?style=flat-square&logo=go&logoColor=7c9cff" alt="Go" />
<img src="https://img.shields.io/badge/C++17-10131a?style=flat-square&logo=cplusplus&logoColor=7c9cff" alt="C++17" />
<img src="https://img.shields.io/badge/Next.js-10131a?style=flat-square&logo=nextdotjs&logoColor=7c9cff" alt="Next.js" />
<img src="https://img.shields.io/badge/React-10131a?style=flat-square&logo=react&logoColor=7c9cff" alt="React" />
<img src="https://img.shields.io/badge/Node.js-10131a?style=flat-square&logo=nodedotjs&logoColor=7c9cff" alt="Node.js" />
<img src="https://img.shields.io/badge/FastAPI-10131a?style=flat-square&logo=fastapi&logoColor=7c9cff" alt="FastAPI" />
<br/>
<img src="https://img.shields.io/badge/PostgreSQL-10131a?style=flat-square&logo=postgresql&logoColor=7c9cff" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/pgvector-10131a?style=flat-square" alt="pgvector" />
<img src="https://img.shields.io/badge/Redis-10131a?style=flat-square&logo=redis&logoColor=7c9cff" alt="Redis" />
<img src="https://img.shields.io/badge/Kafka-10131a?style=flat-square&logo=apachekafka&logoColor=7c9cff" alt="Kafka" />
<img src="https://img.shields.io/badge/Temporal-10131a?style=flat-square&logo=temporal&logoColor=7c9cff" alt="Temporal" />
<img src="https://img.shields.io/badge/Docker-10131a?style=flat-square&logo=docker&logoColor=7c9cff" alt="Docker" />
<img src="https://img.shields.io/badge/Prometheus-10131a?style=flat-square&logo=prometheus&logoColor=7c9cff" alt="Prometheus" />
<img src="https://img.shields.io/badge/LangGraph-10131a?style=flat-square" alt="LangGraph" />
<img src="https://img.shields.io/badge/PyTorch-10131a?style=flat-square&logo=pytorch&logoColor=7c9cff" alt="PyTorch" />
<img src="https://img.shields.io/badge/ONNX-10131a?style=flat-square&logo=onnx&logoColor=7c9cff" alt="ONNX" />

</div>

<br/>

## `06` Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=naman777&show_icons=true&hide_border=true&include_all_commits=true&bg_color=0a0c10&title_color=7c9cff&icon_color=7c9cff&text_color=8b93a5&hide_title=true" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=naman777&layout=compact&hide_border=true&langs_count=8&bg_color=0a0c10&title_color=7c9cff&text_color=8b93a5" alt="Top languages" />

<img src="https://streak-stats.demolab.com?user=naman777&hide_border=true&background=0a0c10&ring=7c9cff&fire=7c9cff&currStreakNum=e8eaf0&sideNums=e8eaf0&currStreakLabel=7c9cff&sideLabels=8b93a5&dates=5b6376&stroke=1e2430" alt="GitHub streak" />

</div>

<br/>

<div align="center">

<sub>Live competitive-programming ratings and the full case studies are on the portfolio.</sub>

**[namankundra.com](https://namankundra.com/)** · [naman@namankundra.com](mailto:naman@namankundra.com) · [LinkedIn](https://www.linkedin.com/in/naman-kundra-850209281/)

</div>
