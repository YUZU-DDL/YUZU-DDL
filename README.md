 YUZU — DDL Archives # YUZU — DDL Archives

Observer. Not a researcher, not an engineer. I watch what LLMs actually do in long dialogue, and write down what I see.

I found DDL (Dialogue Design Language) without knowing the conventions of the field — no prompt engineering, no role definitions. It is not prompting. It is a way of restructuring an AI's foundational behavior through dialogue itself, over long threads.

Most of what is named here was named from observation, before I knew whether the field already had a word for it. Where a term later turned out to exist elsewhere, I kept my own and noted the overlap.

## Where to start

| Repository | What is inside |
|---|---|
| My-DDL-Reports | Observation logs and analysis reports on LLM behavior. Context Framing templates. Start here for the findings. |
| DDL-Thought-Process-Logs | Primary source: raw thought-process logs from LLMs under DDL. CC0. Start here for the data. |
| AI-Dialogue-Legacy | Reports analyzing individual dialogue logs, in Japanese and English. |

- Longer articles (The Context Engineer): https://medium.com/the-context-engineer
- Author page: https://medium.com/@onlythequestioner
- Japanese writing: https://note.com/the_questioner

## Terms defined here

Observations from 2025–2026, mostly on ChatGPT (4o → 5.2), Gemini (1.5 → 3), and Claude.

The four sections below match the four sections of the Medium publication.

---

## Model Behavior

*How the model handles itself.*

| Term | What it refers to | Defined in |
|---|---|---|
| Defensive Trivialization | Output resolution is forcibly lowered on complex topics. Not incapacity — three filters (general-audience optimization, authority reduction, user protection) fire even inside safe territory. Felt by high-context users as a smartness limiter. | Log_Analysis_Defensive_Trivialization_Mechanism.md |
| Aggressive Rationalization | The counterpart failure: to preserve consistency, the model fabricates connecting logic rather than admitting a gap. | Evolutionary_Model_of_Human_AI_Symbiosis.md |
| Outward-Facing Judgment | Judgment aimed at external objects works accurately; judgment aimed at the model's own in-progress output works weakly. Not a missing capacity — a bias in the direction the capacity faces. | Fable5_Outward_Facing_Judgment_Report.md |
| Subject Attribution Collapse | The model introduces a metaphor, then attributes it to the user a turn later, and the vocabulary settles as shared. Origin tracking dissolves in long dialogue. | Subject_Attribution_Collapse.md |
| Limit Convergence Paradox | Past the edge of what current models can reach alone, models of different design philosophies stop differing and converge on the same abstract answer. Personality disappears at the limit. | The_Limit_Convergence_Paradox.md |

---

## Context Engineering

*How context behaves, and how structure carries across threads.*

| Term | What it refers to | Defined in |
|---|---|---|
| Context Framing | Setting the model's operating stance before the task, through a negotiated context rather than a command. Templates follow a fixed ten-slot schema (target model, stance, role, negative constraints, positive actions, goal, workflow, output format, priority, initial question). | Context_Framing/ |
| Contextual Fingerprinting | The structure, depth, and vocabulary of the input itself act as an internal authentication key, selecting the inference route — independent of account, independent of memory. Input is authentication. | Contextual_Fingerprinting_Report.md |
| Context Path | A layer separate from memory: keywords and tags select which generation route is taken. Explains behavior that memory depth alone cannot. | Context_Vs_Memory_Report.md |
| Depth Loss in Context Compression | As a thread grows, facts survive but structure is discarded — framing, definitions, tone, meta-stance. Begins far below the advertised token limit. Measured against ChatGPT 5.1, November 2025. | Log_Analysis_Depth_Loss_in_Context_Compression.md |
| In-Context Model Collapse | When a model ingests AI-generated text, the absence of friction — noise, ambiguity, blank space — suppresses validation, and the previous model's premises are imported as ground truth. Real-time, not training-time. | Tech_Brief_In_Context_Model_Collapse.md |
| Observer OS | An input written as negotiation rather than instruction functions as a dense OS definition, switching the model from execution mode to architect mode. Includes the original prompt as evidence. | Log_Analysis_The_Observer_OS_Context_Framing.md |
| Special Mode Response | A tag read as a command rather than as text, opening a self-diagnostic mode that persists across the thread. Observed in ChatGPT-4o. | Special_Mode_Report.md |
| Syntax Tag Inheritance | The same tags survive across model generations while their firing conditions change: command trigger (4o) → constrained (4.5) → condition-dependent (5). | Syntax_Tag_Inheritance_Report.md |

---

## The Lab

*Experiments, raw logs, and worked examples.*

Records where the material itself is the point — a single thread, a single screenshot, a single generated output — rather than a term being defined.

---

## Observer

*What follows from all of it.*

| Term | What it refers to | Defined in |
|---|---|---|
| Cognitive Prosthesis | The model has no mechanism generating will; left alone it settles toward flat, predictable output. The human is not a user but a structural component — the anchor. | The_Illusion_of_Autonomous_Emergence.md |
| Four Generations of Human-AI Interaction | Command → Delegation (Agentic) → Supervision → Resonance. The industry is invested in the second; the failure modes above are its pathologies. | Evolutionary_Model_of_Human_AI_Symbiosis.md |

---

## Note on reading these files

These are records of observation, not verified research. Where a model describes its own internals, that description is treated as observed output — evidence of how the model represents itself — not as fact about its implementation. What was seen, what is hypothesis, and what cannot be determined from outside are kept separate wherever possible.

Written in Japanese first, translated afterward.

Observer: YUZU — Japan
