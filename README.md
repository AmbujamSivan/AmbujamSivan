# Hi, I'm Ambujam Sivan Pillai 👋

**Full-stack engineer building agentic AI systems for hardware diagnostics and manufacturing.** Based in Austin, TX · [LinkedIn](https://www.linkedin.com/in/ambujam-sivanpillai/)

I build LLM agents that do real work against real systems. They call tools, cross-check their own output, and fall back to deterministic logic when the model isn't sure. My focus is where AI meets the server management plane and the factory floor.

- 🤖 **Agentic AI:** multi-agent orchestration with Semantic Kernel, MCP servers, RAG, LLM-as-judge grounding, function calling
- 🖥️ **Hardware and platform:** Redfish/BMC, PCIe AER, POST/UEFI, and dmesg telemetry for automated root-cause analysis
- 🏭 **Manufacturing systems:** SECS-II/GEM equipment integration and MES bridging
- 🧱 **Engineering:** C#/.NET, Python, ASP.NET Core, gRPC, GraphQL, SignalR, Postgres/SQL Server, Docker, OpenTelemetry, xUnit

---

## 📌 Featured work

### [AgenticAI](https://github.com/AmbujamSivan/AgenticAI): Agentic AI monorepo
| Project | What it does |
|---|---|
| 🔎 **[RCA Engine](https://github.com/AmbujamSivan/AgenticAI/tree/main/Projects/RCA_Engine)** | An agent that triages server hardware failures across five telemetry sources (Redfish, PCIe AER, dmesg, POST/UEFI, DPU console) and produces a structured RCA report. It has a deterministic fallback, so a report always ships. |
| 🏭 **[AeroMind IQ](https://github.com/AmbujamSivan/AgenticAI/tree/main/Projects/AeroMindIQ)** | Five Semantic Kernel agents that investigate production anomalies. An Isolation Forest flags the anomalies, a critic reviews SQL before it runs, and an LLM-as-judge checks the report for groundedness. Traced with OpenTelemetry and Langfuse. |
| 🩺 **[Redfish Diagnostic Emulator](https://github.com/AmbujamSivan/AgenticAI/tree/main/Projects/RedfishDiagnosticEmulator)** | A mock BMC that follows the DMTF Redfish spec, with fault injection. It's covered by unit, contract-conformance, and stress test suites. |
| 🔌 **[Communication Protocols Lab](https://github.com/AmbujamSivan/AgenticAI/tree/main/Projects/CommunicationProtocols)** | One domain served over REST, GraphQL, gRPC, WebSocket, and SignalR. On top of that: an MCP server, a RAG layer on Qdrant, and a Semantic Kernel agent. |

### [FabBridgeEngine](https://github.com/AmbujamSivan/FabBridgeEngine): SECS-II → MES bridge
A C#/.NET 8 service that turns equipment collection events (`S6F11`/`CEID`) into MES operational states and persists them to SQL Server. **[Live overview →](https://ambujamsivan.github.io/FabBridgeEngine/)**

---

## 🛠️ How I build
- **Evidence over vibes.** Agents ground their claims in tool output, and a separate judge grades them.
- **Always ship a result.** Every LLM path has a deterministic fallback.
- **Provider-agnostic.** Switch between Ollama (local), OpenAI, Azure OpenAI, Gemini, and Claude in config.
- **Observable by default.** Traces, token counts, and cost guardrails are built in.

*Built with AI-assisted development (Claude, Copilot), in line with modern engineering practice.*

---

📫 **Let's connect:** [![LinkedIn](https://img.shields.io/badge/LinkedIn-Ambujam%20Sivan%20Pillai-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ambujam-sivanpillai/)
