---
author: "Hollow House Institute"
last_updated: "2025-12-02"
status: "DRAFT"
---

# Dataset Card Template

## Purpose

This template guides the creation of comprehensive dataset documentation following best practices for transparency, ethics, and responsible use. All Hollow House Institute datasets must include a completed dataset card.

Based on: Gebru et al. (2021) "Datasheets for Datasets"

---

# Dataset Card: [Dataset Name]

*Replace all bracketed sections with your specific information*

## Dataset Description

### Basic Information
- **Dataset Name**: [Full name]
- **Dataset Version**: [e.g., 1.0.0]
- **Release Date**: [Date]
- **Dataset ID**: [Unique identifier, e.g., HHI-TIMH-001]
- **License**: [License type and link]
- **DOI**: [If available]

### Point of Contact
- **Maintainer**: [Organization/Individual]
- **Email**: [Contact email]
- **Website**: [Dataset webpage]

### Citation
```
[Formatted citation for this dataset]
```

## Motivation

### Purpose
[Why was this dataset created?]

**Primary Goals**:
- [Goal 1]
- [Goal 2]

**Intended Research Areas**:
- [Area 1]
- [Area 2]

### Funding
- **Funded by**: [Funding sources]
- **Grant numbers**: [If applicable]

### Creators
- **Organization**: [Creating organization]
- **Contributors**: [Key contributors and their roles]
- **Acknowledgments**: [Others to acknowledge]

## Dataset Composition

### Overview
- **Total Size**: [Number of records/samples]
- **Data Types**: [Text, numeric, categorical, etc.]
- **Format**: [CSV, JSON, Parquet, etc.]
- **File Size**: [Storage size]

### Instance Breakdown
[Describe what each instance/row represents]

**Example**: Each row represents a single anonymized therapeutic session summary with associated metadata.

**Count**: [Number of instances]

### Data Fields

| Field Name | Data Type | Description | Example Values | Missing % |
|------------|-----------|-------------|----------------|-----------|
| [field_1] | [type] | [description] | [examples] | [%] |
| [field_2] | [type] | [description] | [examples] | [%] |
| [field_3] | [type] | [description] | [examples] | [%] |

### Labels/Targets
[If applicable, describe label distribution]

| Label | Count | Percentage |
|-------|-------|------------|
| [label_1] | [count] | [%] |
| [label_2] | [count] | [%] |

**Label Definition**: [How labels were determined]

**Label Quality**: [Inter-annotator agreement, validation methods]

### Missing Data
- **Overall Missing**: [Percentage of missing values]
- **Patterns**: [Systematic missing data patterns]
- **Handling**: [How missing data should be handled]

### Data Splits
[If pre-split]

- **Training**: [% or count]
- **Validation**: [% or count]
- **Test**: [% or count]

**Split Methodology**: [How splits were created]

### Data Quality

**Quality Assurance**:
- [QA step 1]
- [QA step 2]

**Known Issues**:
- [Issue 1]
- [Issue 2]

## Collection Process

### Source Data
[Where did the data come from?]

**Origins**:
- [Source 1 with description]
- [Source 2 with description]

**Collection Methods**:
- [Method 1]
- [Method 2]

**Collection Period**: [Date range]

### Data Collection

**Who collected the data?**
- [Collectors and their qualifications]

**Collection Procedures**:
- [Procedure 1]
- [Procedure 2]

**Quality Control**:
- [QC measure 1]
- [QC measure 2]

### Sampling Strategy
- **Target Population**: [Description]
- **Sampling Method**: [Random, stratified, convenience, etc.]
- **Sample Size Determination**: [How size was chosen]
- **Response/Participation Rate**: [If applicable]

### Ethical Review
- **IRB Approval**: [Yes/No and details]
- **Ethics Board**: [Institution/Organization]
- **Approval Number**: [Reference number]
- **Review Date**: [Date]

## Preprocessing and Anonymization

### Preprocessing Steps
[Describe all preprocessing performed]

1. [Step 1]
2. [Step 2]
3. [Step 3]

**Tools Used**: [Software/scripts]

### Anonymization

**Methods Applied**:
- Direct identifier removal
- K-anonymity (k=[value])
- L-diversity (l=[value])
- Differential privacy (ε=[value], if applicable)
- [Other methods]

**Removed/Modified Fields**:
- [Field 1 - how handled]
- [Field 2 - how handled]

**Generalization Applied**:
- [Field 1 - generalization method]
- [Field 2 - generalization method]

