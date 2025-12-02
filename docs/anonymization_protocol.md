---
author: "Hollow House Institute"
last_updated: "2025-12-02"
status: "DRAFT"
---

# Anonymization Protocol

## Overview

The Hollow House Institute employs rigorous anonymization procedures to protect research participant privacy while maintaining data utility for ethical research. This document details our multi-layered anonymization approach and technical standards.

## Guiding Principles

### Privacy by Design
- Privacy protection built into data collection and processing
- Proactive rather than reactive measures
- Default to maximum privacy protection
- End-to-end security throughout lifecycle

### Proportional De-identification
- Level of anonymization matched to data sensitivity
- Balance between privacy and research utility
- Conservative approach when uncertain
- Regular reassessment of adequacy

### Non-Reversibility
- Anonymization designed to be irreversible
- No "keys" or mapping tables maintained
- Prevents internal or external re-identification
- Technical and organizational safeguards

## Regulatory Compliance

Our protocol meets or exceeds:
- **HIPAA Safe Harbor Method** (45 CFR §164.514(b))
- **GDPR Anonymization Standards** (Recital 26, Article 4(5))
- **ISO 25237** - Health informatics - Pseudonymization
- **NIST Privacy Framework** - De-identification techniques

## Anonymization Stages

### Stage 1: Direct Identifier Removal

Complete removal of all direct identifiers:

**Personal Identifiers**:
- Full names
- Social Security Numbers
- Medical record numbers
- Account numbers
- License numbers
- Device identifiers (IP, MAC addresses)

**Contact Information**:
- Email addresses
- Phone numbers
- Fax numbers
- Physical addresses (street level)
- URLs and social media handles

**Biometric Data**:
- Photographs
- Fingerprints
- Voice recordings (unless anonymized)
- Facial recognition data
- Retinal scans

**Other Unique Identifiers**:
- Certificate/license numbers
- Vehicle identification numbers
- Passport numbers
- Any other unique identifying code

### Stage 2: Quasi-Identifier Generalization

Quasi-identifiers are generalized to prevent linkage attacks:

**Geographic Information**:
- Zip codes: First 3 digits only (if population >20,000)
- Cities: Generalized to county or region
- States/Countries: Retained
- Rare locations: Suppressed or generalized further

**Temporal Information**:
- Dates: Generalized to month/year or quarter
- Ages: Reported in ranges (e.g., 30-34, 35-39)
- Ages over 89: Grouped as "90+"
- Time stamps: Removed or generalized to day

**Demographic Information**:
- Rare occupations: Generalized to broader categories
- Small ethnic groups: Aggregated or suppressed
- Unusual combinations: Broken up or generalized
- Family relationships: Simplified or removed

**Medical Information**:
- Rare diagnoses: Generalized to broader categories
- Unusual procedures: Aggregated
- Extreme lab values: Top/bottom coded
- Genetic information: Special handling (usually excluded)

### Stage 3: K-Anonymity and L-Diversity

**K-Anonymity** (minimum k=5):
- Every combination of quasi-identifiers appears at least k times
- Prevents individual identification within dataset
- Higher k for sensitive data
- Verified through automated tooling

**L-Diversity** (minimum l=3):
- At least l diverse values for sensitive attributes
- Prevents attribute disclosure
- Applied to diagnosis, treatment, outcomes
- Prevents homogeneity attacks

**T-Closeness** (where applicable):
- Distribution of sensitive attributes similar to overall distribution
- Prevents skewness attacks
- Applied to highly sensitive fields

### Stage 4: Differential Privacy

For aggregate statistics and releases:

**Noise Injection**:
- Calibrated noise added to query results
- Privacy budget (ε) tracked and limited
- Balance between privacy and accuracy
- Documented privacy-loss bounds

**Parameters**:
- ε (epsilon): 0.1 to 1.0 depending on sensitivity
- δ (delta): < 1/n² where n is dataset size
- Query limits to prevent privacy budget exhaustion

### Stage 5: Narrative Sanitization

Free-text and narrative data requires special handling:

**Named Entity Recognition (NER)**:
- Automated detection of names, locations, organizations
- Manual review of flagged entities
- Replacement with generic tokens

**Pattern Matching**:
- Regex patterns for phone numbers, emails, SSNs
- Date and time patterns
- Address patterns
- Account numbers

**Manual Review**:
- Human review of all free-text
- Clinical expertise for medical narratives
- Contextual understanding to catch implicit identifiers
- Multiple reviewers for sensitive content

**Redaction/Replacement**:
- Replace names with "[NAME]" or generic alternatives
- Replace locations with "[CITY]" or regional descriptions
- Dates replaced with relative timeframes
- Context-preserving when possible

### Stage 6: Validation and Testing

**Automated Validation**:
- Verification that all direct identifiers removed
- K-anonymity compliance checking
- Pattern matching for missed identifiers
- Statistical disclosure control tests

**Manual Validation**:
- Expert review of random sample (minimum 5%)
- Domain expert review
- Privacy expert review
- Fresh eyes from uninvolved team member

**Re-identification Testing**:
- Simulated linkage attacks
- Public records matching attempts
- Online search for unique patterns
- Adversarial testing by security team

**Statistical Utility Testing**:
- Verification that data remains useful
- Comparison of distributions pre/post anonymization
- Validation of key relationships preserved
- Researcher feedback on usability

