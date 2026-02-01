scenarioOS

scenarioOS defines how complex conversational work becomes a coherent, long-term process rather than a sequence of disconnected chat sessions.

Most conversational AI workflows focus on prompts, memory toggles, or context windows. scenarioOS focuses on continuity: how reasoning, assumptions, tone, constraints, and intermediate artifacts persist across sessions without relying on hidden model state.

scenarioOS is part of MetaMemoryWorks — a file-based architecture for persistent AI working memory.

🌐 https://metamemoryworks.com  
📄 Architecture: https://github.com/johannes42x/MetaMemoryArchitecture

Version: 0.9.0

---

What is scenarioOS?
scenarioOS is a conversational state and continuity system, not a prompt framework.

It turns a language model into something that can resume complex work as if no interruption occurred — even across fresh sessions, new contexts, or degraded long conversations.

scenarioOS does not attempt to preserve full chat transcripts. Instead, it extracts what actually matters for continuation: decisions made, constraints established, assumptions formed, artifacts created, and the interaction equilibrium that emerged.

The result is not recall, but orientation.

---

What problem scenarioOS addresses
Long conversations degrade.

As sessions grow, performance drops. Context becomes noisy. Prompts accrete rituals. Users hesitate to restart because too much implicit state would be lost.

This leads to brittle workflows and parasitic prompt engineering.

scenarioOS treats conversational work as a continuous process rather than a bounded session.

A session ending is not a reset. It is a checkpoint.

---

Core characteristics
Explicit reconstruction of conversational working state  
File-based persistence of context (human-readable, portable)  
Separation between raw conversation and scenario state  
Deterministic reinitialization rules  
Model-agnostic design  
No reliance on hidden or proprietary memory mechanisms  

scenarioOS does not attempt to optimize outputs. It stabilizes context.

---

What scenarioOS is not
scenarioOS deliberately avoids claims it cannot guarantee:

Not an agent framework  
Not an automation or execution system  
Not a planning or orchestration engine  
Not a memory toggle or embedding store  
Not a replacement for human judgment  

scenarioOS provides structure and continuity. Decisions remain contextual and human-directed.

---

How scenarioOS works in practice
scenarioOS operates across three phases:

Extraction  
At the end of a session, the model analyzes the interaction and extracts the effective working state.

Scenario file  
This state is written into an explicit scenarioOS file containing assumptions, constraints, artifacts, and interaction parameters.

Reinitialization  
In a new session, the scenarioOS file is loaded, restoring orientation and continuity without replaying the entire conversation.

The system does not preserve everything. It preserves what allows work to continue coherently.

---

Relation to MetaMemoryWorks
scenarioOS can be used standalone.

Within MetaMemoryWorks, it typically functions as:

a continuity layer for complex conversational work  
a bridge between short-term interaction and long-term reasoning  
an upstream component for research, writing, analysis, and system design workflows  

scenarioOS does not require MetaMemoryWorks, but integrates cleanly with it.

---

Installation & usage
scenarioOS is distributed as a file package.

There is nothing to install and nothing to configure. You upload the files into your LLM environment and begin.

Typical workflow:

Download and unzip scenarioOS  
Upload all files into a new project or session  
Work normally  
When context degrades, generate a scenario file  
Start a new session and load the scenario file  

Primarily tested with ChatGPT Projects. Other LLMs should work as long as file context is supported.

---

Versioning
scenarioOS follows semantic versioning.

Scenario formats and specifications may version independently.

---

Licensing
Private, non-commercial use: free  
Commercial or institutional use: license required  

See /legal/ for details.

For licensing: licensing@metamemoryworks.com  
For general contact: contact@metamemoryworks.com  

MetaMemoryWorks — do EVERYTHING.
