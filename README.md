<h1 align="center">Balakumar V</h1>

<p align="center">
  First-year B.E. Computer Science and Engineering student at Chennai Institute of Technology<br>
  Building practical, measurable software where AI meets engineering
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/balakumar-v-78b11b437"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:balakumarv1872008@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

## About

I work across full-stack development, retrieval-augmented generation (RAG), mathematical optimization, and statistical evaluation of ML systems. I like turning real problems into working, tested software, and I report assumptions and negative results alongside headline numbers.

Currently strengthening my software engineering and AI/ML foundations, and open to opportunities to learn, collaborate, and build.

---

## Featured Projects

### FarmRoute Optimizer
*Python · SciPy · FastAPI · PostgreSQL · React · TypeScript*

A decision system that pools small farmers onto shared trips, assigns a finite vehicle fleet, and splits produce across wholesale markets (mandis). It combines clustering, 2-opt routing, an LP for market allocation, and a set-partitioning MILP solved with HiGHS.

- Heuristic reaches **96.0%** of the exact MILP optimum on small instances
- On a Bihar scenario (real Agmarknet prices, 34 synthetic farmers), beats behavioural baselines by **42–54%** in farmer value under a stated 20% farm-gate price assumption; on the cold-chain scenario it only ties
- Nine scenarios: 3 synthetic, 6 on real mandi data from 5 states
- Admin console (React/TypeScript) and an installable farmer PWA in English, Hindi, Tamil, and Telugu with text-to-speech
- LLM-assisted change requests output structured JSON only, and each requires admin approval
- Allocation cache cut planning time 3–6x (60 farmers: 12.9 s to 2.8 s) with plans unchanged
- 280+ pytest tests plus Vitest, CI on GitHub Actions, deployed on Render and Neon

### Measured Feedback Tipping Points
*Python · NumPy · SciPy · scikit-learn · pandas*

A pre-rollout audit for ranking policies, built as team leader of 3 for the Perceptron Hackathon 2026 (Problem 3). It estimates repeat-exposure fatigue from a small randomized traffic slice, finds the tipping point κ\* where a new policy's lift reaches zero, and returns **APPROVE**, **REJECT**, or **NEED RANDOMIZED DATA**.

- One-step off-policy estimators (IPW, SNIPS, DM, DR) cannot see fatigue: in one simulated case the logs showed a **+0.084** click lift while the true 10-round lift was **−0.019**
- Thresholds fixed before each run. Final rule: **0 of 144** false approvals (95% upper bound 2.1%) and 26 of 48 correct approvals on fresh held-out simulator worlds
- Simulator-only, no production data. CLI, 288 seed-reproducible audits, and a unittest suite with exact-reproduction checks

### DocuQuery: RAG Document Q&A
*React · TypeScript · Node.js · PostgreSQL · pgvector*

A deployed full-stack app that answers questions about uploaded PDFs and cites the source passages.

- PostgreSQL with pgvector in place of a separate vector database
- Hybrid retrieval: vector similarity plus full-text search, merged with Reciprocal Rank Fusion
- Async PDF processing with batched embeddings, answers streamed over WebSockets
- JWT authentication, schema validation, and rate limiting
- Small eval (10–15 QA pairs): 93% answerable, 75% with correct citations
- Docker, Render, Vercel, GitHub Actions

---

## Research

### K-TRACE: Knowledge-Grounded Scene Prediction
*Vision-Language Models · Knowledge Graphs*

A research proposal asking whether retrieved knowledge-graph triples help a vision-language model reconstruct the past and predict the future of a scene, beyond what the image and a short description provide alone. From one anchor frame at time *t*, the model predicts the scene at *t − δ* and *t + δ*. Evaluation uses a KG-Gain metric against a context-only baseline, with a planned pilot of 500–1,000 anchors on egocentric video.

*Status: concept and proposal stage. No experiments have been run.*

---

## Tech Stack

| Area | Tools |
|---|---|
| **Languages** | Python, C, C++, JavaScript, TypeScript |
| **Frontend** | React, HTML, CSS, PWA, MapLibre GL, deck.gl |
| **Backend** | Node.js, Express.js, FastAPI, REST APIs |
| **Databases** | PostgreSQL, MySQL, SQLite, pgvector, Drizzle ORM |
| **AI / Optimization** | RAG, Embeddings, Hybrid Search, OpenRouter, SciPy (HiGHS), MILP, Off-Policy Evaluation |
| **Data / ML** | NumPy, pandas, scikit-learn, Matplotlib, Bootstrap and Statistical Testing |
| **Tools / Deployment** | Git, Docker, GitHub Actions, Render, Vercel, Neon, pytest, Vitest |

---

## Education

**B.E. Computer Science and Engineering** (2026 – 2030)
Chennai Institute of Technology, Chennai

---

<p align="center">
  <i>Open to learning, collaboration, and building useful things.</i>
</p>
