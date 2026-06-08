# ISTQB Testing Roles Mindmap

## Overview
This mindmap illustrates the key roles and responsibilities in Software Testing based on the ISTQB (International Software Testing Qualifications Board) framework.

> **Note on QA vs QC:** ISTQB Foundation Level (CTFL 4.0) does not define "QA Role" or "QC Role" as formal certification roles. Instead, it defines **Test Management Role** and **Testing Role**. QA (Quality Assurance) and QC (Quality Control) are **quality concepts** — QA focuses on **process & prevention**, while QC focuses on **product & detection**. They are complementary and are embedded within the roles below, not standalone ISTQB roles.

---

## Mindmap

```mermaid
mindmap
  root((ISTQB QA/QC Roles))
    QA - Quality Assurance
      Process & Methodology
        ISTQB Foundation Level
        Test Process Improvement
        Risk-Based Testing
        Test Strategy Development
      Prevention Focus
        Test Planning
        Test Process Definition
        Test Policy Creation
        Quality Metrics Definition
      Team & Training
        Tester Competency Development
        Test Tool Selection
        Test Process Documentation
        Defect Prevention

    QC - Quality Control
      Execution & Validation
        Test Case Design
        Test Data Preparation
        Test Execution
        Defect Reporting
      Verification Focus
        Unit Testing
        Integration Testing
        System Testing
      Validation Focus
        User Acceptance Testing (UAT)
        Field Testing
        Beta Testing
      Product Focus
        Bug Detection
        Test Reporting
        Test Result Analysis
        Test Exit Criteria

    Test Manager
      Leadership
        Test Plan Approval
        Resource Management
        Schedule Management
        Stakeholder Communication
      Strategic
        Test Effort Estimation
        Test Strategy Selection
        QA vs QC Balance
        ROI Calculation

    Test Analyst
      Analysis
        Requirements Analysis
        Test Condition Identification
        Traceability Matrix Creation
        Test Scenario Design
      Design
        Test Case Specification
        Test Data Requirements
        Test Environment Setup
        Test Data Preparation

    Test Automation Engineer
      Framework
        Test Automation Architecture
        Framework Selection
        Test Library Development
        CI/CD Integration
      Execution
        Automated Test Execution
        Test Maintenance
        Test Reporting
        Tool Evaluation

    Test Environment Manager
      Infrastructure
        Test Environment Setup
        Test Data Management
        Environment Monitoring
        Environment Troubleshooting
      Support
        Access Control
        Environment Backup
        Performance Optimization
        Virtualization Management

    CTFL - Certified Tester Foundation Level
      Core Knowledge Areas
        Fundamentals of Testing
        Testing Throughout the SDLC
        Static Testing Techniques
        Test Design Techniques
        Test Management
        Tool Support for Testing
      Competencies
        Black Box Testing
        White Box Testing
        Experience-Based Testing
        Risk-Based Testing

    CTAL - Certified Tester Advanced Level
      Test Manager Track
        Risk Management
        Test Planning & Estimation
        Test Monitoring & Control
        Test Selection & Strategy
        Test Process Improvement
      Test Analyst Track
        Test Design Techniques
        Requirements-Based Testing
        Risk-Based Testing
        Defect Prevention
        Industry Standards Compliance
      Technical Test Analyst Track
        Test Architecture Design
        Performance Testing
        Security Testing
        Test Automation Strategy
```

---

## Role Summary Table

| Role | Focus | Key Responsibilities | ISTQB Level |
|------|-------|---------------------|-------------|
| **Test Manager** | Strategy & Leadership | Test planning, resource management, stakeholder management | Advanced |
| **Test Analyst** | Design & Analysis | Requirements analysis, test case design, traceability | Foundation / Advanced |
| **Test Automation Engineer** | Tool & Automation | Framework development, script creation, CI/CD | Specialist |
| **Test Environment Manager** | Infrastructure | Environment setup, data management, monitoring | Support Role |
| **Technical Test Analyst** | Architecture & Non-Functional | Test architecture, performance, security, automation strategy | Advanced |

---

## QA vs QC Comparison

| Aspect | QA (Quality Assurance) | QC (Quality Control) |
|--------|----------------------|---------------------|
| **Focus** | Process & Prevention | Product & Detection |
| **Goal** | Prevent defects | Find and report defects |
| **Approach** | Proactive | Reactive |
| **Activities** | Process improvement, standards | Testing, inspection, review |
| **When** | Throughout lifecycle | During execution phase |
| **Output** | Process documentation, metrics | Test reports, defect logs |

---

## ISTQB Certification Pathway

```
Foundation Level (CTFL)
├── Entry point for all testers
├── 40 hours study recommended
└── Valid for life (no expiry)

    ├── Advanced Level (CTAL)
    │   ├── Test Manager
    │   ├── Test Analyst
    │   └── Technical Test Analyst
    │
    └── Specialist Certifications
        ├── Test Automation Engineer
        ├── Agile Tester
        ├── Security Tester
        └── Performance Tester
```

---

## Key Takeaways

- **ISTQB defines two primary roles:** Test Management Role and Testing Role — not "QA" or "QC" as standalone roles
- **QA** (process & prevention) and **QC** (product & detection) are quality concepts embedded within testing roles, not separate ISTQB-certified roles
- **Verification** ("building the product right") applies to unit, integration, and system testing
- **Validation** ("building the right product") is the primary goal of UAT and acceptance testing
- ISTQB provides a **structured certification pathway** from Foundation to Expert level
- The **Test Manager** oversees testing activities; the **Test Analyst** focuses on test analysis and design
- **Test Automation** is a specialized role within the testing framework