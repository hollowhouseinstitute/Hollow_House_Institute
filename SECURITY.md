# Security Policy

## Overview

Hollow House Institute is committed to maintaining the security and privacy of our research frameworks, datasets, and community members. This document outlines our security policies and procedures for reporting vulnerabilities.

## Supported Versions

We provide security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| 1.x     | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

### How to Report

If you discover a security vulnerability, please report it privately:

1. **GitHub Security Advisories** (Preferred):
   - Navigate to the repository's Security tab
   - Click "Report a vulnerability"
   - Provide detailed information about the vulnerability

2. **Direct Contact**:
   - Contact the project maintainers through GitHub
   - Use the subject line: "SECURITY: [Brief Description]"

### What to Include

When reporting a vulnerability, please include:

- **Type of vulnerability** (e.g., data exposure, authentication bypass, etc.)
- **Affected component(s)** (specific files, functions, or systems)
- **Steps to reproduce** the vulnerability
- **Potential impact** of the vulnerability
- **Suggested remediation** (if you have ideas)
- **Your contact information** for follow-up questions

### Response Timeline

- **Initial Response**: Within 48 hours of report
- **Status Update**: Within 7 days
- **Resolution Timeline**: Depends on severity (see below)

### Severity Levels

| Severity | Response Time | Description |
|----------|---------------|-------------|
| **Critical** | 24-48 hours | Immediate risk to data privacy, security, or ethical compliance |
| **High** | 3-5 days | Significant risk with potential for exploitation |
| **Medium** | 1-2 weeks | Moderate risk with limited impact |
| **Low** | 1 month | Minor issues with minimal impact |

## Security Considerations

### Data Privacy

Hollow House Institute handles sensitive research data related to:
- Human relational patterns
- Emotional and psychological data
- Nervous-system responses
- AI interaction logs

**We take data privacy extremely seriously.**

All data must be:
- Anonymized according to our [Anonymization Protocol](Docs/Anonymization%20Protocol.md)
- Stored securely with appropriate access controls
- Used only within the scope of ethical research guidelines
- Protected from unauthorized access or exploitation

### Licensing and Intellectual Property

**Security vulnerabilities related to licensing violations:**

Our work is licensed under **CC BY-NC-SA 4.0**. Violations include:
- Unauthorized commercial use
- Failure to provide attribution
- Removal of licensing information
- Misrepresentation of authorship

Such violations will result in:
- Immediate license termination
- Legal enforcement action
- Permanent ban from the project

### Ethical Compliance

Security in our context includes:
- **Trauma-informed practices**: Ensuring systems don't cause harm
- **Consent and autonomy**: Respecting participant sovereignty
- **Non-exploitation**: Preventing misuse of frameworks and data
- **Relational safety**: Maintaining nervous-system-aware interactions

## What We Do

Upon receiving a security report, we will:

1. **Acknowledge** receipt within 48 hours
2. **Assess** the vulnerability and its severity
3. **Investigate** and develop a fix
4. **Test** the fix thoroughly
5. **Deploy** the fix to supported versions
6. **Notify** affected users (if applicable)
7. **Credit** the reporter (with permission)
8. **Publish** a security advisory (if appropriate)

## What We Ask of You

If you discover a vulnerability:

- **Give us time** to fix it before public disclosure
- **Do not exploit** the vulnerability beyond what's necessary to demonstrate it
- **Do not access** or modify data that isn't yours
- **Act in good faith** and respect our community

## Public Disclosure

We follow **coordinated disclosure**:

- We work with reporters to address vulnerabilities
- We aim to fix critical issues within 90 days
- We credit reporters publicly (with permission)
- We publish advisories after fixes are deployed

## Security Best Practices

For contributors and users:

### For Developers
- Never commit secrets, API keys, or credentials
- Use `.gitignore` to exclude sensitive files
- Follow secure coding practices
- Keep dependencies updated
- Review code for security issues before committing

### For Researchers
- Follow the [Researcher Access Application](Docs/researcher_access_application.md) process
- Comply with all licensing terms
- Protect any data you access
- Report any suspicious activity
- Respect privacy and anonymization protocols

### For Users
- Keep your local environment secure
- Use strong authentication
- Don't share credentials
- Report suspicious behavior
- Follow ethical guidelines

## Compliance and Legal

Hollow House Institute operates under:
- **CC BY-NC-SA 4.0 License**: See `LICENSE.md`
- **Dataset License**: See `dataset_license`
- **AI Safety Policy**: See [Docs/ai_safety_policy.md](Docs/ai_safety_policy.md)
- **Ethics Guidelines**: See [Docs/ethics_limits.md](Docs/ethics_limits.md)

Violations of these policies are security issues and will be treated accordingly.

## Contact

For security concerns:
- Use GitHub Security Advisories (preferred)
- Open a private issue (mark as "security")
- Contact project maintainers directly

For general questions about our security practices, open a public issue with the "security" label.

## Acknowledgments

We appreciate the security research community's efforts to keep our project safe. Reporters who responsibly disclose vulnerabilities will be:
- Credited publicly (with permission)
- Acknowledged in release notes
- Added to our security acknowledgments

Thank you for helping keep Hollow House Institute secure!

---

**Version**: 1.0  
**Last Updated**: December 2024  
**Maintainer**: Amy Pierce Bui, Hollow House Institute  
**License**: CC BY-NC-SA 4.0
