# Hi, I'm Kirill 👋 | Web3 Research & Infrastructure Engineer

Smart contract developer and Web3 stress-testing research engineer. Focused on Decentralized Physical Infrastructure (DePIN), Data Availability (DA) throughput limits, custom ERC standards, and automated load profiling.

---

## 📊 0G Labs DA Infrastructure Benchmarks (Controlled R&D)

*All architecture was deployed, evaluated, and validated within the official **0G Galileo Testnet** environment.*

* 🛠️ **[0g-da-phase3-kessler-benchmark](https://github.com/kirilks2026-maker/0g-da-phase3-kessler-benchmark)** — **Fixed-Mass Saturation Marathon**
  * **Approach:** Flooded the 0G DA storage layer using a fixed chunk size of **350 MB** per node insertion, bypassing EVM execution gas (`--skip-tx`). Load scaling was driven progressively via cumulative epoch multipliers (`epoch * 10`).
  * **Circuit Breaker Integration:** Implemented a programmatic stop-loss mechanism. When network node discovery/ingestion queue degradation triggered a **Drop Rate > 30%**, the script executed an emergency exit to prevent unmonitored validator socket starvation.

* 📈 **[0g-da-phase4-adaptive-profiler](https://github.com/kirilks2026-maker/0g-da-phase4-adaptive-profiler)** — **Dynamic Load Profiler**
  * **Approach:** Shifted from fixed sizing to a step-up variable load array. The system incrementally scales data chunks from **50 MB up to 500 MB** (in 50 MB steps) with controlled asynchronous spacing (`sleep(300)`).
  * **Outcome:** Successfully mapped out the automated `failure_threshold_chunk_mb` metric. Demonstrates how an adaptive telemetry architecture assesses network stability boundaries without introducing catastrophic overhead.

---

## 🛠️ Advanced Stress-Testing Frameworks

* ⚡ **[litvm-orbital-stress-profiler](https://github.com/kirilks2026-maker/litvm-orbital-stress-profiler)** — High-concurrency throughput testing and latency profiling framework optimized for **Lit VM** nodes.
* 🛰️ **[omcp-da-stress-framework](https://github.com/kirilks2026-maker/omcp-da-stress-framework)** & **[omcp-da-stress-framework-Phase-2](https://github.com/kirilks2026-maker/omcp-da-stress-framework-Phase-2)** — Multi-phase stress framework simulating real-world node congestion and telemetry metrics under burst loads across alternative Data Availability layers.

---

## 📜 Smart Contracts & Web3 Protocols

* 🌉 **[oimpact-erc8004-bridge](https://github.com/kirilks2026-maker/oimpact-erc8004-bridge)** — On-chain / off-chain bridge implementation leveraging AI-agent execution standards (ERC-8004) and cross-chain message passing. Features the custom `GroundRadarStressTester.sol` telemetry engine.
* 🚀 **[want-to-mars](https://github.com/kirilks2026-maker/want-to-mars)** — Core smart contracts, business logic, and infrastructure deployment files for the "Want to Mars" decentralized system.
* ⚙️ **[web3-smart-contracts](https://github.com/kirilks2026-maker/web3-smart-contracts)** & **[my-smart-contracts](https://github.com/kirilks2026-maker/my-smart-contracts)** — Specialized Solidity development workspace featuring "Gold of Germany" & "Manhattan" logistics and yield distribution models for Simple Chain.

---

## 💻 Tech Stack & Tooling

* **Languages & Smart Contracts:** Solidity, JavaScript / Node.js, Shell, Web3.js / Ethers.js
* **Infrastructure & Testing:** GitHub Codespaces, 0G Storage CLI, Lit Protocol, Custom Circuit Breakers & Benchmarkers

---

## 🎯 Mainnet Integration Goal

The developed ERC-8004 Circuit Breaker infrastructure is engineered as a **Public Good** (MIT Licensed) for the Web3 validation ecosystem.

**Our Objective:** We are requesting **0G Mainnet storage provisioning and dedicated execution slots** from the 0G Foundation/DevRel team to deploy our autonomous ERC-8004 guardian agent live on production infrastructure.

* **Discord ID:** `kiril_54116` (ID: `1490088551021412363`)
* **Associated Email:** `kirilks2026@gmail.com`
