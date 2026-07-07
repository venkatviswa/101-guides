# 101 Guides

Concise, opinionated 101 guides for architects and enterprise practitioners — the concepts that explain most day-to-day work, the vocabulary worth internalising, and the tradeoffs that decide which approach fits. Written to answer *"what should I understand before making a call?"* rather than to replace vendor docs.

Each guide is standalone; cross-references between them are called out inline.

## Guides

### [Snowflake 101](./snowflake101.md) — concepts, enterprise positioning & key SQL cheatsheet

The mental model (separated storage, compute, and cloud services), core objects (warehouses, roles, databases/schemas, tables, views, streams, tasks, dynamic tables), extending Snowflake with UDFs/UDTFs/Snowpark, an SQL cheatsheet, Iceberg tables, Cortex AI, Snowflake on AWS, and a full **Snowflake ↔ Salesforce Data 360** section covering the four interop directions (federation in, file federation, zero-copy sharing back) plus a "Why Data 360" subsection with without-vs-with and decision-tree diagrams.

### [ML 101](./ml101.md) — concepts, evolution, and choosing the right model for the job

How ML evolved from statistical learning to deep learning to LLMs, the difference between the two, model families (tabular / text / vision / time-series / unsupervised / recommenders), a business-question → task → metric table, an **ML vs. LLM vs. Rules** decision table, the ML lifecycle in practice, feature engineering, AutoML's traps, MLOps essentials, and a runnable Python starter (scikit-learn + LightGBM) plus a time-series forecasting starter. Written for architects and engineering leads, not as a math-first textbook.

### [LLM 101](./llm101.md) — concepts, enterprise positioning & the API surface worth knowing

The stateless-function mental model, tokens/context/temperature, reasoning models, tool use and the agent loop, MCP as the tool-integration standard, RAG, when fine-tuning is (and isn't) the right move, deployment options, the LLM API shape worth memorising, a Jan 2026 model snapshot, and a runnable Anthropic SDK Python example. Complements *ML 101* — read that one for classical/predictive ML and this one for the language-model surface.

### [LLM for Salesforce Architects](./LLM%20for%20Architects.md) — deep-dive companion

The longer, deeper companion to *LLM 101*, oriented at Salesforce architects specifically: neural-network and transformer internals, key hyperparameters, a detailed model catalog, a full lifecycle walkthrough (architecting → pre-training → fine-tuning → RAG → deployment), prompt engineering, RAG beyond the basics, deployment options, Salesforce-and-LLMs (Agentforce, Einstein, Data 360 grounding), and a BYOLLM-vs-hosted recommendation framework. Read *LLM 101* first for the mental model, then this for depth.

## How to read these

Each guide starts with a one-line mental model and a Contents index. Skim the Contents, jump to what you need, and treat the code blocks as starting points rather than production templates. The "gotchas" and "what this 101 intentionally does not cover deeply" sections are where the honest limits live — worth reading before you commit to an approach.
