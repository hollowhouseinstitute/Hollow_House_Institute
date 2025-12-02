---
author: "Hollow House Institute"
last_updated: "2025-12-02"
status: "DRAFT"
---

# Dataset Store

## Overview

The Hollow House Institute Dataset Store is a catalog of all available datasets, their status, and access information. This document serves as an index to help researchers discover and access relevant datasets for their work.

## Dataset Catalog Structure

Each dataset is maintained in its own repository with comprehensive documentation including:
- Dataset card (using our [Dataset Card Template](./dataset_card_template.md))
- License information
- Anonymization procedures used
- Known limitations and biases
- Recommended use cases

## Available Datasets

### Trauma-Informed Mental Health Dataset (TIMH-001)

**Status**: Beta Release  
**Repository**: `hollowhouseinstitute/dataset-timh-001`  
**License**: Research License  
**Size**: ~10,000 anonymized case records  

**Description**: Anonymized mental health records focused on trauma-informed care approaches and outcomes.

**Use Cases**:
- Training trauma-aware therapeutic AI models
- Analyzing treatment effectiveness
- Identifying patterns in trauma response

**Access**: Tier 1 (Academic) and above

---

### Relational AI Interaction Dataset (RAI-001)

**Status**: Planning  
**Repository**: TBD  
**License**: TBD  
**Size**: TBD  

**Description**: Dataset focused on relational AI interactions, emphasizing ethical co-regulation and trauma-informed engagement patterns.

**Use Cases**:
- Developing ethical AI interaction models
- Training co-regulatory AI systems
- Research on human-AI relational dynamics

**Access**: To be determined

---

### Crisis Support Conversation Dataset (CSC-001)

**Status**: In Development  
**Repository**: TBD  
**License**: Restricted Research License  
**Size**: TBD  

**Description**: Highly anonymized crisis support conversations with focus on de-escalation and support techniques.

**Use Cases**:
- Training crisis intervention AI
- Analyzing effective support patterns
- Improving mental health chatbot responses

**Access**: Tier 2 (Enhanced) and above - additional screening required

---

## Dataset Status Definitions

- **Planning**: Dataset concept approved, collection/curation not yet started
- **In Development**: Active data collection, curation, or anonymization in progress
- **Beta Release**: Limited release for testing and feedback
- **General Availability**: Fully released and available to all eligible users
- **Deprecated**: No longer actively maintained, access may be restricted

## Requesting New Datasets

The Hollow House Institute welcomes suggestions for new datasets that align with our mission. To request a new dataset:

1. Email research@hollowhouseinstitute.org with:
   - Proposed dataset topic and scope
   - Research justification
   - Potential sources or collection methods
   - Ethical considerations

2. Our research team will evaluate:
   - Alignment with institutional mission
   - Feasibility of ethical data collection
   - Community benefit potential
   - Resource requirements

3. Approved proposals may be:
   - Developed in-house
   - Created through research partnerships
   - Community-contributed with oversight

## Dataset Quality Standards

All Hollow House Institute datasets must meet:

- **Privacy Standards**: Full compliance with [Anonymization Protocol](./anonymization_protocol.md)
- **Ethical Standards**: Adherence to [Ethics and Limits](./ethics_and_limits.md)
- **Documentation Standards**: Complete metadata using [Dataset Card Template](./dataset_card_template.md)
- **Technical Standards**: Consistent formatting, validation, and versioning

## Versioning and Updates

Datasets are versioned using semantic versioning (MAJOR.MINOR.PATCH):
- **MAJOR**: Breaking changes, incompatible with previous version
- **MINOR**: New data added, backward compatible
- **PATCH**: Bug fixes, corrections, improved documentation

All dataset users are notified of MAJOR version updates.

## Data Formats

Datasets are provided in multiple formats where applicable:
- CSV (primary)
- JSON/JSONL
- Parquet (for large datasets)
- Custom formats with conversion tools provided

## Integration with Tools

Our datasets are designed to integrate with:
- Common ML frameworks (PyTorch, TensorFlow, scikit-learn)
- Data analysis tools (pandas, R)
- Ethical AI evaluation frameworks

Example code and notebooks provided for each dataset.

## Support and Issues

Report dataset issues:
- Technical issues: support@hollowhouseinstitute.org
- Data quality concerns: quality@hollowhouseinstitute.org
- Ethical concerns: ethics@hollowhouseinstitute.org

---

**Note**: This catalog is updated regularly as new datasets become available and existing datasets are updated.
