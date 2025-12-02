# Repository Scaffold Documentation

## Overview

This document describes the repository scaffold created for Hollow House Institute. The scaffold provides essential community health files, templates, and automation that make the repository professional, welcoming, and well-organized.

## Created Files and Their Purpose

### Community Health Files

#### `.gitignore`
- **Purpose**: Prevents tracking of temporary files, build artifacts, and sensitive data
- **Includes**: OS files, IDE configs, Python/Node/R artifacts, environment variables, logs, large data files
- **Why it matters**: Keeps the repository clean and prevents accidental commits of secrets

#### `CONTRIBUTING.md`
- **Purpose**: Guidelines for contributing to the project
- **Features**:
  - Trauma-informed contribution values
  - How to report issues and suggest enhancements
  - Pull request guidelines
  - Coding standards and documentation requirements
  - Licensing and attribution requirements
- **Why it matters**: Sets clear expectations and makes it easy for others to contribute

#### `CODE_OF_CONDUCT.md`
- **Purpose**: Establishes behavioral standards for the community
- **Features**:
  - Trauma-informed principles
  - Nervous-system safety emphasis
  - Clear enforcement guidelines
  - Relational repair processes
- **Why it matters**: Creates a safe, respectful environment aligned with project values

#### `SECURITY.md`
- **Purpose**: Security policy and vulnerability reporting procedures
- **Features**:
  - How to report vulnerabilities privately
  - Response timelines by severity
  - Data privacy considerations
  - Ethical compliance guidelines
  - Security best practices
- **Why it matters**: Protects the project and community from security risks

#### `CHANGELOG.md`
- **Purpose**: Tracks all notable changes to the project
- **Features**:
  - Follows Keep a Changelog format
  - Semantic versioning
  - Categorized changes (Added, Changed, Fixed, etc.)
- **Why it matters**: Provides transparency and helps users understand what's changed

### GitHub-Specific Files

#### `.github/ISSUE_TEMPLATE/`

Four comprehensive issue templates:

1. **`bug_report.yml`**
   - Structured form for reporting bugs
   - Includes environment, reproduction steps, expected vs actual behavior
   - Pre-submission checklist

2. **`feature_request.yml`**
   - Structured form for suggesting features
   - Includes use cases, priority, ethical considerations
   - Category and impact assessment

3. **`question.yml`**
   - Form for asking questions
   - Categories for different question types
   - Helps users get better answers

4. **`documentation.yml`**
   - Form for documentation issues
   - Types of documentation problems
   - Location, impact, and priority

5. **`config.yml`**
   - Configuration for issue templates
   - Links to documentation and community resources
   - Security vulnerability reporting instructions

#### `.github/PULL_REQUEST_TEMPLATE.md`
- **Purpose**: Standardizes pull request submissions
- **Features**:
  - Type of change checkboxes
  - Testing requirements
  - Documentation requirements
  - Ethical considerations checklist
  - Licensing confirmation
  - Reviewer checklist
- **Why it matters**: Ensures thorough, consistent PR submissions

#### `.github/FUNDING.yml`
- **Purpose**: Placeholder for funding/sponsorship information
- **Features**: Commented-out sections for various platforms (GitHub Sponsors, Patreon, etc.)
- **Why it matters**: Makes it easy to add funding options later

#### `.github/workflows/`

Two GitHub Actions workflows:

1. **`markdown-lint.yml`**
   - Automatically checks Markdown files for formatting issues
   - Runs on PRs and pushes to main
   - Helps maintain documentation quality

2. **`link-checker.yml`**
   - Automatically checks for broken links in documentation
   - Runs on PRs, pushes, and weekly schedule
   - Helps maintain documentation accuracy

## File Structure

```
Hollow_House_Institute/
├── .github/
│   ├── FUNDING.yml
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.yml
│   │   ├── config.yml
│   │   ├── documentation.yml
│   │   ├── feature_request.yml
│   │   └── question.yml
│   ├── PULL_REQUEST_TEMPLATE.md
│   ├── REPOSITORY_SCAFFOLD.md (this file)
│   └── workflows/
│       ├── link-checker.yml
│       └── markdown-lint.yml
├── .gitignore
├── CHANGELOG.md
├── CITATION.cff (existing)
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE.md (existing)
├── LICENSE.txt (existing)
├── README.md (existing)
├── SECURITY.md
└── dataset_license (existing)
```

## Key Features

### 1. Trauma-Informed Approach
All community health files incorporate nervous-system safety principles and trauma-informed practices, aligning with Hollow House Institute's core values.

### 2. Attribution and Sovereignty
Every file properly acknowledges Amy Pierce Bui as the founder and principal architect, respecting the intellectual and emotional labor embedded in this work.

### 3. Ethical Compliance
Templates include ethical consideration checkboxes and guidelines, ensuring all contributions align with the project's ethical framework.

### 4. Professional Standards
Follows GitHub best practices and industry standards for open-source projects, making the repository enterprise-ready.

### 5. Automation
GitHub Actions workflows automate quality checks, reducing manual work and maintaining consistency.

## How to Use

### For Contributors
1. Read `CONTRIBUTING.md` before making any contributions
2. Follow the `CODE_OF_CONDUCT.md` in all interactions
3. Use the appropriate issue template when reporting issues
4. Follow the pull request template when submitting changes

### For Maintainers
1. Review and customize funding options in `FUNDING.yml` as needed
2. Update `CHANGELOG.md` with each release
3. Respond to security reports following `SECURITY.md` guidelines
4. Enforce the Code of Conduct consistently

### For Users
1. Use issue templates to report bugs or request features
2. Check `SECURITY.md` if you discover a vulnerability
3. Review `CHANGELOG.md` to see what's new

## Customization Options

While the scaffold is comprehensive, you may want to customize:

1. **Funding**: Update `.github/FUNDING.yml` with actual funding links
2. **Workflows**: Add more GitHub Actions for testing, deployment, etc.
3. **Templates**: Adjust issue/PR templates based on specific needs
4. **Gitignore**: Add project-specific patterns as needed

## Benefits

### For the Project
- Professional appearance
- Clear contribution process
- Automated quality checks
- Better issue organization
- Security vulnerability management

### For Contributors
- Clear guidelines
- Easy-to-use templates
- Welcoming environment
- Transparent processes

### For the Community
- Safe, respectful environment
- Trauma-informed practices
- Ethical standards
- Open communication

## Standards and Compliance

This scaffold adheres to:
- [GitHub Community Guidelines](https://docs.github.com/en/site-policy/github-terms/github-community-guidelines)
- [Open Source Guide](https://opensource.guide/) best practices
- [Keep a Changelog](https://keepachangelog.com/) format
- [Semantic Versioning](https://semver.org/) principles
- [Contributor Covenant](https://www.contributor-covenant.org/) (adapted with trauma-informed principles)

## Maintenance

### Regular Tasks
- Update `CHANGELOG.md` with each release
- Review and respond to issues/PRs using templates
- Monitor workflow runs for failures
- Update documentation as the project evolves

### Periodic Review
- Quarterly: Review and update community health files
- Annually: Review and update Code of Conduct and Security policy
- As needed: Add new issue templates or workflows

## Questions and Support

If you have questions about this repository scaffold:
- Open an issue using the "question" template
- Contact the project maintainers
- Review the documentation in each file

---

**Created by**: Amy Pierce Bui, Hollow House Institute  
**Date**: December 2024  
**License**: CC BY-NC-SA 4.0  
**Version**: 1.0
