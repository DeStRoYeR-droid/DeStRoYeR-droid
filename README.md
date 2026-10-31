<div align="center">

# Immanuel Vivek Tirkey

**Final-year MCA @ NIT Warangal**  

Building evaluation pipelines for LLMs · Writing C++ that has to be fast · Playing basketball otherwise 🏀 

<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/immanuel-vivek-tirkey/) [![LeetCode](https://img.shields.io/badge/LeetCode%20Guardian%20%C2%B7%202221-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/immanuelvivek40609/) [![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:immanuelvivek40609@gmail.com) [![Resume](https://img.shields.io/badge/R%C3%A9sum%C3%A9-2F855A?style=for-the-badge&logo=readdotcv&logoColor=white)](https://github.com/DeStRoYeR-droid)

</div>

---
## 🔭 Featured projects

- **[Chess Analysis and Learning Tool](https://github.com/DeStRoYeR-droid/Chess-Analysis-and-Learning-Tool)**: benchmarks LLM chess commentary against Stockfish and human annotations (Python, PyTorch, FastAPI, llama.cpp)
- **[Nebula Atlas](https://github.com/DeStRoYeR-droid/nebula-atlas)** · [live demo](https://destroyer-droid.github.io/nebula-atlas/): interactive nebula gallery with a sliding-puzzle view (React, Tailwind, Motion, FastAPI, GitHub Pages)

---
 
## 🔨 What I've built
 
### [Chess Analysis and Learning Tool (CALT)](https://github.com/DeStRoYeR-droid/Chess-Analysis-and-Learning-Tool)  ·  `MIT License`
 
A research pipeline that asks a hard question: **when an LLM explains a chess position, is it actually right — and is "right" even the same thing as "instructive"?**
 
- Benchmarks LLM-generated commentary against **Stockfish ground truth** and **blind human annotation** across the 300-position Win-at-Chess set, scored on a four-axis compound metric
- Retrieval subsystem pairing **bitboard tactical-motif detection** with **Zobrist-anchored semantic lookup**, so commentary is grounded in verified patterns instead of free generation
- **FastAPI + SSE streaming** over a multi-process engine pool; Gemma and Qwen served locally via `llama.cpp` against a shared cache to isolate model quality from engine variance
<sub>`Python` · `PyTorch` · `FastAPI` · `llama.cpp` · `Stockfish` · `SSE`</sub>
 
### [LandChain: Land Records on a Permissioned Blockchain](https://github.com/DeStRoYeR-droid/land-records-blockchain)
 
A land registry shared by three government departments (Registration, Revenue, Collectorate) — with the ledger **built from scratch** rather than imported.
 
- **Permissioned ledger in plain Python, following Hyperledger Fabric's design:** certificate authorities, 3 Raft orderers, 3 endorsing peers, execute-order-validate with MVCC, and an `AND(Org1, Org2, Org3)` endorsement policy
- Citizens sign sales with **browser-held `did:key` identities**; every transfer record and validator report is **PGP-signed** and verifiable in the browser or with `gpg --verify`
- **LangGraph AI validator** on a local Qwen2.5-3B model: 15 fixed checks, then tool-cited investigation with grounding and hallucination screening — it can flag, never approve or edit
- Map-based public register on an **R\*Tree-indexed GeoPackage** (search by text, area, map window or distance); Next.js dashboards for officials, citizens and the validator; 76 unit tests + 200+ end-to-end checks
<sub>`Python` · `Next.js` · `React` · `LangGraph` · `OpenPGP` · `SQLite` · `GeoPackage`</sub>
 
### [Trust-Based Secure Routing for Wireless Sensor Networks](https://github.com/DeStRoYeR-droid/trust-routing-wsn)  ·  `C++17`
 
Packet-dropping attackers hide inside multi-hop sensor networks because plain routing can't tell a relay that forwards from one that silently drops.
 
- Trust-aware routing layer on **NS-3**: watchdog overhearing + end-to-end ACKs feed per-node trust; Dijkstra routes around low-trust relays
- Raises packet delivery under blackhole attacks from **19% to 94%**, with **zero honest nodes flagged** across 130 paired runs
- Traced a **1.5 GB-per-run memory blow-up** to the simulator's energy model with Valgrind massif; replaced it with an equivalent model (within 0.01%), cutting memory **50×**
- Tests at four layers (C++, Python, JS, browser end-to-end) and an Obsidian-style **D3 viewer** that replays attackers being caught
<sub>`C++17` · `NS-3` · `Python` · `D3.js` · `Valgrind`</sub>
 
### [Agentic AI Defence for Medical IoT](https://github.com/DeStRoYeR-droid/agentic-iomt-defense)
 
A simulated hospital network where ECG traffic passes a man-in-the-middle relay before reaching an AI defender.
 
- **Per-packet fast path:** rules, LightGBM, Isolation Forest, autoencoders and CUSUM fused into one risk score that picks among forward, flag, hold, block, quarantine or escalate
- **Supervisory LLM agent** (local Qwen2.5-3B) retunes the defence every 2 s — only through whitelisted, bounded changes, each replay-verified and rolled back if it doesn't help
- FastAPI + React live dashboard; Docker setup; covers reconnaissance, spoofing, exfiltration and command-injection traffic
<sub>`Python` · `LightGBM` · `PyTorch` · `FastAPI` · `React` · `Docker`</sub>
 
### Smaller builds
 
- **[Error-Correcting Codes](https://github.com/DeStRoYeR-droid/Error-Correcting-Codes)** (C++17): Hamming codes with syndrome correction and CRC via polynomial division, from scratch, validated against injected bit flips
- **[Connect Four](https://github.com/DeStRoYeR-droid/Connect-Four-Pygame)** (Python): minimax with alpha-beta pruning
- **[Nebula Atlas](https://github.com/DeStRoYeR-droid/nebula-atlas)** · [live demo](https://destroyer-droid.github.io/nebula-atlas/): interactive nebula gallery with a sliding-puzzle view (React, Tailwind, Motion)

---

## 🧰 Stack

<div align="center">

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

</div>

---

## By the numbers

<div align="center"> <img height="180" src="https://leetcard.jacoblin.cool/immanuelvivek40609?theme=light&font=Poppins&ext=heatmap" alt="LeetCode stats" />

<br><br>

> **1,300** in C++ · **500+ day** streak · top **1%** of rated contestants.

---

## ✍️ Writing

Six published technical articles for **[LinuxForDevices](https://www.linuxfordevices.com/author/immanuel)** on the Rust toolchain, Pyright static type checking, and Linux desktop tooling — written for developers who want the _why_, not just the command.

---

## 🎯 Currently

Final year of my MCA at NIT Warangal, graduating **2027**. Deep in LLM evaluation, distributed systems, security, and competitive programming.
 
**Open to full-time SDE, ML engineering, and AI research roles for the 2027 batch.** If you're hiring or just want to discuss about basketball (certified ball 🏀 knower here) — [reach out](mailto:immanuelvivek40609@gmail.com).

<div align="center"> <br>

![Github stats](https://github-stats-extended.vercel.app/api?username=destroyer-droid)

</div>