**Validation**:
- [Validation method 1]
- [Validation method 2]

**See Also**: [Anonymization Protocol](./anonymization_protocol.md)

### Data Transformations
[Additional transformations beyond anonymization]

- **Normalization**: [Methods used]
- **Encoding**: [Categorical encoding, etc.]
- **Feature Engineering**: [New features created]
- **Excluded Data**: [What was excluded and why]

## Dataset Characteristics

### Demographics
[If applicable, demographic breakdowns]

**Age Distribution**:
| Age Range | Count | Percentage |
|-----------|-------|------------|
| [range] | [count] | [%] |

**Gender Distribution**:
| Gender | Count | Percentage |
|--------|-------|------------|
| [category] | [count] | [%] |

**Geographic Distribution**:
| Region | Count | Percentage |
|--------|-------|------------|
| [region] | [count] | [%] |

**Other Relevant Demographics**:
[As appropriate for the dataset]

### Representativeness
[How well does this dataset represent the target population?]

**Strengths**:
- [Strength 1]
- [Strength 2]

**Limitations**:
- [Underrepresented group 1]
- [Underrepresented group 2]

**Known Biases**:
- [Bias 1 and its source]
- [Bias 2 and its source]

## Use Cases

### Intended Use Cases
[Specific applications this dataset was designed for]

1. **[Use Case 1]**
   - Description: [Details]
   - Requirements: [What users need]
   - Example: [Concrete example]

2. **[Use Case 2]**
   - Description: [Details]
   - Requirements: [What users need]
   - Example: [Concrete example]

### Proven Applications
[If dataset has been used successfully]

- [Published work 1]
- [Published work 2]

### Discouraged Use Cases
[Uses that are not recommended]

- [Use case 1] - Reason: [Why not recommended]
- [Use case 2] - Reason: [Why not recommended]

### Prohibited Use Cases
[Explicitly forbidden uses per AI Safety Policy]

- **Weapons/Surveillance**: [Specific prohibitions]
- **Manipulation**: [Specific prohibitions]
- **Discrimination**: [Specific prohibitions]
- **Re-identification**: Attempting to identify individuals
- [Other prohibited uses]

See: [AI Safety Policy](./ai_safety_policy.md)

## Limitations

### Data Limitations