## Special Considerations

### Rare Conditions or Characteristics

For extremely rare conditions (prevalence <1:10,000):
- Evaluate inclusion carefully
- May require exclusion
- Alternative: Group with similar conditions
- Document limitations

### Longitudinal Data

Time-series data presents unique challenges:
- Trajectory itself can be identifying
- Temporal bucketing applied
- Limit length of observation periods
- Shuffle ordering where appropriate

### Linked Records

Related records (e.g., family members, treatment episodes):
- Break linkages or generalize relationships
- Pseudo-IDs for within-dataset linking only
- No persistent identifiers across datasets
- Document relationship structure limitations

### Small Sample Sizes

When n < 100:
- Enhanced anonymization required
- Higher k-anonymity threshold
- Greater generalization
- Consider not releasing

### Cross-Dataset Linkage Risk

When multiple datasets from same population:
- Evaluate combined disclosure risk
- Consistent anonymization approach
- Limit overlapping variables
- Stagger releases

## Technical Implementation

### Tools and Technologies

**Anonymization Tools**:
- ARX Data Anonymization Tool
- Microsoft Presidio
- Custom NLP pipelines
- Differential privacy libraries (Google DP, IBM Diffprivlib)

**Validation Tools**:
- Statistical disclosure control software
- Custom validation scripts
- Manual review protocols

**Infrastructure**:
- Secure processing environment (air-gapped)
- Access controls and audit logging
- Encrypted storage and transmission
- Secure deletion of source data

### Process Workflow

1. **Intake**: Source data received in secure environment
2. **Inventory**: Catalog all data elements and identify PII
3. **Classification**: Categorize by sensitivity and identifier type
4. **Processing**: Apply anonymization pipeline
5. **Validation**: Multi-stage validation process
6. **Review**: Expert review and approval
7. **Release**: Transfer to release environment
8. **Documentation**: Complete dataset card with limitations
9. **Monitoring**: Ongoing monitoring for disclosure risks
10. **Archival**: Secure archival and source data destruction

## Quality Assurance

### Validation Checklist

Before release, verify:
- [ ] All direct identifiers removed
- [ ] Quasi-identifiers adequately generalized
- [ ] K-anonymity threshold met (k≥5)
- [ ] L-diversity applied to sensitive attributes
- [ ] Free text manually reviewed
- [ ] Re-identification testing completed
- [ ] Privacy expert sign-off obtained
- [ ] Statistical utility validated
- [ ] Documentation complete
- [ ] Release notes include limitations

### Continuous Monitoring

Post-release:
- Monitor for re-identification attempts
- Track publications using data for issues
- Respond to reported concerns
- Update protocols based on lessons learned
- Annual re-evaluation of released datasets

## Known Limitations

Anonymization cannot eliminate all risks:

**Residual Risk**:
- Theoretical possibility of re-identification with sufficient auxiliary data
- Advances in re-identification techniques
- Unforeseen linkage possibilities

**Utility Trade-offs**:
- Generalization reduces data granularity
- Some analyses may not be possible
- Statistical power may be reduced
- Temporal resolution limited

**Cannot Protect Against**:
- Intentional violations by data users
- Sophisticated adversaries with extensive resources
- Future technologies or methods

## User Responsibilities

Dataset users must:
- **Never attempt re-identification**
- **Not link datasets** to identify individuals
- **Not use external data** for identification purposes
- **Report concerns** if identifiable information suspected
- **Follow all license terms** regarding data handling

Violations are grounds for immediate license termination and potential legal action.

## Transparency and Documentation

Each dataset includes:

**Anonymization Summary**:
- Methods applied
- Parameters used (k, l, ε values)
- Known limitations
- Residual risks

**Data Dictionary**:
- Variables included
- Generalization applied
- Suppression thresholds
- Value ranges

**Limitations Section**:
- Analyses not possible due to anonymization
- Known biases introduced
- Recommended cautions

## Updates and Revisions

Protocol updates occur:
- Annually as standard practice
- When new risks identified
- When better methods available
- When regulations change

Previously released datasets:
- Evaluated against updated standards
- Re-released if significant gaps identified
- Users notified of updates

## Research on Anonymization

We welcome research collaboration on:
- Improving anonymization techniques
- Better utility preservation
- Novel disclosure risk assessment
- Privacy-preserving analytics

Contact: research@hollowhouseinstitute.org

## Contact and Questions

**Privacy Questions**: privacy@hollowhouseinstitute.org  
**Technical Questions**: anonymization@hollowhouseinstitute.org  
**Report Concerns**: security@hollowhouseinstitute.org

## References

- Narayanan, A., & Shmatikov, V. (2008). Robust De-anonymization of Large Sparse Datasets. IEEE S&P.
- HIPAA Safe Harbor: https://www.hhs.gov/hipaa/for-professionals/privacy/special-topics/de-identification/index.html
- UK Anonymisation Network: https://ukanon.net/
- Article 29 Working Party Opinion on Anonymisation Techniques (WP216)
- NIST Privacy Framework: https://www.nist.gov/privacy-framework

---

**Note**: This protocol represents our current best practices and is continuously refined based on research advances and emerging threats. Feedback and suggestions welcome.

**Last Updated**: 2025-12-02  
**Next Review**: 2026-06-02  
**Version**: 1.0-DRAFT
