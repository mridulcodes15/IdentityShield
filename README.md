# 🛡️ IdentityShield — Neural_Nexus

> **Real-Time Multimodal Deepfake Detection, Coercion Prevention & Digital Trust Platform**
> *Developed for Smart India Hackathon 2026 (SIH 2026)*

---

## 📌 Overview

**IdentityShield** is an AI-powered, real-time threat detection and early intervention ecosystem designed to shield citizens, corporate executives, and institutions from synthetic voice cloning, video deepfakes, authority impersonation, and "Digital Arrest" coercion scams.

Unlike legacy reactive security systems that analyze recorded media after financial or identity loss has occurred, IdentityShield operates on a **proactive, two-stage detection model**. It passively screens continuous incoming media and selectively escalates to deep multimodal analysis (Voice + Video + Context) upon detecting suspicious signals—providing instant, on-screen warnings during active calls.

* 📊 [View Target Audience & Impact Diagram](assets/target-audience-flowchart.png)

---

## 🔬 Research & External Resources

The technical architecture, legal positioning, and empirical benchmarks supporting IdentityShield are documented in detail:

* 📄 **Technical Research & Legal Specs:** See [`docs/Research.md`](docs/Research.md) for benchmark datasets, competitor matrices, and DPDP Act compliance notes.
* 📂 **External Research Repository:** [Access Neural_Nexus Google Drive Folder](https://drive.google.com/drive/folders/1kEshmEFXIH1pF_I_JMJKXndjwZukFLTW)

---

## 🚀 Key Features

* 📱 **Real-Time Active Call Screening:** Passive, low-power monitoring that alerts users live during incoming voice or video interactions.
* 🎙️ **Voice Cloning & Synthetic Audio Detection:** On-device acoustic feature extraction analyzing spectral anomalies, phase distortion, and synthetic artifacts.
* 🎥 **Video Deepfake & Visual Anomaly Spotting:** Frame-by-frame visual integrity checks flagging facial manipulation, temporal inconsistencies, and synthetic rendering.
* 🗣️ **NLP Context & Coercion Intelligence:** Speech-to-text combined with natural language understanding to detect extortion patterns, authority impersonation (e.g., police, legal, banking), and high-urgency financial coercion.
* ⚙️ **Two-Stage Targeted Trigger Pipeline:** Lightweight screening runs continuously; deep multimodal model pipelines trigger only when potential anomaly thresholds are breached—conserving system resources and battery.
* 🔒 **Cryptographic Incident Vault (SHA-256):** Generates local, tamper-evident audit logs with cryptographic hash integrity verification for reporting cybercrime evidence to authorities.
* 🛡️ **Privacy-First Architecture:** Local edge-oriented processing compliant with India's Digital Personal Data Protection (DPDP) Act.

---

## 🏗️ System Architecture & Workflow

### Technical Architecture

IdentityShield integrates three core analysis engines (Voice, Video, and Context) into a unified **Multimodal Threat Fusion Framework** to compute a real-time Confidence & Risk Score (*Low*, *Moderate*, *High*, *Very High*).

* 📐 [View Technical Architecture Diagram](assets/technical-architecture.png)

---

### Step-by-Step Incident Execution Flow

* 🔄 [View System Execution Flowchart](assets/system-workflow.png)

1. **Incoming Voice / Video Call:** Call is initiated or answered on the target user's device.
2. **Lightweight Monitoring:** Continuous passive screening evaluates baseline acoustic and conversational signals.
3. **Trigger Event Detection:** Suspicious indicators (audio anomaly, coercion terminology) activate the deep capture engine.
4. **Targeted Multimodal Capture:** Recent audio context, current video frames, and live transcript snippets are passed to specialized analysis models.
5. **Multimodal Threat Fusion:** Cross-correlates synthetic audio likelihood, visual deepfake scoring, and coercion/urgency context.
6. **Threat Risk Assessment:** Assigns real-time risk tiers (*Low*, *Moderate*, *High*, *Very High*).
7. **Real-Time Warning & Mitigation:** Triggers on-screen warning overlays (`"Possible Fraud / Impersonation Detected"`), prompting the user to end or block the call safely.
8. **Incident Log & Cryptographic Export:** Logs timestamped threat metadata locally and generates a downloadable SHA-256 hashed incident report.

---

## 🛠️ Tech Stack

| Domain | Technology / Framework | Usage |
| --- | --- | --- |
| **Frontend UI / Prototype** | HTML5, Tailwind CSS, Vanilla JavaScript (ES6+) | Interactive real-time simulation dashboard |
| **Icons & Visuals** | Lucide Icons, Custom SVG / Canvas graphics | Modular UI status badges & workflow charts |
| **Audio Processing** | Web Audio API / PyTorch / ONNX Runtime | Acoustic spectrogram & synthetic voice analysis |
| **NLP & Speech Text** | Whisper / Speech-to-Text APIs, Transformer NLP | Coercion keyword extraction & transcript analysis |
| **Crypto & Integrity** | Web Crypto API (`crypto.subtle.digest`) | SHA-256 hashing for tamper-evident report generation |
| **Target Platforms** | Web Dashboard, Mobile App (Flutter / Android Native) | Multi-device user & enterprise coverage |

---
## 📂 Project Structure

```text
sih2026/
├── assets/
│   ├── system-workflow.png
│   ├── technical-architecture.png
│   └── target-audience-flowchart.png
├── docs/
│   └── Research.md
├── frontend/
│   └── index.html
├── .env.example
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
└── README.md
```
🏁 Getting Started
Prerequisites
Any modern web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, or Safari).

VS Code with the Live Server extension installed (optional, recommended).

Running the Interactive Prototype Locally
Clone the Repository:

Bash
git clone [https://github.com/YOUR_USERNAME/sih2026.git](https://github.com/YOUR_USERNAME/sih2026.git)
cd sih2026
Launch via Live Server (Recommended):

Open the sih2026 folder in VS Code.

Navigate to frontend/index.html.

Right-click index.html and select "Open with Live Server".

Direct File Preview:

Open frontend/index.html directly in any standard browser.

🔐 Security, Privacy & DPDP Compliance
Local Processing First: Media streaming for continuous monitoring is processed directly on-device or via secure local buffer pipelines.

No Unsolicited Storage: Raw audio and video streams are never continuously saved or transmitted to external third-party servers.

User-Controlled Evidence: Incident logs and SHA-256 digests are generated client-side and saved exclusively under explicit user command.

📜 License
This project is licensed under the MIT License — see the LICENSE file for full details.
