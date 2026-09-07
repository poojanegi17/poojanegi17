## Pooja Negi

I build real-time systems and machine learning projects — and I tend to build them
twice, because the second implementation is what tells you whether the first design
was right.

Two threads run through most of my work: **distributed state** — CRDTs, operational
transformation, offline sync — and **machine learning I can interrogate**, where the
interesting part is why the model decided what it decided.

<p align="center">
  <img src="https://raw.githubusercontent.com/poojanegi17/collab-docs/main/docs/media/lab-four-replicas.gif" width="720" alt="Four replicas of a collaborative editor under simulated latency: one is partitioned, diverges, and is healed">
</p>

<p align="center">
  <em>Four replicas. One gets partitioned, diverges, and heals — from the collab-docs concurrency lab.</em>
</p>

---

### Selected work

**[collab-docs](https://github.com/poojanegi17/collab-docs)** — *Distributed systems · CRDT vs OT*

A real-time collaborative editor built twice. One application, one transport, one
storage layer — and two interchangeable concurrency engines behind a single seam: a
CRDT (Yjs) and a server-authoritative OT implementing the three-state Jupiter machine.
The point isn't that it syncs; it's that you can swap the engine under a running
system and measure what changes.

Includes a concurrency lab that partitions replicas on demand, lets them diverge, and
heals them — plus offline persistence to IndexedDB, broadcast batching gated on
whether the engine declares its updates mergeable, and a decision record for every
trade-off. Every number in the README traces to the script that produced it.

**[Live demo](https://collab-client-kvn5.onrender.com/)** · `JavaScript` · `Yjs` · `WebSockets` · `PostgreSQL`

<p align="center">
  <img src="https://raw.githubusercontent.com/poojanegi17/collab-docs/main/docs/media/architecture.svg" width="680" alt="collab-docs architecture: editor, transport, engine seam and storage">
</p>

---

**[RL-Minesweeper-Lab](https://github.com/poojanegi17/RL-Minesweeper-Lab)** — *Reinforcement learning · benchmarking*

A benchmark platform for how different RL algorithms learn Minesweeper — a game that
is partially observable, sparse in reward, and genuinely unsolvable in some positions.
Interactive visualisations of what each agent learned, and performance analysis across
algorithms rather than a single leaderboard number.

**[Live demo](https://rl-minesweeper-lab.vercel.app)** · `TypeScript`

---

**[Tasker](https://github.com/poojanegi17/Tasker)** — *Full-stack · applied AI*

A task manager where the AI is a feature, not the product: it drafts task descriptions
from a title, and accepts tasks by voice. Appwrite backend, priorities, sorting,
search, dark mode.

**[Live demo](https://taskwrite.netlify.app/)** · `TypeScript`

---

### What I work with

**Systems** — JavaScript/TypeScript, Node, WebSockets, PostgreSQL, CRDTs and
operational transformation, offline-first sync

**ML** — Python, reinforcement learning, model explainability, Jupyter

Open to roles in distributed systems and applied ML · [LinkedIn](https://www.linkedin.com/in/pooja-negi-b45bab285) · poojaa.negi17@gmail.com 
