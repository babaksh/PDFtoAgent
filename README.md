# 📘 PDFtoAgent 🤖

> **Turn domain literature into executable AI Agents with deterministic Python tools served over MCP — available as a Zero-Docker Windows Portable package & Docker container.**

[![Portable Windows](https://img.shields.io/badge/Windows%20Portable-Zero--Docker%20.zip-brightgreen?logo=windows)](https://github.com/babaksh/PDFtoAgent/raw/main/dist/PDFtoAgent-Portable-stock-market-barometer-hamilton.zip)
[![Docker Hub](https://img.shields.io/badge/Docker%20Hub-babak60-blue?logo=docker)](https://hub.docker.com/u/babak60)
[![Protocol](https://img.shields.io/badge/MCP-Streamable--HTTP-purple)](https://modelcontextprotocol.io)
[![Python](https://img.shields.io/badge/Python-3.12-brightgreen?logo=python)](https://python.org)
[![Author](https://img.shields.io/badge/Maintained%20by-Babak-black?logo=github)](https://github.com/babaksh)
[![Security Scan](https://github.com/babaksh/PDFtoAgent/actions/workflows/security-scan.yml/badge.svg)](https://github.com/babaksh/PDFtoAgent/actions/workflows/security-scan.yml)
[![HOL Guard](https://img.shields.io/endpoint?url=https%3A%2F%2Fhol.org%2Fapi%2Fregistry%2Fbadges%2Fplugin%3Fslug%3Dbabaksh%252Fpdftoagent%26metric%3Dtrust)](https://hol.org/registry/plugins/babaksh%2Fpdftoagent)
[![Zero-Trust](https://img.shields.io/badge/Verification-Zero--Trust%20Docker%20Sandbox-success)]()
[![License](https://img.shields.io/badge/License-Community%20(Non--Commercial)-blue)](LICENSE)
[![Showcase](https://img.shields.io/badge/Showcase-Public%20Domain%20(1922)-orange)]()

---

<p align="center">
  <a href="https://www.youtube.com/watch?v=5ytxQepI5mY" target="_blank">
    <img src="assets/pdftoagent-thumbnail.png" alt="PDFtoAgent Video Walkthrough" width="100%">
  </a>
  <br>
  <sub>🎬 <b>Watch Video Walkthrough (1m 24s):</b> Click the image above to play on YouTube</sub>
</p>

---

## 💡 The Paradigm Shift: Why Plain RAG Fails

Traditional **Retrieval-Augmented Generation (RAG)** turns books into static text chunks. When you ask an ordinary RAG system to evaluate mathematical rules or multi-step algorithmic strategies, it resorts to **probabilistic token guessing**—frequently hallucinating calculations, miscalculating percentages, and failing to execute rigorous domain procedures.

**PDFtoAgent** solves this by transforming technical literature into a cohesive **Triad-Architecture MCP Server (RAG + Domain Skill + Deterministic Tools)**:

1. 📚 **Chapter-Level Vector RAG:** Semantic search with page citations, tables, and book figures/charts.
2. 🧠 **Codified Domain Skill (`SKILL.md`):** Procedural guidelines, decision trees, and expert system instructions.
3. ⚙️ **Deterministic Python Tools:** Verified executable algorithms running in sandboxes with zero math hallucinations.

```
┌────────────────────────────────────────────────────────────────────────┐
│                      ORDINARY RAG vs PDFTOAGENT                        │
├────────────────────────────────────────────────────────────────────────┤
│        Traditional RAG               PDFtoAgent Unified MCP Agent      │
│        (Text Chunks Only)            (Vector RAG + Skill + Tools)      │
├────────────────────────────────────────────────────────────────────────┤
│ ❌ Probabilistic word guessing ✅ Deterministic Python code execution │
│ ❌ Frequent calculation errors ✅ Exact mathematical computation      │
│ ❌ No procedural guidance      ✅ Codified Domain Skill (SKILL.md)    │
│ ❌ Blind trust in model output ✅ Zero-trust Docker sandbox gate      │
│ ❌ Context window overflows    ✅ Progressive Disclosure Tool Router  │
│ ❌ Opaque, unverified answers  ✅ Exact chapter & page provenance     │
└────────────────────────────────────────────────────────────────────────┘
```

---

## 🏛️ The Engine: 4-Tier Zero-Trust Architecture

PDFtoAgent employs a multi-tier verification pipeline to ensure every synthesized tool is mathematically sound, resilient to edge cases, and strictly grounded in the source book:

```
                  Domain PDF (e.g., 1922 Dow Theory)
                                  │
    ┌─────────────────────────────▼─────────────────────────────┐
    │  PHASE 1: Ingestion & Knowledge Extraction                │
    │  Clean Markdown + Multimodal Figures + Page Citations     │
    └─────────────────────────────┬─────────────────────────────┘
                                  ▼
    ┌───────────────────────────────────────────────────────────┐
    │  PHASE 2: Agentic Tool Synthesis (The 4-Tier Gate)        │
    │  ├─ Tier-1: Planner & Value Gate (Quoted Evidence Proof)  │
    │  ├─ Tier-2: Writer & Docker Sandbox (Live Execution)      │
    │  ├─ Tier-2.5: Adversarial Robustness Gate (Zero tokens)   │
    │  ├─ Tier-3: Independent LLM Judge (Fidelity vs Source)    │
    │  └─ Tier-4: Redundancy & Granular Provenance Audit        │
    └─────────────────────────────┬─────────────────────────────┘
                                  ▼
    ┌───────────────────────────────────────────────────────────┐
    │  PHASE 3: Packaging & Progressive Disclosure MCP Router   │
    │  SKILL.md + Exact Vector Store + 100+ Python Tools        │
    └─────────────────────────────┬─────────────────────────────┘
                                  ▼
        Dual Distribution: Portable Windows Zip (.bat) & Docker
```

---

## 📊 Pre-Built Showcase: William Peter Hamilton (1922 Dow Theory)

To demonstrate this architecture, I compiled William Peter Hamilton's 1922 classic, **"The Stock Market Barometer"** (the foundational text of Dow Theory, now in the Public Domain), into a production-ready MCP Agent.

The delivered package is a turnkey, multi-component showcase:

* 📚 **Full-Book Chapter-by-Chapter Vector RAG:** Comprehensive semantic search across all 24 chapters with exact page-level citations (`sqlite-vec` + local embeddings).
* 🧠 **Specialized Dow Theory Domain Skill (`SKILL.md`):** Deep codified market philosophy, rule interpretation protocols, and procedural decision trees directly distilled from Hamilton's work.
* ⚙️ **100+ Quantitative Trading Tools:** Verified, deterministic Python calculations including double top/bottom detectors, 3/8ths retracement rules, primary/secondary trend classifiers, line formation breakout tests, and speculative volume balance metrics.
* 🎛️ **Progressive Disclosure Router:** Exposes only 3 lightweight router meta-tools (`search_tools`, `get_tool`, `run_tool`) so the LLM context window never gets overloaded regardless of tool count.
* ⚖️ **Public Domain Compliance:** 100% legal, non-infringing, and open for global use under 17 U.S.C. § 105/304.

---

## 🚀 Delivery & Execution Guide

Follow these simple steps to run the **Hamilton Dow-Theory MCP Server** on your local machine and connect it to **your favorite Agentic Apps** (Claude Desktop, ChatGPT, Antigravity, OpenClaw, Cursor, etc.).

Choose the execution method that best fits your environment:

| Execution Method | Target Platform | Prerequisites | Setup Effort |
| :--- | :--- | :--- | :--- |
| **[⚡ Method 1: Standalone Portable Bundle](#-method-1-standalone-portable-bundle-recommended-for-windows)** | **Windows (10 / 11)** | Ollama (only for RAG embeddings; auto-handled by script) | 🟢 **1-Click Launch (`run_server.bat`)** |
| **[🐳 Method 2: Docker Container Image](#-method-2-docker-container-image-cross-platform)** | **macOS / Linux / Windows** | Docker Desktop & Ollama (only for RAG embeddings) | 🟢 **Standard Container Run** |

---

### ⚡ Method 1: Standalone Portable Bundle (Recommended for Windows)

The **Portable Distribution** is a ComfyUI-style, fully self-contained package created by [Babak](https://github.com/babaksh). It runs 100% locally on Windows **without requiring Docker Desktop, WSL2, or a system Python installation**.

```
┌────────────────────────┐       ┌────────────────────────┐       ┌────────────────────────┐
│  Step 1: Download .zip │ ───>  │  Step 2: Start Server  │ ───>  │  Step 3: Connect Apps  │
│  (dist/ folder)        │       │  (run_server.bat)      │       │  (See Section 3 Below) │
└────────────────────────┘       └────────────────────────┘       └────────────────────────┘
```

#### Step 1.1: Download & Extract
1. Download **`PDFtoAgent-Portable-stock-market-barometer-hamilton.zip`** ([Direct Download Link](https://github.com/babaksh/PDFtoAgent/raw/main/dist/PDFtoAgent-Portable-stock-market-barometer-hamilton.zip) or browse the [dist/](dist/) folder).
2. Extract the archive into any folder on your machine (e.g., `D:\PDFtoAgent-Portable` or `C:\PDFtoAgent-Portable`).

#### Step 1.2: Launch the Server (`run_server.bat`)
Double-click **`run_server.bat`**. The intelligent PowerShell launcher automates the entire runtime setup:
* 🔍 **Automatic Ollama CLI Setup:** Checks if Ollama is installed on your PC. If missing, it automatically installs it via the Windows Package Manager (`winget`) or the official CLI installer—no manual hunting for installers needed.
* 📦 **Automatic Model Verification:** Checks whether the required `nomic-embed-text:v1.5` semantic embedding model is cached locally. If missing, it downloads it directly in your terminal.
* 🚀 **Background Daemon:** Starts the Ollama service in the background if it is not already running.
* 🛡️ **Isolated Python Runtime:** Runs from a self-contained, pre-packaged virtual environment with all 100+ Dow Theory calculation tools, SQLite vector store, and FastMCP libraries ready to use.
* 🌐 **Server Online:** Binds strictly to your loopback adapter at `http://127.0.0.1:8765/mcp`.

```
===================================================================================
   PDF     to     Agent  --  HAMILTON DOW THEORY (1922)
   Standalone Portable MCP Distribution | Built by Babak
===================================================================================
  [OK] Ollama is installed.
  [OK] Model nomic-embed-text:v1.5 is ready.
  [OK] Ollama service is running.
  [*] Starting FastMCP Server on http://127.0.0.1:8765/mcp ...
===================================================================================
```

#### Step 1.3: Connect Your Favorite AI Client
Once `run_server.bat` is running, your MCP server is listening at `http://127.0.0.1:8765/mcp`. You can connect **Claude Desktop**, **Google Antigravity**, **ChatGPT Desktop**, **Cursor**, or **OpenClaw** in seconds.

👉 Refer to **`README.txt`** inside your extracted folder or see the complete **[Client Connection Guide (CONNECTING_APPS.md)](CONNECTING_APPS.md)** for ready-to-paste JSON configs and UI steps.

#### Step 1.4 (Optional): Zero-RAM Cloud Embeddings Mode
By default, the server runs completely offline using local Ollama embeddings (~500 MB RAM). If you prefer cloud embeddings with **0 MB local RAM usage**:
1. Open `config/.env` inside the portable folder with any text editor.
2. Set the provider to `nomic`:
   ```env
   EMBEDDING_PROVIDER=nomic
   NOMIC_API_KEY=your_nomic_api_key
   ```
   *(Nomic Atlas offers 1,000,000 free embedding tokens per month at [nomic.ai](https://nomic.ai)).*

---

### 🐳 Method 2: Docker Container Image (Cross-Platform)

For macOS, Linux, or Windows developers who prefer running through Docker Desktop, the server is available as an audited container image on Docker Hub.

#### Step 2.1: Prerequisites (One-Time Setup)

You only need to install these two tools once. After this setup, running any agent takes seconds.

##### Install Docker Desktop
1. Download and install **[Docker Desktop](https://www.docker.com/products/docker-desktop/)** for Windows, macOS, or Linux.
2. Launch Docker Desktop and verify the status icon shows **Engine Running** (green).

> 🛡️ **Container Security & Isolation:** Complete isolation and transparency. All container images in this showcase are automatically audited for vulnerabilities using **Aqua Security Trivy** (see the Security badge above). Furthermore, the container binds strictly to local loopback (`127.0.0.1`), executes under non-root privileges, and never transmits data outside your machine. Within Docker Desktop's interface, you can inspect the **Files** tab to see that all code is quarantined inside the container, view real-time logs, or stop it with a single click.

##### Install Ollama & Pull Embedding Model
The MCP server uses a local embedding model for semantic knowledge retrieval (RAG) so that **no external API keys or cloud services are required**.

1. Download and install **[Ollama](https://ollama.com/download)**.
2. Open your terminal (PowerShell, CMD, or Terminal) and run:
   ```bash
   ollama pull nomic-embed-text:v1.5
   ```
   *(This downloads the lightweight 270 MB embedding model to your machine).*
3. Ensure Ollama is running (it runs automatically in the background on port `11434`).

#### Step 2.2: Run the Container

The server is packaged as a single self-contained Docker image that serves **Streamable HTTP** on port `8765` (path `/mcp`).

Open your terminal and run:

##### Windows / macOS (Docker Desktop):
```bash
docker run -d --restart unless-stopped --name pdftoagent-stock-market-barometer-hamilton \
  -p 127.0.0.1:8765:8765 \
  -e EMBEDDING_PROVIDER=ollama \
  -e OLLAMA_EMBEDDING_HOST=http://host.docker.internal:11434 \
  -e OLLAMA_EMBEDDING_MODEL=nomic-embed-text:v1.5 \
  -e MCP_TRANSPORT=streamable-http \
  babak60/pdftoagent-stock-market-barometer-hamilton:latest
```

##### Linux:
```bash
docker run -d --restart unless-stopped --name pdftoagent-stock-market-barometer-hamilton \
  -p 127.0.0.1:8765:8765 \
  --add-host=host.docker.internal:host-gateway \
  -e EMBEDDING_PROVIDER=ollama \
  -e OLLAMA_EMBEDDING_HOST=http://host.docker.internal:11434 \
  -e OLLAMA_EMBEDDING_MODEL=nomic-embed-text:v1.5 \
  -e MCP_TRANSPORT=streamable-http \
  babak60/pdftoagent-stock-market-barometer-hamilton:latest
```

---

### 3. Connect to Your Agentic Apps

Once the server is running (via Portable `.bat` or Docker), it listens on `http://127.0.0.1:8765/mcp`.

👉 **For complete step-by-step setup walkthroughs and ready-to-paste configurations for Claude Desktop, ChatGPT, Google Antigravity, Cursor, and OpenClaw, see the [Client Connection Guide (CONNECTING_APPS.md)](CONNECTING_APPS.md)** *(also included inside the Portable bundle as `README.txt`)*.

---

## 🧪 Test Drive: 6-Month Bitcoin Analysis

Included in this repository is [`data/btc_ohlcv.csv`](data/btc_ohlcv.csv), containing historical Bitcoin daily OHLCV data.

### The Test Prompt
Attach `data/btc_ohlcv.csv` in your connected Agentic App (Claude Desktop, ChatGPT, Antigravity, OpenClaw, Cursor, etc.) and send the following prompt:

```text
I have attached the daily Bitcoin price dataset (btc_ohlcv.csv).

Please extract and analyze the last 6 months of data using Charles Dow and William Peter Hamilton's principles from 'The Stock Market Barometer':
1. What is the Primary Trend (Bull or Bear) according to Dow's higher-high / lower-low comparison? Include exact swing high/low levels and the break percentage.
2. Are there any Double Top or Double Bottom patterns detected within Dow's tolerances?
3. Which of Dow's three movements is the latest price action (Primary, Secondary reaction, or Day-to-Day)?
4. Does volume behavior validate the trend according to Dow's rule that 'volume confirms movement'?

Format the response into an executive dashboard with status badges, numerical swing coordinates, and list the exact calculation tools executed along with their provenance metadata.
```

### What Happens Behind the Scenes:
1. The Agentic App parses the CSV and invokes the Hamilton MCP server.
2. It executes `bull_bear_higher_high_lower_low_test`, `double_top_bottom_detector`, and `dow_three_movement_classification` inside the Docker container.
3. It renders a deterministic report with exact calculations:
   * **Primary Trend:** `BULL` (Latest swing high 85,190 exceeds prior average 83,476 by 2.05%).
   * **Pattern Alert:** No double top detected within the 1.5% tolerance band.
   * **Provenance:** Explicitly separates what was derived from Hamilton's 1922 text (`source_grounded`) versus calibrated algorithmic defaults (`model_extrapolated`).

---

## 🗺️ Roadmap & Pre-Built Agent Catalog

| Agent / Domain | Source Book | Status | Distribution Formats |
| :--- | :--- | :--- | :--- |
| **Dow Theory Quantitative Engine** | *The Stock Market Barometer* (1922) | 🟢 **Available** | 📦 **[Download Portable .zip](https://github.com/babaksh/PDFtoAgent/raw/main/dist/PDFtoAgent-Portable-stock-market-barometer-hamilton.zip)**<br>🐳 `babak60/pdftoagent-stock-market-barometer-hamilton` |
| **Tape Reading & Speculation** | *Reminiscences of a Stock Operator* (1923) | 🟡 In Pipeline | Portable .zip + Docker |
| **Market Cycles & Price Structure** | *Richard D. Wyckoff Method* (1910–1931) | 🟡 In Pipeline | Portable .zip + Docker |
| **Classical Scientific & Medical Reference** | Foundational Domain Treatises | ⚪ Planned | Portable .zip + Docker |

---

## 🏢 Enterprise Solutions & Custom Compilation

Have proprietary technical manuals, financial underwriting policies, compliance rulebooks, or internal SOPs?

I provide **on-premise, air-gapped deployments** and custom agent compilation services for enterprise clients:
* **Zero Cloud Leakage:** All processing, verification, and serving occurs entirely within your local or VPC infrastructure.
* **Deterministic Tool Synthesis:** Turn complex multi-page operational guidelines into verifiable, zero-hallucination computational tools.
* **Contact:** Connect with me for pilot programs and enterprise integrations at [`Babak`](https://github.com/babaksh) on GitHub or open an issue.

---

## ⚠️ Financial & Trading Disclaimer

* **No Financial Advice:** The materials, analysis, algorithms, and tools provided in this repository and within the generated MCP agents (including the Dow Theory and market barometer agents) are strictly for **educational, historical, and technical research purposes only**.
* **Not a Financial Advisor:** I am not a registered investment advisor, broker-dealer, or financial analyst. Nothing contained in this project constitutes investment, trading, legal, or financial advice.
* **User Responsibility:** Any trading or investment decisions made using these tools or their outputs are made entirely at your own risk. Past performance or historical algorithmic principles described in century-old literature do not guarantee future market results. Always conduct your own due diligence and consult with a licensed financial professional before risking capital.

---

## 📄 License

This showcase repository, the sample dataset, and the pre-compiled container images are released under the **PDFtoAgent Community & Research License (Non-Commercial)**:
* **Free for Personal, Educational, and Research Use:** You are welcome to run, study, and test the agent locally.
* **Commercial Redistribution Prohibited:** Sublicensing, commercial resale, hosting as a paid SaaS/API service, or repackaging into proprietary products is strictly prohibited without prior written permission.
* **Full Terms:** See the [`LICENSE`](LICENSE) file for complete legal details.
* **Commercial & Enterprise Inquiries:** To license for commercial production use or discuss custom agent compilation, contact [`Babak`](https://github.com/babaksh).

---

## ⚖️ Legal & Compliance Notice

* The pre-built Hamilton agent is derived exclusively from William Peter Hamilton's 1922 publication *The Stock Market Barometer*, which is in the **Public Domain** under U.S. Copyright Law (17 U.S.C. § 105/304).
* Under **17 U.S.C. § 102(b)**, mathematical procedures, algorithms, systems, and operational methods are excluded from copyright protection. Algorithmic tools generated by PDFtoAgent represent independent, functional software implementations.
* PDFtoAgent is designed for compiling lawfully acquired internal documentation, proprietary enterprise knowledge, and public domain literature.

---

<div align="center">
  <b>Turn your PDF into Action.</b><br>
  Maintained by <a href="https://github.com/babaksh">Babak</a>
</div>
