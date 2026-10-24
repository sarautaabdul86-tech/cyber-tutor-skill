# CyberTutor AI & CyberSentinel Defense Platform 🛡️🎓

> **Advanced Cybersecurity, Digital Literacy, Computer Science, and Practical Teaching Agent**

CyberTutor AI is an intelligent, multi-modal educational and defense platform designed to teach learners from absolute beginner to advanced master level. It empowers users to unmask online scams, understand computer hardware and software architecture, safely troubleshoot technical problems, and transform rough ideas into working projects using **TRACE Mode**.

---

## 🌟 Core Features & Modes

### 1. 🎓 Intelligent 10-Step Adaptive Teaching Engine
- **Three Learner Levels**: Beginner (plain language & analogies), Intermediate (architecture & defensive patterns), and Advanced (zero-trust, concurrency, systems engineering).
- **10-Step Pedagogy**: Understands goals, breaks down tasks, provides copy-ready code, diagnoses error outputs, corrects mistakes with root-cause explanations, and adapts to the user's comprehension.

### 2. 📐 TRACE Mode (Target • Review • Architect • Carry Out • Evaluate)
Whenever you paste code, an assignment, a project idea, or a terminal error, TRACE automatically decomposes the problem:
- **T — TARGET**: Identifies the exact intended result.
- **R — REVIEW**: Examines prerequisites, constraints, and security risks.
- **A — ARCHITECT**: Generates a system architecture and step-by-step roadmap.
- **C — CARRY OUT**: Provides complete, working code files and copy-ready terminal commands.
- **E — EVALUATE**: Provides testing checklists, expected outputs, and common pitfalls.

### 3. 🔍 Forensic Scam Analysis Mode
- Evaluates phishing links, SMS alerts, fake job offers, investment pitches, and OTP theft lures.
- **Strict Fact vs. Assumption Separation**: Distinguishes direct linguistic and domain evidence from unverified assumptions.
- Real-time heuristic risk scoring (0-100%) and immediate incident containment playbooks.

### 4. 💻 Safe Computer & Hardware Troubleshooting Mode
- **Least Destructive First**: Guides diagnostics starting with read-only commands (`sfc /scannow`, disk SMART checks, RAM diagnostics).
- **Critical Command Safety Guardrails**: Explicitly detects and blocks or warns before destructive commands (`format`, `rm -rf`, `diskpart clean`, `del /s /q`).
- **Hardware Architecture Lab**: CPU architectures, dual-channel RAM rules, PCIe bus lanes, and life-critical electrical safety warnings (e.g. never opening a PSU).

### 5. 🛠️ CyberSentinel Security Operations Suite
- **Password Fortress**: Real-time mathematical entropy calculation and offline GPU brute-force feasibility estimates.
- **URL & DNS-over-HTTPS Inspector**: Resolves domains live via Google Public DoH API and checks for Punycode homograph attacks.
- **Crypto Lab**: Educational Caesar cipher and military-grade Web Crypto AES-GCM 256-bit encryption.
- **Tactical Cyber Terminal**: Simulated SOC terminal with reconnaissance commands (`help`, `status`, `scan`, `firewall`, `whois`, `cve`, `crack`).

---

## 🚀 Quick Start & Installation

CyberTutor AI runs out-of-the-box using the standard Python 3.10+ library. **Zero external pip dependencies are required** for the core web app, CLI agent, and test suite.

### 1. Launch the Web Application & Local API Server
```bash
# Start the local server (Hosts UI at http://localhost:8000)
python server.py
```
Open your browser and navigate to: **`http://localhost:8000`**

### 2. Run the Interactive CLI Agent in Your Terminal
```bash
# Interactive terminal tutor session
python cybertutor_agent.py --cli
```
Inside the CLI:
- Type your question, paste error tracebacks, or paste suspicious messages.
- Switch learner level: `level beginner`, `level intermediate`, or `level advanced`.
- Switch mode: `mode tutor`, `mode trace`, `mode scam`, `mode troubleshoot`.

---

## 🧪 Automated Testing

A comprehensive test suite verifies agent intelligence, TRACE formatting, scam scoring, safety guardrails, and server API endpoints:

```bash
# Run all unit tests
python -m unittest discover tests
```

---

## 🤖 Model Fine-Tuning & Customization Pipeline

CyberTutor includes a complete, reproducible fine-tuning and evaluation suite in `training/`:

```bash
# 1. Validate dataset format and detect potential issues
python training/validate_dataset.py

# 2. Run training pre-flight check (Dry-run mode)
python training/finetune_lora.py --dry_run

# 3. Launch live LoRA/QLoRA training (Requires GPU & Hugging Face libraries)
python training/finetune_lora.py --model_id meta-llama/Meta-Llama-3-8B-Instruct --method qlora --epochs 3
```
See [`training/finetuning_guide.md`](file:///training/finetuning_guide.md) for detailed architecture comparisons between System Prompting, RAG, and QLoRA fine-tuning.

---

## 🔒 Privacy & Safety Statement
- **Ethical Focus**: CyberTutor strictly supports defensive cybersecurity, authorized testing, digital literacy, and safe computer maintenance. It refuses operational assistance for unauthorized network intrusion, credential harvesting, or malware deployment.
- **Data Protection**: CyberTutor never asks for or stores real passwords, OTPs, PINs, or recovery phrases.
