---
author: "Hollow House Institute"
last_updated: "2025-12-02"
status: "DRAFT"
---

# Model Card Template

## Purpose

This template helps researchers create comprehensive documentation for AI/ML models developed using Hollow House Institute datasets. Model cards promote transparency, enable informed use, and facilitate ethical review.

Based on: Mitchell et al. (2019) "Model Cards for Model Reporting"

---

# Model Card: [Model Name]

*Replace brackets with your information*

## Model Details

### Basic Information
- **Model Name**: [Full name]
- **Model Version**: [e.g., 1.0.0]
- **Model Date**: [Release date]
- **Model Type**: [e.g., Neural Network, Random Forest, Transformer, etc.]
- **Architecture**: [Specific architecture details]

### Developers and Contact
- **Developed by**: [Organization/Individuals]
- **Contact**: [Email or website]
- **License**: [Model license]
- **Citation**: [How to cite this model]

### Resources
- **Model Repository**: [GitHub/HuggingFace/Other URL]
- **Paper/Documentation**: [Publication or detailed docs]
- **Demo**: [Link to demo if available]

## Intended Use

### Primary Intended Uses
[Describe the primary use cases for which the model was designed]

**Examples**:
- Research on trauma-informed therapeutic approaches
- Analyzing patterns in mental health treatment responses
- Educational demonstrations of ethical AI

### Primary Intended Users
[Describe the intended users]

**Examples**:
- Mental health researchers
- AI safety researchers
- Healthcare professionals (with appropriate disclaimers)
- Educators in AI ethics

### Out-of-Scope Use Cases
[List uses that are NOT appropriate]

**Examples**:
- Clinical diagnosis or treatment decisions without human oversight
- Automated mental health crisis response
- Surveillance or monitoring
- Marketing or advertising
- Any use that violates Hollow House Institute AI Safety Policy

## Training Data

### Datasets Used
- **Primary Dataset**: [Name and version from Hollow House Institute]
- **Additional Datasets**: [Any supplementary data]
- **Training Data Size**: [Number of samples/tokens/examples]

### Data Preprocessing
[Describe preprocessing steps]
- Filtering criteria
- Normalization methods
- Feature engineering
- Data augmentation

### Data Splits
- **Training**: [Percentage/size]
- **Validation**: [Percentage/size]
- **Test**: [Percentage/size]

### Known Data Limitations
[Limitations from the source datasets]
- Demographic representation gaps
- Temporal coverage
- Geographic bias
- Selection bias
- Other limitations

## Model Architecture and Training

### Architecture Details
[Describe model architecture]
- Number of parameters
- Layer structure
- Attention mechanisms (if applicable)
- Input/output formats

### Training Procedure
**Hyperparameters**:
- Learning rate: [value]
- Batch size: [value]
- Epochs: [value]
- Optimizer: [type and settings]
- Loss function: [type]

**Training Environment**:
- Hardware: [GPU/TPU details]
- Framework: [TensorFlow, PyTorch, etc.]
- Training time: [approximate duration]

**Training Process**:
- [Describe training process, stopping criteria, checkpointing]

## Evaluation

### Evaluation Data
- **Dataset**: [Name and version]
- **Size**: [Number of examples]
- **Difference from training data**: [If evaluation data differs]

### Metrics
[List all evaluation metrics used]

| Metric | Value | Notes |
|--------|-------|-------|
| Accuracy | [value] | [context] |
| Precision | [value] | [context] |
| Recall | [value] | [context] |
| F1 Score | [value] | [context] |
| [Custom Metric] | [value] | [context] |

### Disaggregated Performance
[Performance across different subgroups]

**By Demographic Category**:
| Group | Metric | Value | Notes |
|-------|--------|-------|-------|
| [Group 1] | [Metric] | [Value] | [Notes] |
| [Group 2] | [Metric] | [Value] | [Notes] |

**By Other Relevant Categories**:
- Severity levels
- Condition types
- Treatment modalities
- Other relevant breakdowns

### Performance Variability
- **Confidence intervals**: [If available]
- **Multiple runs**: [Statistics from multiple training runs]
- **Statistical significance**: [Tests performed]

## Ethical Considerations

### Bias Analysis
[Results of bias testing]

**Tested for**:
- Demographic bias (age, gender, ethnicity, etc.)
- Socioeconomic bias
- Geographic bias
- Temporal bias
- [Other relevant biases]

**Findings**:
[Describe any identified biases and their magnitude]

**Mitigation Strategies**:
[Steps taken to address biases]

### Fairness Evaluation
[Fairness metrics and evaluation]

- **Equalized odds**: [value]
- **Demographic parity**: [value]
- **Equal opportunity**: [value]
- [Other fairness metrics]

### Privacy Considerations
- **Training data privacy**: [How privacy is protected]
- **Model privacy**: [Potential privacy leakage risks]
- **Membership inference risk**: [If evaluated]
- **Differential privacy**: [If applied, parameters]

