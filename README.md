# 🕵️‍♂️ Threat Hunting Playbooks for APT Activity

Welcome to the **APT Threat Hunting Playbooks** repository — a curated collection of **true, intelligence-driven threat hunts** built for defenders, threat hunters, and detection engineers. These playbooks are designed to proactively uncover stealthy adversary behavior in your environment **without relying on alerts**.

---

## 🎯 Purpose

This repository provides **assumption-based threat hunt chains** focused on real-world adversaries such as **APT29, APT41, APT10, FIN6, and APT27**. Each hunt breaks down known TTPs into **actionable steps** using:

- Windows Event Logs
- Sysmon telemetry
- Authentication records
- File, process, and network artifacts
- Hypothesis-driven methodology

---

## 🧠 Methodology

Each hunt follows this structure:

- **🎯 Objective** — What behavior are we trying to uncover?
- **✅ Hypothesis** — What are we assuming the adversary is doing?
- **🧱 Tactics to Focus On** — ATT&CK-style breakdown of scope
- **🔍 Hunt Chain** — Step-by-step investigation flow using logs
- **💡 Thought Process** — Why the step matters, what to ask yourself
- **🧠 Summary** — What you’ve accomplished and what to do next

These are **not alert-centric** — they're designed to help you hunt with **no EDR trigger**, just logs and threat intel.

---

## ⚙️ How to Use

1. Pick a playbook based on threat actor or technique.
2. Review the hypothesis and steps.
3. Query your SIEM/EDR using Sysmon/Event IDs provided.
4. Adjust logic to match your log schema or visibility.
5. Document findings and escalate as needed.

---

## 📌 Requirements

These playbooks assume access to:

- Windows Event Logs
- Sysmon logs (especially IDs: 1, 3, 10, 11, 13)
- Network logs (Zeek, Suricata, Proxy)
- Authentication telemetry (4624, 4648, 4672, etc.)
