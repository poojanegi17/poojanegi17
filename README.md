
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

Five agents on one partially observable board — a CSP solver that *proves* cells safe,
tabular Q-learning, Double DQN, PPO, and random. Same environment, same encoding, same
2,000 evaluation boards, so what's being compared is the approaches rather than their
inputs.

Learning won: Double DQN reaches **77.25%** against the deduction solver's **70.35%**,
on disjoint confidence intervals. The more interesting result is that a lookup table
with no generalization whatsoever ties the solver too — which says more about the
benchmark than about the agent. Every game is replayable move by move with each agent's
own reasoning exposed: Q-values, action probabilities, the exact deductions the solver
made.

**[Live demo](https://rl-minesweeper-lab.vercel.app)** · `Python` · `PyTorch` · `Gymnasium` · `FastAPI` · `React`

<p align="center">
  <img src="https://raw.githubusercontent.com/poojanegi17/RL-Minesweeper-Lab/main/docs/media/race.gif" width="720" alt="Four agents take turns on one shared Minesweeper board: Random is eliminated on turn 5, DQN on turn 10, PPO on turn 11, and CSP clears the board on turn 14">
</p>

<p align="center">
  <em>Four agents, one shared board. Random, DQN and PPO are eliminated in turn; CSP clears it.</em>
</p>

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

**ML** — Python, PyTorch, reinforcement learning, model explainability

Open to roles in distributed systems and applied ML · [LinkedIn](https://www.linkedin.com/in/pooja-negi-b45bab285) · poojaa.negi17@gmail.com