**Scope Limitations**:
- [What the dataset doesn't cover]
- [Temporal limitations]
- [Geographic limitations]

**Quality Limitations**:
- [Measurement error]
- [Annotation errors]
- [Inconsistencies]

**Technical Limitations**:
- [Format constraints]
- [Size constraints]
- [Compatibility issues]

### Methodological Limitations

**Sampling Limitations**:
- [Selection bias]
- [Non-response bias]
- [Coverage gaps]

**Collection Limitations**:
- [Measurement bias]
- [Recall bias]
- [Social desirability bias]

### Generalization Limitations
[To what populations/contexts does this dataset NOT generalize?]

- [Population 1] - Reason: [Why]
- [Context 1] - Reason: [Why]

### Privacy-Utility Trade-offs
[What was lost in anonymization?]

- [Trade-off 1]
- [Trade-off 2]

**Not Possible with This Dataset**:
- [Analysis 1 - why not possible]
- [Analysis 2 - why not possible]

## Ethical Considerations

### Informed Consent
- **Consent Obtained**: [Yes/No/Waived with justification]
- **Consent Scope**: [What participants consented to]
- **Withdrawal Process**: [How participants can withdraw]
- **Re-contact**: [Whether participants can be re-contacted]

### Vulnerable Populations
[If applicable]

- **Populations Included**: [Description]
- **Additional Protections**: [Extra safeguards taken]
- **Special Considerations**: [What users should know]

### Potential Harms

**To Participants**:
- Risk: [Potential harm]
- Mitigation: [How it's addressed]

**To Users**:
- Risk: [Potential harm]
- Mitigation: [How it's addressed]

**To Society**:
- Risk: [Potential harm]
- Mitigation: [How it's addressed]

### Sensitive Content
- **Content Warnings**: [If dataset contains sensitive material]
- **Trauma Considerations**: [Trauma-informed handling recommendations]
- **Recommended Precautions**: [For working with this data]

### Bias and Fairness

**Known Biases**:
| Bias Type | Description | Magnitude | Source |
|-----------|-------------|-----------|--------|
| [type] | [description] | [low/med/high] | [source] |

**Fairness Considerations**:
- [Consideration 1]
- [Consideration 2]

**Recommended Bias Mitigation**:
- [Strategy 1]
- [Strategy 2]

## Access and Distribution

### Access Requirements
- **Access Tier**: [Tier 1/2/3]
- **Application Required**: [Yes/No]
- **Prerequisites**: [What's needed for access]
- **Review Time**: [Expected wait time]

See: [Access and Pricing](./access_and_pricing.md)

### License Terms
- **License Type**: [Specific license]
- **Commercial Use**: [Permitted/Prohibited/Restricted]
- **Attribution**: [Requirements]
- **Redistribution**: [Terms]

See: [Licensing](./licensing.md)

### Access Instructions

**How to Access**:
1. [Step 1]
2. [Step 2]
3. [Step 3]

**Download Size**: [Size]  
**Format Options**: [Available formats]

### Versioning
- **Current Version**: [Version number]
- **Version History**: [Link or summary]
- **Update Schedule**: [How often updated]
- **Deprecation Policy**: [How long supported]

## Maintenance and Support

### Maintenance Plan
- **Maintained by**: [Team/person]
- **Update Frequency**: [Schedule]
- **Bug Fixes**: [How reported and addressed]
- **Issue Tracking**: [Where to report issues]

### Support Resources

**Documentation**:
- [Link to detailed documentation]
- [Link to tutorials]
- [Link to example code]

**Community**:
- [Forum/discussion group]
- [Mailing list]

**Direct Support**:
- Email: [support email]
- Response time: [Expected response time]

### Contribution Guidelines
[If community contributions accepted]
- [How to contribute]
- [Review process]
- [Contributor agreement]

## Related Resources

### Related Datasets
- [Dataset 1] - Relationship: [How related]
- [Dataset 2] - Relationship: [How related]

### Related Publications
- [Publication 1]
- [Publication 2]

### Code and Tools
- [Repository with example code]
- [Analysis toolkit]
- [Visualization tools]

### Additional Documentation
- [Model Card Template](./model_card_template.md)
- [Ethics and Limits](./ethics_and_limits.md)
- [Anonymization Protocol](./anonymization_protocol.md)

## Changelog

### Version [X.Y.Z] - [Date]
**Added**:
- [Addition 1]

**Changed**:
- [Change 1]

**Fixed**:
- [Fix 1]

**Removed**:
- [Removal 1]

### Version [X.Y.Z-1] - [Date]
[Earlier version changes]

## Appendix

### Variable Codebook
[Detailed variable descriptions if not fully covered above]

### Glossary
[Definitions of domain-specific terms]

| Term | Definition |
|------|------------|
| [term] | [definition] |

### Frequently Asked Questions

**Q: [Common question]**  
A: [Answer]

**Q: [Common question]**  
A: [Answer]

### Statistical Summary
[Additional statistical descriptions]

**Descriptive Statistics**:
[Summary tables]

**Correlation Analysis**:
[Key correlations]

---

## Dataset Card Completion Checklist

Before publishing your dataset card:

- [ ] All sections completed (no brackets remaining)
- [ ] Basic information filled (name, version, date, contact)
- [ ] Dataset composition fully described
- [ ] Collection process documented
- [ ] Anonymization methods detailed
- [ ] Demographics and representativeness described
- [ ] Intended and prohibited uses specified
- [ ] Limitations clearly stated
- [ ] Ethical considerations addressed
- [ ] Known biases documented
- [ ] Access instructions provided
- [ ] License information included
- [ ] Maintenance plan described
- [ ] Contact information provided
- [ ] Examples of appropriate use included
- [ ] Peer review completed (if applicable)

## Questions?

For assistance completing this template:
- Template questions: documentation@hollowhouseinstitute.org
- Technical content: support@hollowhouseinstitute.org
- Ethical review: ethics@hollowhouseinstitute.org

## Additional Resources

- Gebru et al. (2021): https://arxiv.org/abs/1803.09010
- Google Dataset Cards: https://research.google/resources/datasets/
- Hugging Face Dataset Cards: https://huggingface.co/docs/hub/datasets-cards
- Hollow House Dataset Standards: [internal link]

---

**Note**: This template is comprehensive by design. Not all sections may apply to every dataset. Remove or mark N/A for non-applicable sections while maintaining transparency about limitations and constraints.

**Template Version**: 1.0-DRAFT  
**Last Updated**: 2025-12-02  
**Based on**: Gebru et al. (2021) Datasheets for Datasets
