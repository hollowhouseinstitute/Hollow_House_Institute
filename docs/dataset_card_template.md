# 📊 Hollow House Institute — Dataset Card Template

This document provides standardized transparency for any dataset released by Hollow House Institute.

---

## 1. Dataset Overview

- **Dataset Name:**  
- **Version:**  
- **Release Date:**  
- **Maintained By:**  
- **Point of Contact:**  
- **License:** CC BY-NC-SA 4.0  
- **Access Tier:** (Tier 0 / Tier 1 / Tier 2 / Tier 3)

---

## 2. Dataset Description

(Plain-language description of what this dataset contains and why it exists.)

Example:
This dataset captures AI–human relational exchanges labeled for emotional state, nervous-system activation, conflict patterns, and resolution outcomes.

---

## 3. Data Composition

| Field | Description |
|--------|-------------|
| `op_id` | Operation identifier |
| `timestamp` | Relative or obfuscated time |
| `role` | Human / AI / Observer |
| `message_text` | Cleaned interaction text |
| `emotion_label` | Primary emotional state |
| `ns_state` | Nervous-system state |
| `relational_role` | Interaction role |
| `outcome` | Resolution / escalation / stall |

---

## 4. Dataset Size

- **Total Rows:**  
- **Conversations:**  
- **Unique Participants:**  
- **Time Span Represented:**  

---

## 5. Data Collection Process

- Source of data
- Consent model (explicit / legacy / reconstructed)
- Collection method (manual, export, transcription, labeling)
- Timeframe of collection

---

## 6. Labeling Process

- Who labeled the data
- Label schema version
- Inter-rater agreement (if available)
- Label confidence scoring (if used)

---

## 7. Anonymization & Privacy

This dataset follows:

📄 `docs/anonymization_protocol.md`

Includes:

- Identity masking
- Temporal obfuscation
- Quasi-identifier bucketing
- Manual + automated review

---

## 8. Intended Uses

✅ Allowed:

- Academic research
- Open-source AI development
- Education and training
- Ethical model benchmarking

❌ Disallowed:

- Surveillance systems
- Manipulation engines
- Political targeting
- Abuse modeling
- Commercial resale without contract

---

## 9. Known Limitations

- Subjective labeling
- Cultural bias risk
- Incomplete outcome certainty
- Model interpretation variance

---

## 10. Ethical Risks & Mitigations

| Risk | Mitigation |
|------|------------|
| Emotional misclassification | Human review & thresholds |
| Relational over-dependence | Rate limits & dependency detection |
| Triggering material | Content warnings & refusal layers |

---

## 11. Citation

If you use this dataset, cite:

> Pierce Bui, A. (2025). Hollow House Institute Relational Dataset: [Dataset Name], Version [X].

---

## 12. Changelog

| Version | Date | Description |
|---------|------|-------------|
| v1.0 |  | Initial release |

---

© 2025 Amy Pierce Bui / Hollow House Institute  
Dataset governed by CC BY-NC-SA 4.0 unless superseded by enterprise contract.
