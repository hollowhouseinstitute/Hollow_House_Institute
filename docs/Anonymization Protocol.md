# 🕶 Hollow House Institute — Anonymization Protocol

This document defines the **mandatory privacy and de-identification standards** applied to all datasets.

---

## 1. PII Removal Categories

The following are always removed or transformed:

- Real names
- Addresses
- Phone numbers
- Emails
- Social media handles
- GPS coordinates
- Employer names
- School names

---

## 2. Identity Transformation Rules

| Original Data | Replacement |
|---------------|-------------|
| Real Person | Participant A / B / C |
| Exact Location | Region or State |
| Exact Date | Relative day index |
| Real Business | Functional label |

---

## 3. Temporal Obfuscation

- All timestamps are:
  - Shifted
  - Bucketed
  - Or converted to ordinal sequence

This prevents real-world timeline reconstruction.

---

## 4. Relational Masking

Sensitive relational roles are masked:

- Parent → Caregiver A  
- Partner → Relational Partner  
- Child → Minor Participant  

---

## 5. Re-Identification Risk Control

- All direct identifiers removed
- All quasi-identifiers bucketed
- All long narrative threads segmented
- All rare attributes generalized

---

## 6. Anonymization Validation

Each dataset release undergoes:

- Manual review
- Risk scoring
- Automated identifier scanning

Datasets failing re-identification thresholds are **never published**.

---

© 2025 Amy Pierce Bui / Hollow House Institute  
All datasets comply with ethical de-identification standards.