### Harm Assessment
[Potential harms and mitigation]

**Potential Harms**:
- [Type of harm and likelihood]
- [Type of harm and likelihood]

**Mitigation Strategies**:
- [Safeguard 1]
- [Safeguard 2]

**Residual Risks**:
- [Risks that cannot be fully mitigated]

## Limitations and Recommendations

### Known Limitations
[Technical and ethical limitations]

**Technical Limitations**:
- [Limitation 1]
- [Limitation 2]

**Contextual Limitations**:
- [When model may not work well]
- [Edge cases or outliers]

**Ethical Limitations**:
- [Ethical considerations or constraints]

### Recommendations for Use

**Do's**:
- [Recommended practice 1]
- [Recommended practice 2]

**Don'ts**:
- [Practice to avoid 1]
- [Practice to avoid 2]

**Best Practices**:
- Human oversight required for [specific scenarios]
- Regular monitoring for [specific metrics]
- User consent and transparency requirements
- Incident response procedures

### Failure Modes
[How the model fails and what to do]

**Common Failure Patterns**:
- [Failure type and frequency]
- [Failure type and frequency]

**Failure Detection**:
- [How to detect failures]

**Failure Response**:
- [What to do when failures occur]

## Safety and Monitoring

### Safety Testing
[Safety evaluation procedures performed]

**Red Team Testing**:
- [Adversarial scenarios tested]
- [Results and responses]

**Edge Case Testing**:
- [Unusual inputs tested]
- [Model behavior]

**Stress Testing**:
- [Load and performance testing]

### Deployment Considerations

**Requirements**:
- Minimum hardware specifications
- Latency requirements
- Throughput capabilities
- Dependencies

**Monitoring Plan**:
- Metrics to track in production
- Alerting thresholds
- Re-evaluation schedule
- Update procedures

**Incident Response**:
- How to report issues
- Escalation procedures
- Rollback plans

### Continuous Evaluation
- **Re-evaluation schedule**: [How often model is re-evaluated]
- **Performance monitoring**: [Ongoing metrics tracking]
- **Drift detection**: [Methods for detecting distribution drift]
- **Update policy**: [When and how model is updated]

## Use Case Examples

### Example 1: [Use Case Name]
**Context**: [Describe the scenario]  
**Input**: [Example input]  
**Output**: [Example output]  
**Interpretation**: [How to interpret the output]  
**Precautions**: [Specific considerations for this use]

### Example 2: [Use Case Name]
[Repeat structure]

### Example 3: [Anti-Pattern - What NOT to Do]
**Context**: [Describe inappropriate use]  
**Why It's Problematic**: [Explain the issues]  
**Alternative**: [Suggest proper approach]

## Changelog and Versioning

### Version History

**Version [X.Y.Z]** - [Date]
- [Changes made]
- [Performance impacts]
- [Breaking changes if any]

**Version [X.Y.Z-1]** - [Date]
- [Changes made]

### Deprecation Policy
[How long versions are supported, migration guidance]

## References and Citations

### How to Cite This Model
```
[Formatted citation]
```

### Related Publications
- [Publication 1]
- [Publication 2]

### Dataset Citation
```
[Citation for Hollow House Institute dataset(s) used]
```

### Acknowledgments
[Funding sources, contributors, data providers, etc.]

## Appendix

### Additional Technical Details
[Supplementary technical information]

### Glossary
[Definitions of technical terms]

### Frequently Asked Questions
**Q**: [Question]  
**A**: [Answer]

---

## Model Card Completion Checklist

Before finalizing your model card, verify:

- [ ] All sections completed with specific information (no brackets remaining)
- [ ] Performance metrics reported with appropriate context
- [ ] Disaggregated performance analysis included
- [ ] Bias and fairness evaluation documented
- [ ] Limitations clearly stated
- [ ] Safety considerations addressed
- [ ] Prohibited uses specified
- [ ] Dataset properly cited
- [ ] Contact information provided
- [ ] Version number and date included
- [ ] Examples of appropriate and inappropriate uses included
- [ ] Monitoring and maintenance plan described

## Questions?

For questions about completing this template:
- Technical questions: support@hollowhouseinstitute.org
- Ethical review: ethics@hollowhouseinstitute.org
- General questions: info@hollowhouseinstitute.org

## Additional Resources

- Mitchell et al. (2019): https://arxiv.org/abs/1810.03993
- Google Model Cards: https://modelcards.withgoogle.com/
- Hugging Face Model Cards: https://huggingface.co/docs/hub/model-cards
- Hollow House Institute AI Safety Policy: [link]

---

**Note**: This template is provided as a starting point. Adapt sections as appropriate for your specific model while maintaining the core transparency and safety principles.

**Template Version**: 1.0-DRAFT  
**Last Updated**: 2025-12-02  
**Based on**: Mitchell et al. (2019) Model Cards for Model Reporting
