# Evaluation Context Protocol (ECP)

> **The Standard for Agent Evaluation.**

> Work in progress: we are actively evolving, and some concepts may change.

<div align="center">

[**Documentation**](https://evaluation-context-protocol.github.io/ecp/) | [**Core Repository**](https://github.com/evaluation-context-protocol/ecp)

</div>

---

### 🎯 Our Mission

As AI Agents move from chat interfaces to executing real-world tasks, evaluating them based solely on their final answer is no longer sufficient.

The **Evaluation Context Protocol** gives you a standard way to run deterministic evaluations of AI agents. We are developing open standards and tooling that force agents to expose their internal reasoning, tool usage, and state during testing, without requiring changes to production code.

We believe that to trust an autonomous system, you must be able to verify its **process**, not just its output.

### 🧩 The Ecosystem

We maintain the core protocol specifications and reference implementations.

| Repository | Description | Status |
| :--- | :--- | :--- |
| [**`ecp`**](https://github.com/evaluation-context-protocol/ecp) | **Python SDK.** Contains the Python SDK (for agents) and the Runtime CLI (for evaluation runners). | 🟢 Active |
| [**`protocol`**](https://github.com/evaluation-context-protocol/ecp/blob/main/spec/protocol.md) | The language-agnostic specification for the JSON-RPC based evaluation protocol. | 📜 Standard |

### 🚀 Why ECP?

Traditional evaluation frameworks (like Ragas or generic LLM judges) focus on semantic similarity or retrieval quality post-hoc. ECP is a **runtime environment** that sits between the test suite and the agent.

* **Verify Safety:** Did the agent internally flag PII before refusing the request?
* **Verify Logic:** Did the agent use the calculator tool, or did it hallucinate the math?
* **Verify Efficiency:** How many steps did the agent take to reach the conclusion?

### 🤝 Community & Contributing

ECP is an open standard intended to support any framework (LangChain, LlamaIndex, CrewAI, AutoGen, etc.).

We welcome contributions of all sizes, especially:
* Adapters for new agent frameworks.
* New Grader types for the runtime.
* Improvements to the core protocol specification.

Please see the main [ecp repository](https://github.com/evaluation-context-protocol/ecp) to get started.

---
<p align="center">
<i>Licensed under Apache 2.0.</i>
</p>
