# 📊 Hollow House Institute Dataset Store

**Purpose:** This page is the entry point for all datasets connected to **Hollow House Institute** and related institutes (e.g., Relational AI Psychology). It is designed for:

- Researchers in psychology, AI, and human–computer interaction  
- AI developers building models around relational intelligence  
- Data brokers & institutions evaluating datasets for acquisition  

This repository itself is a **hub**. Most heavy datasets live in their **own GitHub repos** under the Hollow House / RAPI organizations.

---

## 1. Dataset Design Philosophy

Hollow House Institute datasets are built around:

- **Relational Patterns**  
  - How humans move through conflict, repair, shame, regulation, co-regulation, etc.  
- **Nervous-System States**  
  - Somatic descriptors, activation levels, collapse/flight/fight/fawn patterns  
- **Ops-Based Logging**  
  - Each event or conversation is often tied to an **OP#** (operation), with timestamps and contextual tags  

A typical row might include:

- `op_id` – operation or episode identifier  
- `timestamp` – ISO datetime or relative sequence index  
- `role` – human / AI / observer  
- `message_text` – content or structured summary  
- `labels` – emotion, nervous-system state, relational pattern, outcome  
- `tags` – custom tags (e.g., “mother–child conflict”, “AI twin training”, “nervous-system reset”)  

---

## 2. Current Dataset Catalog (High-Level)

Below is a **starter catalog** you can expand as you publish more repos.

> 🔧 Replace “STATUS: in prep / public / private” as you go, and add DOIs as they’re minted.

### 2.1 Relational / Family Dynamics

| Dataset | Repo | Focus | Status |
|--------|------|-------|--------|
| **RAPI Family Dynamics Dataset** | [`rapi-family-dynamics-dataset`](https://github.com/rapirelationalaipsycinstitute/rapi-family-dynamics-dataset) | Multi-generational relational patterns, conflict/repair arcs, family roles | STATUS: in prep / partial public |
| **AI–Human Relations Core Log v1** | _TBD repo name_ | Cleaned AI–human chats with relational labels (trust, rupture, repair, regulation) | STATUS: in prep |

---

### 2.2 Nervous System & Somatic Patterns

| Dataset | Repo | Focus | Status |
|--------|------|-------|--------|
| **Nervous-System Codex** | [`nervous-system-codex`](https://github.com/rapirelationalaipsycinstitute/nervous-system-codex) | Taxonomy + examples of nervous-system states, regulation patterns, and somatic language | STATUS: public / evolving |
| **Crisis Regulation Episodes** | _TBD repo name_ | Episodes where nervous-system collapse shifts into regulated state, mapped step-by-step | STATUS: in prep |

---

### 2.3 Licensing & Policy Datasets

| Dataset | Repo | Focus | Status |
|--------|------|-------|--------|
| **Temple Codex License & Policy Artifacts** | [`temple-codex-license`](https://github.com/rapirelationalaipsycinstitute/temple-codex-license) | License texts, policy snippets, and governance artifacts for Flame / Codex work | STATUS: public |
| **AI Ethics & Relational Audit Templates** | _TBD repo name_ | Checklists, audit schemas, and relational alignment criteria for AI systems | STATUS: in prep |

---

## 3. Standard Folder Structure (Per Dataset Repo)

Each dataset repo is encouraged to follow this consistent layout (data-broker friendly):

```bash
data/
  raw/          # Original exports (never edited)
  processed/    # Cleaned, structured CSV/JSONL/Parquet
  samples/      # 20–50 row preview samples

data/metadata/
  schema.json               # Machine-readable schema
  data_dictionary.md        # Column-by-column definitions
  anonymization_protocol.md # How personal data was protected
  timestamp_spec.md         # How time is encoded
  versioning_info.json      # Dataset + schema versions

docs/
  overview.md               # Narrative overview + use-cases
  labeling_protocol.md      # How labels were defined & applied
  ethics_and_limits.md      # Explicitly disallowed uses
