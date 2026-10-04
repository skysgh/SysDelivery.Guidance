# Proposed New SELF Target Index

> DRY RUN ONLY - NO SOURCE FILE OR FOLDER HAS BEEN MOVED OR RENAMED

This document proposes where every current source folder will land. It deliberately permits variable semantic depth so that delivery work is exposed rather than compressed into conventional high-level SDLC labels.

## Governing rules

- Preserve every existing SELF concept unless a reviewed coverage matrix explicitly records a split, merge, replacement, or retirement.
- Use as many semantic levels as are required to expose distinct work, responsibility, risk, evidence, or artefacts.
- Do not add a folder merely for symmetry or to hold one file when its parent remains clear.
- Use one local two-digit decimal component in each physical folder name. Compose the canonical SELF identifier from the ordered path components.
- Give documents one local two-digit reading-order number such as `[10 - DRAFT]`.
- Put diagrams and images in `_media` without SELF, ordering, or state prefixes.
- Keep the complete absolute path below 220 characters by shortening repeated physical labels, not by deleting conceptual distinctions.
- Give each item one authoritative home and express cross-cutting relationships through links and indexes.


### Local folder numbers and canonical identifiers

Physical folder names contain only the local component:

```text
[60] Delivery/
└─ [40] Core Service/
   └─ [40] Registries and Work/
```

The path composes the canonical SELF identifier `60.40.40`. The index is the authority for that composed identifier. If a subtree is exported independently, its package name or included README must state the complete canonical identifier so that it can be reassembled without ambiguity.

## Coverage and feasibility

- Source folders represented: **483**
- Source files considered when determining folder destinations: **2021**
- Unmapped source files: **0**
- Distinct proposed semantic destination folders: **80**
- Existing numbered SELF entries represented in the coverage ledger: **525**
- Existing SELF identifiers occurring more than once: **88**
- Coherent source folders with one destination: **404**
- Mixed source folders requiring a controlled split: **79**
- Source folders containing at least one low-confidence placement: **51**
- Individual files requiring classification review: **215**
- Longest proposed absolute folder path: **120 characters**
- Proposed destination folders at 220 characters or longer: **0**

A `SPLIT` is not data loss. It means the existing source folder mixes concepts that will receive separate authoritative homes. The file-level dry-run must be reviewed before executing those splits.

## Proposed New SELF destination tree

```text
├─ [00] Management
│  ├─ [10] Repository
│  │  ├─ [10] Indexes and Navigation
│  │  └─ [20] Repository Guidance
│  ├─ [20] Governance
│  │  ├─ [10] Governance and Principles
│  │  ├─ [20] Decisions
│  │  ├─ [30] Reviews and Compliance
│  │  └─ [90] Existing Cross-Cutting Management
│  ├─ [30] Registers
│  │  ├─ [10] Risks
│  │  └─ [90] Existing Registers
│  └─ [90] Review
│     ├─ [10] Classification Required
│     ├─ [20] Temporary and Unsorted
│     └─ [30] Existing SELF Review
├─ [10] Strategy
│  ├─ [50] Direction
│  │  └─ [10] Direction Outcomes and Scope
│  └─ [90] Existing Strategy
│     └─ [10] Sensing and Framing
├─ [20] Investment
│  ├─ [10] Business Case
│  │  ├─ [10] Strategic Case
│  │  └─ [20] Economic Case
│  └─ [90] Existing Investment
│     └─ [10] Financing and Preparation
├─ [30] Discovery
│  ├─ [10] Context
│  │  ├─ [10] Business Context
│  │  ├─ [20] System Context
│  │  └─ [30] Scope Constraints and Dependencies
│  ├─ [30] Stakeholders
│  │  └─ [10] Stakeholders Personas and Journeys
│  ├─ [50] Requirements
│  │  ├─ [10] Business and User Requirements
│  │  └─ [30] Quality Requirements
│  └─ [90] Existing Definition
│     └─ [10] Context and Definition
├─ [40] Procurement
│  ├─ [10] Preparation
│  │  └─ [10] Approach and Requirements
│  ├─ [70] Contracting
│  │  └─ [10] Contracts and Obligations
│  └─ [90] Existing Procurement
│     └─ [10] Preparation and Selection
├─ [50] Design
│  ├─ [10] Architecture
│  │  ├─ [10] Architecture Direction
│  │  ├─ [20] Architecture Descriptions
│  │  └─ [30] Patterns and Principles
│  ├─ [20] Information
│  │  ├─ [10] Information Architecture
│  │  ├─ [30] Physical Models
│  │  └─ [30] Quality Metadata and Records
│  ├─ [30] Functionality
│  │  ├─ [10] Capabilities and Functions
│  │  ├─ [20] Workflows
│  │  └─ [30] Use Cases
│  ├─ [50] Assurance
│  │  ├─ [10] Security and Assurance Design
│  │  ├─ [20] Identity and Access Design
│  │  └─ [30] Privacy Design
│  ├─ [60] Technology
│  │  └─ [10] Platforms and Infrastructure
│  └─ [90] Existing Design
│     └─ [10] Solution Design Response
├─ [60] Delivery
│  ├─ [10] Enablement
│  │  ├─ [10] Resourcing Onboarding and Training
│  │  ├─ [20] Environments Access and Licensing
│  │  ├─ [30] Tools and Licensing
│  │  └─ [90] Delivery Preparation
│  ├─ [20] System of Delivery
│  │  ├─ [20] Artefacts and Packaging
│  │  ├─ [30] Pipelines and Automation
│  │  └─ [90] Existing Delivery Enablement
│  ├─ [30] Data and Content
│  │  ├─ [10] Schemas and Storage
│  │  └─ [30] Content Media and Localisation
│  ├─ [40] Core Service
│  │  ├─ [10] Components and Modules
│  │  ├─ [20] Configuration Storage and Caching
│  │  ├─ [30] Identity Access and Sessions
│  │  ├─ [40] Registries and Work
│  │  └─ [90] Development Requiring Detail
│  ├─ [50] Integrations
│  │  ├─ [10] APIs and Endpoints
│  │  ├─ [20] Messaging and Events
│  │  ├─ [30] External Services
│  │  ├─ [30] External and Secure Integrations
│  │  └─ [40] Interoperability and Discovery
│  ├─ [60] Client Applications
│  │  ├─ [10] Web and Client Applications
│  │  ├─ [20] Mobile Clients
│  │  └─ [30] User Interfaces
│  ├─ [70] Verification
│  │  ├─ [10] Component and System Testing
│  │  ├─ [30] Performance Testing
│  │  └─ [40] Security Testing
│  ├─ [80] Release and Deployment
│  │  ├─ [10] Release Management
│  │  ├─ [20] Deployment
│  │  └─ [30] Data Migration
│  └─ [90] Operational Enablement
│     ├─ [10] Logging and Telemetry
│     ├─ [20] Monitoring and Alerting
│     └─ [30] Diagnostics and Health
├─ [70] Transition
│  ├─ [10] Readiness
│  │  └─ [90] Existing Readiness Assessment
│  └─ [50] Transition
│     ├─ [10] Cutover and Stabilisation
│     └─ [90] Existing Service Transition
├─ [80] Operations
│  ├─ [10] Service
│  │  ├─ [10] Operation and Support
│  │  └─ [90] Existing Service Management
│  └─ [30] Maintenance
│     └─ [10] Change and Maintenance
└─ [90] Closure
   ├─ [10] Retirement
   │  ├─ [10] Planning and Exit
   │  └─ [90] Existing Closure and Exit
   └─ [30] Decommissioning
      └─ [20] Migration and Retention
```

## Existing SELF coverage ledger

Every numbered heading extracted from the existing SELF draft appears below, including duplicate identifiers. `PRESERVE` means the concept remains represented; `REVIEW DUPLICATE ID` means the concept is retained but its old identifier is not unique and must be repaired before migration.

| Existing ID | Existing concept | Proposed New SELF destination | Treatment |
|---|---|---|---|
| `01` | Cross Cutting Management | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.1` | Cross-Cutting Governance | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.1.1` | Preparation | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.2` | Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.1.2.1` | Service Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.1.2.2` | Support Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.2.3` | Delivery Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.2.4` | Solution Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.2.5` | Enterprise Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.2.6` | Integration Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.2.7` | Data Principles | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.3` | Reviews | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.3.1` | Architectural Reviews | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.1.2` | Logs | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.1.2.1` | Decision Log | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.1.2` | Registries | `[00] Management / [30] Registers / [90] Existing Registers` | REVIEW DUPLICATE ID |
| `01.1.2.01` | Privacy Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.1.2.02` | Security Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.1.2.03` | Accessibility Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.1.2.04` | Risk Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.1.2.05` | Compliance Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.1.2.06` | Issue Register | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.1.2.07` | Contact Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2` | Cross-Cutting Management (Aspect) | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.2.01` | Preparation | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.2.01.01` | Document Storage | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.2.01.02` | Document Storage Organisation Methodology | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.2.01.02` | Resources | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.2.01.02` | Guidance | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.2.02` | Registries | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.01` | Role Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.02` | People Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.03` | Dates Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.04` | Commitments Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.05` | Stakeholder Engagement Log | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.2.02.06` | Communication Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.07` | Dependency Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.08` | Meeting and Event Log | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.2.02.09` | Deliverables Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.10` | Contract Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.2.02.11` | Accessibility Registry | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.3` | Enterprise Risk and Compliance Management (Aspect) | `[00] Management / [30] Registers / [90] Existing Registers` | REVIEW DUPLICATE ID |
| `01.3.1` | Risk Management Framework Application | `[00] Management / [30] Registers / [90] Existing Registers` | PRESERVE |
| `01.3.2` | Compliance Traceability Mapping | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.3.3` | Assurance Event Planning | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | PRESERVE |
| `01.4` | Structured Review Planning (Aspect) | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `02` | Environmental Sensing | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `02.1` | Preparation | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `02.2` | Early Sector/Problem Sensing | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `02.2.1` | Environmental Scan | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `02.2.2` | Problem Statement Drafting | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `02.2.2.1` | Problem Statement Document | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `02.2.3` | Trigger Event Analysis | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `02.2.4` | Opportunity Identification | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `03` | Strategic Framing | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `03.1` | Preparation | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `03.2` | Early Direction Setting | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `03.2.1` | Strategic Intent Definition | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `03.2.2` | Strategic Fit Assessment | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `03.2.3` | Outcome Framing | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `03.3` | Strategic Financing Planning | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `03.3.1` | Investment Logic Mapping | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `03.3.2` | Indicative Funding Scenario Planning | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `03.3.3` | Constraints and Dependencies Identification | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | PRESERVE |
| `04` | Project Financing | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.1` | Preparation | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.2` | Cost Estimation | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.3` | Funding Strategy Development | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `04.4` | Investment Logic Mapping (Optional) | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.4` | Budget Submission Preparation | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.5` | Funding Negotiation and Approval | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `04.6` | Funding Allocation and Baseline Setup | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `04.4` | Financial Governance Planning | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `05` | Project Preparation | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `05.1` | Preparation | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.2` | Project Framing | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.2.1` | Purpose and Scope Definition | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.2.2` | Governance Structure Design | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.2.3` | Success Criteria and KPIs | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.3` | Resourcing | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.3.01` | Determine Delivery Roles | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `05.3.01` | Advertise for Delivery Roles | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `05.3.03` | Interview | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.3.04` | Contract | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.4` | Project Resource | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.4.1` | Delivery Methods and Planning | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.4.2` | Project Initiation and Resourcing | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `05.4.3` | Stakeholder and Communications Planning | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | PRESERVE |
| `06` | Solution Context Discovery | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.1` | Preparation | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.2` | Context Discovery | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.2.1` | Sector and Ecosystem Mapping | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.2.2` | Stakeholder Mapping | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.2.3` | Systems Landscape Review | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3` | Constraint Discovery | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.3.1` | Legal Constraints | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.1.1` | Disclosure Regulations | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.1.2` | Privacy Regulations | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.1.3` | Security Regulations | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.1.4` | Accessibility Regulations | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.2` | Organisation Policy Constraints | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.2.1` | Governance Constraints | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.2.2` | Principle Constraints | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.2.3` | Pattern Constraints | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.3.2.4` | Technology Constraints | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4` | Reference | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.4.1` | Reference Terminologies | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.01.01` | Reference: Delivery Terms & and Acronyms Document | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.2` | Delivery Guidance | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.3` | Discovery Guidance | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.4` | Definition Guidance | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.5` | Design Guidance | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.6` | Design Guidance | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.7` | Service Design Guidance | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4.8` | System Design Guidance | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.5` | Definition of Needs, Constraints, and Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.5.1` | Reference: Terminologies | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.5.1` | Business Needs Definition | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.5.1` | Delivery Channels | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.5.2` | User Persona Definition | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.5.3` | User Journey Mapping | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.5.4` | User Role Modelling: Definitions, Escalation, Delegation | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.5.5` | User Requirements Discovery | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.5.6` | Capability Modelling | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.7` | Market Analysis | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.8` | Options Analysis | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07` | Solution Definition | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.1` | Preparation | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2` | Definitions | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `07.2.1` | Terminologies | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2.1.1` | Business Domain Terminology | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2.1.2` | Delivery Terminology | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2.1.3` | Infrastructure Terminology | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2.1.4` | System Terminology | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `07.2.1.4` | System Integration Terminology] | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `07.2` | Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `07.1.1` | Business Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.1.2` | User Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2.3` | Quality Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2.4` | Capability Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.2.5` | Define the Service Capabilities. | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.1.3` | System Non-Functional Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.1.4` | System Functional Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.1.5` | Transitional Requirements | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `06.4` | Solution Description | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `07.3.1` | Solution Options and Analysis | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.3.2` | High-Level Architecture Framing | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `07.3.3` | Traceability Mapping | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | PRESERVE |
| `08` | Solution Design Response | `[50] Design / [90] Existing Design / [10] Solution Design Response` | REVIEW DUPLICATE ID |
| `08.1` | Preparation | `[50] Design / [90] Existing Design / [10] Solution Design Response` | REVIEW DUPLICATE ID |
| `08.2` | Solution Response Investigation | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.3` | Solution Response Preparation | `[50] Design / [90] Existing Design / [10] Solution Design Response` | REVIEW DUPLICATE ID |
| `08.3.1` | Response Structuring | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.3.2` | Compliance Self-Assessment | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.3.3` | Risk Identification in Response | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.3.4` | Commercial Modelling | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.4` | Solution Alignment and Internal Review | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.4.1` | Internal Architecture and Technical Review | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.4.2` | Strategic and Business Alignment Review | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `08.4.3` | Readiness for Procurement or Build Decision | `[50] Design / [90] Existing Design / [10] Solution Design Response` | PRESERVE |
| `09` | Procurement Preparation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.1` | Preparation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `09.2` | Procurement Strategy and Planning | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2.1` | Procurement Threshold Analysis | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2.2` | Procurement Governance Setup | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2.3` | Approach to Market Structuring | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2` | Tender Documentation Preparation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2.1` | Solution Architecture Documentation Finalisation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2.2` | Tender Response Requirements Specification | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2.3` | Evaluation Criteria and Weighting Definition | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2.4` | Draft Contract and Terms Finalisation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `09.3` | Internal Procurement Approvals | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `09.3.1` | Probity and Legal Review | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `09.3.2` | Governance and Sponsorship Endorsement | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10` | Vendor Selection | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10.1` | Preparation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.2` | Response Validation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10.2.1` | Eligibility Screening | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.2.2` | Completeness Review | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.2.3` | Alignment Pre-Check | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.3` | Response Evaluation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10.3.1` | Scoring Coordination | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.3.2` | Moderation and Consensus | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.3.3` | Compliance, Quality, and Risk Reviews | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.4` | Recommendation and Governance Approval | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10.4.1` | Evaluation Reporting | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `10.4.2` | Governance Decision and Recording | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | PRESERVE |
| `11` | Delivery Preparation & Enablement | `[60] Delivery / [10] Enablement / [90] Delivery Preparation` | REVIEW DUPLICATE ID |
| `11.1` | Preparation | `[60] Delivery / [10] Enablement / [90] Delivery Preparation` | PRESERVE |
| `11.2` | Contract Finalisation | `[60] Delivery / [10] Enablement / [90] Delivery Preparation` | REVIEW DUPLICATE ID |
| `11.3` | Resourcing | `[60] Delivery / [10] Enablement / [10] Resourcing Onboarding and Training` | REVIEW DUPLICATE ID |
| `11.4` | Environment and Licensing Enablement | `[60] Delivery / [10] Enablement / [20] Environments Access and Licensing` | REVIEW DUPLICATE ID |
| `11.5` | Delivery Orientation and Training | `[60] Delivery / [10] Enablement / [10] Resourcing Onboarding and Training` | REVIEW DUPLICATE ID |
| `12` | Service Delivery Implementation | `[60] Delivery / [20] System of Delivery / [90] Existing Delivery Enablement` | REVIEW DUPLICATE ID |
| `12.2` | Preparation | `[60] Delivery / [20] System of Delivery / [90] Existing Delivery Enablement` | PRESERVE |
| `12.1` | System of Delivery Enablement | `[60] Delivery / [20] System of Delivery / [90] Existing Delivery Enablement` | REVIEW DUPLICATE ID |
| `13` | Service Implementation | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.1` | Preparation | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.2` | System Data Implementation | `[60] Delivery / [30] Data and Content / [10] Schemas and Storage` | REVIEW DUPLICATE ID |
| `13.3` | System Media | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | REVIEW DUPLICATE ID |
| `13.3.11` | Logo Images | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.12` | Background Images | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.21` | Cookie/Tracking Disclosure | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.22` | Data Use Purpose, Correction and Sharing Disclosure | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.23` | System Terms & Conditions | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.31` | Labels (internal) | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.32` | Messages (external) | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.41` | Audio | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.3.51` | Culture-Language Packs | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | PRESERVE |
| `13.4` | Core Services Build | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.4.01` | Component Layout | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.4.01` | Logical Schema | `[60] Delivery / [30] Data and Content / [10] Schemas and Storage` | REVIEW DUPLICATE ID |
| `13.4.02` | Data Schema | `[60] Delivery / [30] Data and Content / [10] Schemas and Storage` | REVIEW DUPLICATE ID |
| `13.4.01` | Service Domain | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.4.01` | Configuration | `[60] Delivery / [40] Core Service / [20] Configuration Storage and Caching` | REVIEW DUPLICATE ID |
| `13.4.02` | Integrations – Diagnostics Storage | `[60] Delivery / [50] Integrations / [30] External and Secure Integrations` | REVIEW DUPLICATE ID |
| `13.4.03` | Integrations – Data Storage | `[60] Delivery / [30] Data and Content / [10] Schemas and Storage` | REVIEW DUPLICATE ID |
| `13.4.04` | Integrations – Caching | `[60] Delivery / [50] Integrations / [30] External and Secure Integrations` | REVIEW DUPLICATE ID |
| `13.4.05` | System Settings | `[60] Delivery / [40] Core Service / [20] Configuration Storage and Caching` | REVIEW DUPLICATE ID |
| `13.4.06` | Sessions | `[60] Delivery / [40] Core Service / [30] Identity Access and Sessions` | PRESERVE |
| `13.4.07` | Permissions | `[60] Delivery / [40] Core Service / [30] Identity Access and Sessions` | PRESERVE |
| `13.4.08` | Routes | `[60] Delivery / [40] Core Service / [20] Configuration Storage and Caching` | PRESERVE |
| `13.4.02` | Social Domain | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.4.01` | Users | `[60] Delivery / [40] Core Service / [30] Identity Access and Sessions` | REVIEW DUPLICATE ID |
| `13.4.02` | Relationships | `[60] Delivery / [40] Core Service / [30] Identity Access and Sessions` | REVIEW DUPLICATE ID |
| `13.4.03` | Groups | `[60] Delivery / [40] Core Service / [30] Identity Access and Sessions` | REVIEW DUPLICATE ID |
| `13.4.04` | Roles | `[60] Delivery / [40] Core Service / [30] Identity Access and Sessions` | REVIEW DUPLICATE ID |
| `13.4.03` | Registries Domain | `[60] Delivery / [40] Core Service / [40] Registries and Work` | REVIEW DUPLICATE ID |
| `13.5.01` | Registries | `[60] Delivery / [40] Core Service / [40] Registries and Work` | PRESERVE |
| `13.4.04` | Aspirations Domain | `[60] Delivery / [40] Core Service / [40] Registries and Work` | REVIEW DUPLICATE ID |
| `13.6.01` | Aspirations | `[60] Delivery / [40] Core Service / [40] Registries and Work` | PRESERVE |
| `13.6.02` | Milestones | `[60] Delivery / [40] Core Service / [40] Registries and Work` | PRESERVE |
| `13.4.05` | Work Domain | `[60] Delivery / [40] Core Service / [40] Registries and Work` | REVIEW DUPLICATE ID |
| `13.7.01` | Tasks | `[60] Delivery / [40] Core Service / [40] Registries and Work` | PRESERVE |
| `13.7.02` | Projects | `[60] Delivery / [40] Core Service / [40] Registries and Work` | PRESERVE |
| `13.05` | Secure Service Integrations | `[60] Delivery / [50] Integrations / [30] External and Secure Integrations` | PRESERVE |
| `13.06` | Data Migrations | `[60] Delivery / [30] Data and Content / [10] Schemas and Storage` | REVIEW DUPLICATE ID |
| `13.06` | Service Monitoring | `[60] Delivery / [90] Operational Enablement / [20] Monitoring and Alerting` | REVIEW DUPLICATE ID |
| `13.08` | Service Interoperability Enablement | `[60] Delivery / [50] Integrations / [40] Interoperability and Discovery` | PRESERVE |
| `13.09` | Service Client User Interface | `[60] Delivery / [60] Client Applications / [30] User Interfaces` | PRESERVE |
| `13.10` | Service Registration and Discovery | `[60] Delivery / [50] Integrations / [40] Interoperability and Discovery` | PRESERVE |
| `14` | Operational Readiness Assessment | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.1` | Service Orientation and Support Artefacts | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.2` | Distribution and Uptake Planning | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.3` | Marketing and Communications | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.4` | Account Management | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.5` | System Quality Review | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.6` | Service Compliance and Assurance | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.7` | Service Evaluation | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.8` | Gateway Review | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | PRESERVE |
| `15` | Operational Service Management | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.1` | Consumer Support Operations | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.2` | Provider Support Operations | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.3` | Live Operations and Scheduling | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.4` | Incident Management | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.5` | Problem Management | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.6` | Change Management | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.7` | Maintenance | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.8` | Continuous Improvement | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.9` | Operation Evaluation | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `16` | Service Transition | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.1` | Preparation | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.2` | Transition Evaluation | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.4` | Transition Preparation and Readiness | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.4` | Transfer Target Identification and Vetting | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.5` | Transition Execution | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.6` | Post Execution Support | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.7` | Transition Evaluation | `[70] Transition / [50] Transition / [90] Existing Service Transition` | PRESERVE |
| `17` | Closure and Exit | `[90] Closure / [10] Retirement / [90] Existing Closure and Exit` | PRESERVE |
| `17.1` | Preparation | `[90] Closure / [10] Retirement / [90] Existing Closure and Exit` | PRESERVE |
| `17.2` | Final Evaluation | `[90] Closure / [10] Retirement / [90] Existing Closure and Exit` | PRESERVE |
| `17.3` | Closure Planning | `[90] Closure / [10] Retirement / [90] Existing Closure and Exit` | PRESERVE |
| `17.4` | Decommissioning and Exit | `[90] Closure / [10] Retirement / [90] Existing Closure and Exit` | PRESERVE |
| `17.5` | Exit Evaluation | `[90] Closure / [10] Retirement / [90] Existing Closure and Exit` | PRESERVE |
| `00` | Whole of Service Lifecycle | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `03` | Cross-Cutting Governance Concerns (Upwards): | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `04` | Cross-Cutting Management Concerns (Inwards) | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `13` | Early Framing and Planning | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.1` | Preparation (Concept Shaping) | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.2` | Direction (Strategic Framing) | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.3` | Discovery (Early Exploration) | `[60] Delivery / [50] Integrations / [40] Interoperability and Discovery` | REVIEW DUPLICATE ID |
| `13.4` | Definition (Needs and Constraints) | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.5` | Business Case Development (Framing, Iteration, Validation) | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.8` | Outputs | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.81` | Stakeholder Map | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `13.82` | Business Requirements | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `13.83` | High-Level Benefits | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `13.84` | Cost Estimates | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `13.85` | Risk Register (Initial) | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `13.86` | Draft Management Case | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `13.87` | Initial (unvalidated) User Requirements | `[60] Delivery / [40] Core Service / [30] Identity Access and Sessions` | PRESERVE |
| `13.9` | Deliverables: | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.91` | Final Business Case Document (Signed) | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `13.92` | Benefits Realisation Strategy (Approved) | `[60] Delivery / [40] Core Service / [10] Components and Modules` | PRESERVE |
| `14` | Financing (distinct from framing & planning) | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `15.1` | Preparation | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.2` | Business Requirements Discovery & Definition | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.3` | User Requirements Discovery & Definition | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.4` | Workflow Scenarios & Journeys Discovery & Definition | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.5` | Service Qualities & Non-Functional Requirement Discovery & Definition | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.6` | Capability Identification and Structuring | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.7` | System Functional Requirement Discovery & Definition | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.8` | Transitional Service Delivery Requirement Discovery & Definition | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.8` | Outputs: | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.81` | Solution Design - Reference / Guidance | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.82` | Solution Design View - Background | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.83` | Solution Design View - Context | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.84` | Solution Design View - Constraints (legal, agreements, principles, patterns, technology, integrations) | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.85` | Solution Design View - Information | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.86` | Solution Design View - User Requirements | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.87` | Solution Design View - Capabilities Requirements | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.88` | Solution Design View - Quality Requirements | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `15.89` | Solution Design View - Selective Functional Summary | `[80] Operations / [10] Service / [90] Existing Service Management` | PRESERVE |
| `16` | Solution Architect Description (SAD) | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `21` | Response Preparation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `22` | Response Development | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `23` | Response Validation and Alignment | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `31` | Procurement Preparation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `31.1` | Procurement Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `31.2` | Market Research and Approach to Market | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `31.3` | Procurement Documentation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `31.4` | Internal Procurement Governance | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `32` | Tender | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `32.1` | Preparation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `32.2` | RFP Issuance and Market Engagement | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `32.3` | Clarifications and Amendments | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `33` | Response Evaluation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `33.1` | Evaluation Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `33.2` | Evaluation Team and Process | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `33.3` | Evaluation Results and Recommendation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `41` | System of Delivery | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `40.1` | Delivery Pipeline and Automation Setup | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `40.2` | Environment Provisioning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `40.3` | Transitional Requirements and Constraints | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `40.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `42` | System Data Implementation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `42.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `43` | System Media | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `44` | System Implementation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `44.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `45` | System Integrations | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `45.1` | Integration Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `45.2` | Technical Integration Execution | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `45.3` | Dependency Stabilisation and Assurance | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `45.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `45.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `46` | System Monitoring | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `46.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `47` | System Interoperability Enablement | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `47.1` | Delivery Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `47.2` | Change Readiness and Communication | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `47.3` | Implementation and Integration Activities | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `47.4` | Operational Transition Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `47.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `47.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `48` | Service Client User Interface | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `49` | System Registration and Discovery | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `48.1` | Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `48.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `48.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `51` | Service Orientation & Support Artefacts | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `51.1` | Planning and Audience Identification | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `51.2` | Artefact Development and Validation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `51.3` | Distribution and Handover | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `51.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `51.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `52` | … | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61` | Distribution, Uptake and Relationship Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61.1` | Channel Strategy | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61.2` | Signup, Subscription, Incentives and Termination Setup | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61.3` | Terms | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61.4` | Pricing (Optional) | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61.5` | Pre-Launch Enablement | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61.6` | Launch Campaigns | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `61.7` | Partnership & Channel Development (Optional) | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `62` | Marketing & Communications | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `62.1` | Marketing Strategy | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `62.2` | Messaging and Content Development | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `62.3` | Channel Planning and Media Buys | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `62.4` | Internal Communications | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `62.5` | Campaign Execution | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `62.6` | Media and Issue Management | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `63` | Account & Relationship Management | `[00] Management / [90] Review / [30] Existing SELF Review` | REVIEW DUPLICATE ID |
| `63.1` | Sales/Uptake Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `63.2` | Sales Enablement Resources | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `63.3` | Prospect and Lead Management | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `63.4` | Subscription and Onboarding Execution | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `63.5` | Account Management Setup | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `63` | – Account Management | `[00] Management / [90] Review / [30] Existing SELF Review` | REVIEW DUPLICATE ID |
| `71` | System Quality Review (QA) | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `71.1` | Quality Planning and Framing | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `71.2` | Quality Testing and Review Activities | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `71.3` | Quality Reporting and Sign-Off | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `71.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `71.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `72` | Service Compliance and Assurance | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `72.1` | C&A Planning and Scoping | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `72.2` | Review Coordination and Remediation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `72.3` | Change Readiness and Communication | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `72.4` | Implementation and Integration Activities | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `72.5` | Operational Transition Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `72.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `73` | Service Evaluation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `81` | Support | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `81.1` | Support Planning and Service Design | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `81.2` | Support Operations and Triage | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `81.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `81.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `82` | Operations | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `82.1` | Operational Monitoring and Scheduling | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `82.2` | Service Execution and Coordination | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `82.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `82.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `83` | Change Management | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `83.1` | Change Requests and Prioritisation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `83.2` | Change Approval and Coordination | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `83.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `83.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `84` | Maintenance | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `84.1` | Maintenance Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `84.2` | Update Execution and Review | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `84.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `84.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `85` | Evaluation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `85.1` | Post-Implementation Review | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `85.2` | Benefits Realisation and Outcome Measurement | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `85.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `85.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `86` | Continuous Improvement | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `86.1` | Improvement Backlog and Ideation | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `86.2` | Evaluation and Selection | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `86.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `86.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `91` | Transition Evaluation | `[00] Management / [90] Review / [30] Existing SELF Review` | REVIEW DUPLICATE ID |
| `92` | Transition Preparation and Readiness | `[00] Management / [90] Review / [30] Existing SELF Review` | REVIEW DUPLICATE ID |
| `93` | Target Identification and Vetting | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `94` | Transition Execution | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `95` | Post-Transition Support and Closure | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `91` | Final Evaluation | `[00] Management / [90] Review / [30] Existing SELF Review` | REVIEW DUPLICATE ID |
| `91.1` | Post-Implementation Review | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `91.2` | Benefits Realisation and Outcome Measurement | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `91.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `91.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `92` | Decommissioning, Closure and Exit | `[00] Management / [90] Review / [30] Existing SELF Review` | REVIEW DUPLICATE ID |
| `92.1` | Decommissioning Planning | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `92.2` | Transition to Successor or Archive | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `92.8` | Outputs | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `92.9` | Deliverables | `[00] Management / [90] Review / [30] Existing SELF Review` | PRESERVE |
| `01` | Cross Cutting Management | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.1` | Cross-Cutting Governance | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.2` | Cross-Cutting Management | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `01.3` | Risk and Compliance Management | `[00] Management / [30] Registers / [90] Existing Registers` | REVIEW DUPLICATE ID |
| `01.4` | Structured Review Planning | `[00] Management / [20] Governance / [90] Existing Cross-Cutting Management` | REVIEW DUPLICATE ID |
| `02` | Environmental Sensing | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `02.2` | Early Sector/Problem Sensing | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `03` | Strategic Framing | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `03.2` | Early Direction Setting | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `03.3` | Strategic Financing Planning | `[10] Strategy / [90] Existing Strategy / [10] Sensing and Framing` | REVIEW DUPLICATE ID |
| `04` | Project Financing | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.1` | Cost EstimationRough-order magnitude costing and refined cost models based on emerging solution understanding. | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `05` | Project Preparation | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.1` | Project Framing | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `04.2` | Project Setup | `[20] Investment / [90] Existing Investment / [10] Financing and Preparation` | REVIEW DUPLICATE ID |
| `06` | Solution Definition | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.1` | Context Discovery | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.3` | Definition | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.4` | Options Analyse | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `06.5` | Solution Description | `[30] Discovery / [90] Existing Definition / [10] Context and Definition` | REVIEW DUPLICATE ID |
| `08` | Service Response | `[50] Design / [90] Existing Design / [10] Solution Design Response` | REVIEW DUPLICATE ID |
| `08.1` | Preparation | `[50] Design / [90] Existing Design / [10] Solution Design Response` | REVIEW DUPLICATE ID |
| `08.3` | Response Alignment | `[50] Design / [90] Existing Design / [10] Solution Design Response` | REVIEW DUPLICATE ID |
| `09` | Procurement Preparation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2` | Procurement Preparation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `09.2` | Tender Management | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10` | Vendor Selection | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10.2` | Response ValidationValidate internal or vendor response for eligibility, strategic, completeness, constraint, technical and delivery alignment. | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10.3` | Response Evaluation | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `10.4` | Recommendation and Governance Approval | `[40] Procurement / [90] Existing Procurement / [10] Preparation and Selection` | REVIEW DUPLICATE ID |
| `11` | Delivery Preparation | `[60] Delivery / [10] Enablement / [90] Delivery Preparation` | REVIEW DUPLICATE ID |
| `11.2` | Contract Finalisation | `[60] Delivery / [10] Enablement / [90] Delivery Preparation` | REVIEW DUPLICATE ID |
| `11.3` | Resourcing | `[60] Delivery / [10] Enablement / [10] Resourcing Onboarding and Training` | REVIEW DUPLICATE ID |
| `11.4` | Environment and Licensing Enablement | `[60] Delivery / [10] Enablement / [20] Environments Access and Licensing` | REVIEW DUPLICATE ID |
| `11.5` | Delivery Orientation and Training | `[60] Delivery / [10] Enablement / [10] Resourcing Onboarding and Training` | REVIEW DUPLICATE ID |
| `12` | Delivery Enablement | `[60] Delivery / [20] System of Delivery / [90] Existing Delivery Enablement` | REVIEW DUPLICATE ID |
| `12.1` | System of Delivery Enablement Establish confidential integration credential storage, code repository protection, automation pipelines, CI/CD, structures, processes, test data, running, and reporting. | `[60] Delivery / [20] System of Delivery / [90] Existing Delivery Enablement` | REVIEW DUPLICATE ID |
| `13` | Service Implementation | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.1` | System Data Implementation | `[60] Delivery / [30] Data and Content / [10] Schemas and Storage` | REVIEW DUPLICATE ID |
| `13.2` | System Media | `[60] Delivery / [30] Data and Content / [30] Content Media and Localisation` | REVIEW DUPLICATE ID |
| `13.3` | Core Services Build | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.4` | Secure Service Integrations | `[60] Delivery / [50] Integrations / [30] External and Secure Integrations` | REVIEW DUPLICATE ID |
| `13.5` | ETL | `[60] Delivery / [40] Core Service / [10] Components and Modules` | REVIEW DUPLICATE ID |
| `13.6` | Service Monitoring | `[60] Delivery / [90] Operational Enablement / [20] Monitoring and Alerting` | PRESERVE |
| `13.7` | Service Interoperability Enablement | `[60] Delivery / [50] Integrations / [40] Interoperability and Discovery` | PRESERVE |
| `13.8` | Service Client User Interface | `[60] Delivery / [60] Client Applications / [30] User Interfaces` | REVIEW DUPLICATE ID |
| `13.9` | Service Registration and Discovery | `[60] Delivery / [50] Integrations / [40] Interoperability and Discovery` | REVIEW DUPLICATE ID |
| `14` | Operational Readiness Assessment | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.1` | Service Orientation and Support Artefacts | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.2` | Distribution and Uptake Planning | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.3` | Marketing and Communications | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.4` | Account Management | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.5` | System Quality Review | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.6` | Service Compliance and Assurance | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `14.7` | Service Evaluation | `[70] Transition / [10] Readiness / [90] Existing Readiness Assessment` | REVIEW DUPLICATE ID |
| `15` | Operational Service Management | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.1` | Consumer Support Operations | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.2` | Provider Support Operations Support partner and intermediary service providers | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.3` | Live Operations and Scheduling Operate the service and manage job orchestration | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.4` | Incident Management Respond to service interruptions and outages. | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.5` | Problem Management identify and eliminate root causes of recurring incidents | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.6` | Change Management Govern change requests, approvals, and releases. | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.7` | Maintenance Apply patches, updates, and technical improvements. | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.8` | Continuous Improvement Gather feedback and incrementally improve the service | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `15.9` | Operation Evaluation | `[80] Operations / [10] Service / [90] Existing Service Management` | REVIEW DUPLICATE ID |
| `16` | Service Transition | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.1` | Transition Evaluation | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.2` | Transition Preparation and Readiness | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.3` | Transfer Target Identification and Vetting | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.4` | Transition Execution | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.5` | Post Execution Support | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.6` | Transition Evaluation | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16` | Service Closure and Exit | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.1` | Final Evaluation | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.2` | Closure Planning | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.3` | Decommissioning and Exit | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |
| `16.4` | Exit Evaluation | `[70] Transition / [50] Transition / [90] Existing Service Transition` | REVIEW DUPLICATE ID |

## Complete source-folder landing register

Every source folder outside `.git` and `TARGET` appears below. Direct file count is the number immediately in that folder. Descendant file count includes its complete subtree.

### 52.Design

- Treatment: **SPLIT**
- Direct files: **8**
- Descendant files: **20**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`
  - `TARGET\[50] Design\[10] Architecture\[10] Architecture Direction`
  - `TARGET\[60] Delivery\[30] Data and Content\[10] Schemas and Storage`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### 52.Design\51.Technical

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **12**
- Proposed destinations:
  - `TARGET\[50] Design\[10] Architecture\[10] Architecture Direction`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### 52.Design\51.Technical\00.Guidance

- Treatment: **SPLIT**
- Direct files: **7**
- Descendant files: **12**
- Proposed destinations:
  - `TARGET\[50] Design\[10] Architecture\[10] Architecture Direction`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### 52.Design\51.Technical\00.Guidance\01.Draft

- Treatment: **SPLIT**
- Direct files: **5**
- Descendant files: **5**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### 99.Archive

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### 99.Archive\01.Legacy

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[90] Closure\[30] Decommissioning\[20] Migration and Retention`

### [03] Images

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [03] Images\[00].Deployment View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [04.aa] Diagrams

- Treatment: **SPLIT REVIEW**
- Direct files: **528**
- Descendant files: **533**
- Proposed destinations:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`
  - `TARGET\[00] Management\[10] Repository\[20] Repository Guidance`
  - `TARGET\[00] Management\[20] Governance\[10] Governance and Principles`
  - `TARGET\[00] Management\[20] Governance\[20] Decisions`
  - `TARGET\[00] Management\[20] Governance\[30] Reviews and Compliance`
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`
  - `TARGET\[20] Investment\[10] Business Case\[10] Strategic Case`
  - `TARGET\[20] Investment\[10] Business Case\[20] Economic Case`
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`
  - `TARGET\[30] Discovery\[10] Context\[20] System Context`
  - `TARGET\[30] Discovery\[10] Context\[30] Scope Constraints and Dependencies`
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`
  - `TARGET\[40] Procurement\[10] Preparation\[10] Approach and Requirements`
  - `TARGET\[40] Procurement\[70] Contracting\[10] Contracts and Obligations`
  - `TARGET\[50] Design\[10] Architecture\[10] Architecture Direction`
  - `TARGET\[50] Design\[10] Architecture\[30] Patterns and Principles`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[20] Information\[30] Physical Models`
  - `TARGET\[50] Design\[20] Information\[30] Quality Metadata and Records`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[50] Design\[30] Functionality\[20] Workflows`
  - `TARGET\[50] Design\[30] Functionality\[30] Use Cases`
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`
  - `TARGET\[50] Design\[50] Assurance\[20] Identity and Access Design`
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`
  - `TARGET\[50] Design\[60] Technology\[10] Platforms and Infrastructure`
  - `TARGET\[60] Delivery\[10] Enablement\[30] Tools and Licensing`
  - `TARGET\[60] Delivery\[20] System of Delivery\[20] Artefacts and Packaging`
  - `TARGET\[60] Delivery\[20] System of Delivery\[30] Pipelines and Automation`
  - `TARGET\[60] Delivery\[30] Data and Content\[10] Schemas and Storage`
  - `TARGET\[60] Delivery\[30] Data and Content\[30] Content Media and Localisation`
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[40] Core Service\[90] Development Requiring Detail`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[50] Integrations\[30] External Services`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[70] Verification\[30] Performance Testing`
  - `TARGET\[60] Delivery\[70] Verification\[40] Security Testing`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[30] Data Migration`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[10] Logging and Telemetry`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04.aa] Diagrams\_WORKAREA

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04.aa] Diagrams\_WORKAREA\[23.da] Context - Business - Service - Dependents

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04.aa] Diagrams\_WORKAREA\[23.da] Context - Business - Service - Dependents\00.Images

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams

- Treatment: **SPLIT REVIEW**
- Direct files: **2**
- Descendant files: **517**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [04] Diagrams\00.C&A

- Treatment: **SPLIT REVIEW**
- Direct files: **0**
- Descendant files: **19**
- Proposed destinations:
  - `TARGET\[00] Management\[30] Registers\[10] Risks`
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`
  - `TARGET\[50] Design\[10] Architecture\[30] Patterns and Principles`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`
  - `TARGET\[60] Delivery\[40] Core Service\[90] Development Requiring Detail`

### [04] Diagrams\00.C&A\02.Diagrams

- Treatment: **SPLIT REVIEW**
- Direct files: **16**
- Descendant files: **19**
- Proposed destinations:
  - `TARGET\[00] Management\[30] Registers\[10] Risks`
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`
  - `TARGET\[50] Design\[10] Architecture\[30] Patterns and Principles`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`
  - `TARGET\[60] Delivery\[40] Core Service\[90] Development Requiring Detail`

### [04] Diagrams\00.C&A\02.Diagrams\00.Images

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\00.C&A\02.Diagrams\01.Document

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[00] Management\[30] Registers\[10] Risks`

### [04] Diagrams\[--] EOI - Primary Identification

- Treatment: **SPLIT REVIEW**
- Direct files: **2**
- Descendant files: **2**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`

### [04] Diagrams\[--] EOI - Secondary Identification

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[00].Specific

- Treatment: **SPLIT REVIEW**
- Direct files: **0**
- Descendant files: **4**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`

### [04] Diagrams\[00].Specific\[64].NZ

- Treatment: **SPLIT REVIEW**
- Direct files: **3**
- Descendant files: **4**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`

### [04] Diagrams\[00].Specific\[64].NZ\[00].Govt

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[10.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[10.ab] Discovery

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[10.ab] Discovery\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[12.aa].Documentation

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[12.aa].Documentation\Templates

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[21.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[21.aa] Context

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **6**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[30] Scope Constraints and Dependencies`

### [04] Diagrams\[21.aa] Context\03.Images

- Treatment: **SPLIT**
- Direct files: **4**
- Descendant files: **4**
- Proposed destinations:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`
  - `TARGET\[30] Discovery\[10] Context\[30] Scope Constraints and Dependencies`
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`

### [04] Diagrams\[21.aa] Context\98.Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[30] Scope Constraints and Dependencies`

### [04] Diagrams\[21.ba] Context - Market

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[21.ba] Context - Market\03.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[21.ba] Context - Market\99.Archive

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[30] Decommissioning\[20] Migration and Retention`

### [04] Diagrams\[21.ba] Context - Market\99.Archive\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[30] Decommissioning\[20] Migration and Retention`

### [04] Diagrams\[21.bb] Context - Trends

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[21.bb] Context - Trends\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[22.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[23.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[23.ca] Context - Business - Service - Users

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **21**
- Proposed destinations:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[23.ca] Context - Business - Service - Users\00.Images

- Treatment: **SPLIT**
- Direct files: **18**
- Descendant files: **18**
- Proposed destinations:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`

### [04] Diagrams\[23.ca] Context - Business - Service - Users\01.Document

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[23.ca] Context - Business - Service - Users\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[23.fi] Context - Business - Service - Domains - Scheduling

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[23.ga] Context - Business - Service - Standards

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **16**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[23.ga] Context - Business - Service - Standards\02.Diagrams

- Treatment: **SPLIT**
- Direct files: **12**
- Descendant files: **15**
- Proposed destinations:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[30] External Services`

### [04] Diagrams\[23.ga] Context - Business - Service - Standards\02.Diagrams\00.Outputs

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [04] Diagrams\[23.ga] Context - Business - Service - Standards\02.Diagrams\test

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`

### [04] Diagrams\[23.ga] Context - Business - Service - Standards\02.Diagrams\test\-------------------------------------------------------------------------

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`

### [04] Diagrams\[23.ha] Context - Business - Service - Integrations

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [04] Diagrams\[23.ha] Context - Business - Service - Integrations\02.Diagrams

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [04] Diagrams\[23.ha] Context - Business - Service - Integrations\02.Diagrams\00.Outputs

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [04] Diagrams\[25.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[25.ab] Context - Business - Case - Drivers

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.ab] Context - Business - Case - Drivers\00.Images

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.ab] Context - Business - Case - Drivers\01.Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.ac] Context - Business - Case - Objectives

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.da] Context - Business - Case - BBC

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.db] Context - Business - Case - BBC - Strategic Case

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.dc] Context - Business - Case - BBC - Commercial Case

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.dd] Context - Business - Case - BBC - Economic Case

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.de] Context - Business - Case - BBC - Financial Case

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[25.df] Context - Business - Case - BBC - Management Case

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[10] Business Context`

### [04] Diagrams\[27.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[28.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[28.aa] Context - System

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **14**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[20] System Context`

### [04] Diagrams\[28.aa] Context - System\00.Images

- Treatment: **SPLIT**
- Direct files: **7**
- Descendant files: **7**
- Proposed destinations:
  - `TARGET\[30] Discovery\[10] Context\[20] System Context`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[28.aa] Context - System\01.Document

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[20] System Context`

### [04] Diagrams\[28.aa] Context - System\02.Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[30] Discovery\[10] Context\[20] System Context`

### [04] Diagrams\[28.aa] Context - System\02.Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[28.ba] Context - System - Constraints

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **10**
- Proposed destinations:
  - `TARGET\[30] Discovery\[10] Context\[20] System Context`
  - `TARGET\[50] Design\[10] Architecture\[30] Patterns and Principles`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`

### [04] Diagrams\[28.ba] Context - System - Constraints\00.Images

- Treatment: **SPLIT**
- Direct files: **10**
- Descendant files: **10**
- Proposed destinations:
  - `TARGET\[30] Discovery\[10] Context\[20] System Context`
  - `TARGET\[50] Design\[10] Architecture\[30] Patterns and Principles`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`

### [04] Diagrams\[30.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[32.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[32.ea] Project - Execution - Planning

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **7**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [04] Diagrams\[32.ea] Project - Execution - Planning\00.Images

- Treatment: **MERGE**
- Direct files: **7**
- Descendant files: **7**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [04] Diagrams\[32.fa] Project - Execution - WorkItems

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [04] Diagrams\[41.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[42.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[42.aa] Digital Service  - Interfaces

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[42.aa] Digital Service  - Interfaces\01.Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [04] Diagrams\[42.aa] Digital Service  - Interfaces\01.Resources\02.Diagrams

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [04] Diagrams\[42.aa] Digital Service - Capabilities

- Treatment: **MERGE**
- Direct files: **4**
- Descendant files: **9**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[42.aa] Digital Service - Capabilities\Discovery View - System - Capabilities

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[42.aa] Digital Service - Capabilities\Images

- Treatment: **MERGE**
- Direct files: **4**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[43.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[43.aa] Digital Service - Information

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **27**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[43.aa] Digital Service - Information\00.Images

- Treatment: **SPLIT**
- Direct files: **26**
- Descendant files: **26**
- Proposed destinations:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`

### [04] Diagrams\[43.ba] Digital Service - Information - Qualities

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **70**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[43.ba] Digital Service - Information - Qualities\02.Diagrams

- Treatment: **SPLIT**
- Direct files: **30**
- Descendant files: **31**
- Proposed destinations:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[20] Information\[30] Quality Metadata and Records`
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [04] Diagrams\[43.ba] Digital Service - Information - Qualities\02.Diagrams\07.Qualities - ISO 25030

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[43.ba] Digital Service - Information - Qualities\03.Images

- Treatment: **SPLIT**
- Direct files: **33**
- Descendant files: **33**
- Proposed destinations:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[20] Information\[30] Quality Metadata and Records`
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [04] Diagrams\[43.ba] Digital Service - Information - Qualities\99.Archive

- Treatment: **SPLIT**
- Direct files: **2**
- Descendant files: **5**
- Proposed destinations:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[90] Closure\[30] Decommissioning\[20] Migration and Retention`

### [04] Diagrams\[43.ba] Digital Service - Information - Qualities\99.Archive\01.Document

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[43.ca] Digital Service - Information - Requirements

- Treatment: **SPLIT REVIEW**
- Direct files: **16**
- Descendant files: **18**
- Proposed destinations:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[20] Information\[30] Quality Metadata and Records`
  - `TARGET\[60] Delivery\[40] Core Service\[90] Development Requiring Detail`

### [04] Diagrams\[43.ca] Digital Service - Information - Requirements\01.Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[43.ca] Digital Service - Information - Requirements\02.Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[43.ca] Digital Service - Information - Requirements\02.Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[43.da] Digital Service - Information - WorkItems

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[44.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[44.ea] Digital Service - Information - URLs

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[44.fa] Digital Service -Information - Messages

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`

### [04] Diagrams\[44.fb] Digital Service - Information - Notifications

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`

### [04] Diagrams\[44.fc] Digital Service - Information - Confirmation

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[44.ga] Digital Service - Information - Validation

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`

### [04] Diagrams\[44.ga] Digital Service - Information - Validation\02.Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[44.ga] Digital Service - Information - Validation\02.Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[44.hb] Digital Service - Information - Documentation

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[44.ia] Digital Service - Information - Domains

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[44.ja] Digital Service - Information - Entities

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`

### [04] Diagrams\[45.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[45.aa] Digital Service - Functionality

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **40**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.aa] Digital Service - Functionality\00.Images

- Treatment: **SPLIT**
- Direct files: **38**
- Descendant files: **38**
- Proposed destinations:
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[50] Design\[30] Functionality\[20] Workflows`
  - `TARGET\[60] Delivery\[30] Data and Content\[30] Content Media and Localisation`
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[45.ba] Digital Service - Functionality - User

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.ca] Digital Service - Functionality - Public

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.da] Digital Service - Functionality - Consumer

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.da] Digital Service - Functionality - Member

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.db] Digital Service - Functionality - Consumer - Admin

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.ea] Digital Service - Functionality - Consumer - Business

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.eb] Digital Service - Functionality - Consumer - Business Admin

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`

### [04] Diagrams\[45.fa] Digital Service - Functionality - Consumer - Support

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[45.fb] Digital Service - Functionality - Consumer - Support - Public

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[45.fc] Digital Service - Functionality - Consumer - Support - Member

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[45.fd] Digital Service - Functionality - Consumer - Support - Consumer

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[45.fe] Digital Service - Functionality - Consumer - Support - Business

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[45.ga] Digital Service - Functionality - Consumer - Operations

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[47.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[47.aa] Digital Service - Workflows

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[50] Design\[30] Functionality\[20] Workflows`

### [04] Diagrams\[47.fa] Digital Service - Workflows - Support

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[47.fb] Digital Service - Workflows - Support - Public

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[47.fc] Digital Service - Workflows - Support - Consumers

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[47.fd] Digital Service - Workflows - Support - Business

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[47.ga] Digital Service - Workflows - Operations

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[47.ha] Digital Service - Workflows - Maintenance

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [04] Diagrams\[48.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[48.aa] Digital Service - Interoperability

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **6**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [04] Diagrams\[48.aa] Digital Service - Interoperability\00.Images

- Treatment: **SPLIT**
- Direct files: **3**
- Descendant files: **3**
- Proposed destinations:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [04] Diagrams\[48.aa] Digital Service - Interoperability\01.Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [04] Diagrams\[50.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[50.aa] Digital Service - Security

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **22**
- Proposed destination:
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`

### [04] Diagrams\[50.aa] Digital Service - Security\Diagrams

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **21**
- Proposed destination:
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`

### [04] Diagrams\[50.aa] Digital Service - Security\Diagrams\00.Images

- Treatment: **SPLIT**
- Direct files: **20**
- Descendant files: **20**
- Proposed destinations:
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`
  - `TARGET\[60] Delivery\[30] Data and Content\[30] Content Media and Localisation`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[10] Logging and Telemetry`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[50.ca] Digital Service - Privacy

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`

### [04] Diagrams\[50.ca] Digital Service - Privacy\01.Diagrams

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`

### [04] Diagrams\[50.ca] Digital Service - Privacy\01.Diagrams\00.Images

- Treatment: **MERGE**
- Direct files: **4**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[50] Design\[50] Assurance\[30] Privacy Design`

### [04] Diagrams\[51.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[52.aa] Digital Service - Operations

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[52.aa] Digital Service - Operations\02.Diagrams

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[52.aa] Digital Service - Operations\02.Diagrams\00.Images

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[53.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[53.aa] Digital Service - Monitoring

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **2**
- Proposed destinations:
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[53.aa] Digital Service - Monitoring\02.Diagrams

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **2**
- Proposed destinations:
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[53.aa] Digital Service - Monitoring\02.Diagrams\00.Images

- Treatment: **SPLIT**
- Direct files: **2**
- Descendant files: **2**
- Proposed destinations:
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[54.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[54.aa] Digital Service - Maintenance

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [04] Diagrams\[54.aa] Digital Service - Maintenance\67.1.Maintenance View - #DR

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [04] Diagrams\[54.aa] Digital Service - Maintenance\67.1.Maintenance View - #DR\01.Images

- Treatment: **MERGE**
- Direct files: **5**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [04] Diagrams\[55.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[55.ab] Digital Service - Disestablishment

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[55.ab] Digital Service - Disestablishment\00.Images

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[72.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[72.aa] Digital Service  - QA

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **9**
- Proposed destinations:
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[70] Verification\[40] Security Testing`

### [04] Diagrams\[72.aa] Digital Service  - QA\0.QA View - Overview

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **9**
- Proposed destinations:
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[70] Verification\[40] Security Testing`

### [04] Diagrams\[72.aa] Digital Service  - QA\0.QA View - Overview\00.Images

- Treatment: **SPLIT**
- Direct files: **9**
- Descendant files: **9**
- Proposed destinations:
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[70] Verification\[40] Security Testing`

### [04] Diagrams\[80.aa] Digital Service - Accreditation

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[80.aa] Digital Service - Accreditation\00.Images

- Treatment: **MERGE REVIEW**
- Direct files: **5**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[81.--] ----- ----- ----- ----- -----

- Treatment: **MERGE REVIEW**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[81.aa] Digital Service - Change Management

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[81.aa] Digital Service - Change Management - ATO

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[81.aa] Digital Service - Change Management - ATO\01.Diagrams

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[81.aa] Digital Service - Change Management - ATO\01.Diagrams\00.Images

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[81.aa] Digital Service - Change Management\01.Diagrams

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[81.aa] Digital Service - Change Management\01.Diagrams\00.Images

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[82.aa] Delivery

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **89**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[82.aa] Delivery\00.Guidance

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [04] Diagrams\[82.aa] Delivery\Diagrams

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **87**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[82.aa] Delivery\Diagrams\00.Images

- Treatment: **SPLIT REVIEW**
- Direct files: **42**
- Descendant files: **42**
- Proposed destinations:
  - `TARGET\[00] Management\[10] Repository\[20] Repository Guidance`
  - `TARGET\[00] Management\[20] Governance\[10] Governance and Principles`
  - `TARGET\[00] Management\[20] Governance\[30] Reviews and Compliance`
  - `TARGET\[00] Management\[30] Registers\[10] Risks`
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[60] Delivery\[20] System of Delivery\[20] Artefacts and Packaging`
  - `TARGET\[60] Delivery\[20] System of Delivery\[30] Pipelines and Automation`
  - `TARGET\[60] Delivery\[30] Data and Content\[30] Content Media and Localisation`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[30] Data Migration`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [04] Diagrams\[82.aa] Delivery\Diagrams\01.Document

- Treatment: **SPLIT REVIEW**
- Direct files: **8**
- Descendant files: **8**
- Proposed destinations:
  - `TARGET\[00] Management\[30] Registers\[10] Risks`
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [04] Diagrams\[82.aa] Delivery\Diagrams\12.Design View  (Risks)

- Treatment: **SPLIT**
- Direct files: **4**
- Descendant files: **7**
- Proposed destinations:
  - `TARGET\[50] Design\[10] Architecture\[10] Architecture Direction`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`

### [04] Diagrams\[82.aa] Delivery\Diagrams\12.Design View  (Risks)\01.Document

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[10] Architecture Direction`

### [04] Diagrams\[82.aa] Delivery\Diagrams\12.Design View  (Risks)\02._Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[82.aa] Delivery\Diagrams\12.Design View  (Risks)\02._Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[82.aa] Delivery\Diagrams\13.Delivery View (Risks)

- Treatment: **SPLIT**
- Direct files: **28**
- Descendant files: **29**
- Proposed destinations:
  - `TARGET\[00] Management\[30] Registers\[10] Risks`
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[10] Release Management`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[82.aa] Delivery\Diagrams\13.Delivery View (Risks)\02.Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\[82.aa] Delivery\Diagrams\13.Delivery View (Risks)\02.Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [04] Diagrams\Deployment View - Assets

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [04] Diagrams\Deployment View - Infrastructure

- Treatment: **MERGE**
- Direct files: **11**
- Descendant files: **11**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [04] Diagrams\Diagrams

- Treatment: **SPLIT REVIEW**
- Direct files: **14**
- Descendant files: **30**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[50] Design\[50] Assurance\[20] Identity and Access Design`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [04] Diagrams\Diagrams\Development View - #Patterns

- Treatment: **SPLIT REVIEW**
- Direct files: **16**
- Descendant files: **16**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[90] Development Requiring Detail`

### [05] Documents

- Treatment: **SPLIT REVIEW**
- Direct files: **117**
- Descendant files: **295**
- Proposed destinations:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[40] Core Service\[90] Development Requiring Detail`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [05] Documents\01.Draft

- Treatment: **SPLIT REVIEW**
- Direct files: **81**
- Descendant files: **81**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`
  - `TARGET\[60] Delivery\[20] System of Delivery\[30] Pipelines and Automation`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [05] Documents\02.ForReview

- Treatment: **MERGE**
- Direct files: **15**
- Descendant files: **15**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\03.Released

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[10] Release Management`

### [05] Documents\25.Service Development Guidelines

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[90] Development Requiring Detail`

### [05] Documents\64.NZ

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **6**
- Proposed destinations:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\64.NZ\NZ Govt

- Treatment: **SPLIT**
- Direct files: **5**
- Descendant files: **6**
- Proposed destinations:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\64.NZ\NZ Govt\NZ MOE

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\98.Resources

- Treatment: **SPLIT**
- Direct files: **2**
- Descendant files: **2**
- Proposed destinations:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\[001.00] Terminologies

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\[001.00] Terminologies\00.DRAFT

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\[001.00] Terminologies\00.DRAFT\Appendices

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\[001.00] Terminologies\01.Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`

### [05] Documents\_TOSORT

- Treatment: **MERGE REVIEW**
- Direct files: **1**
- Descendant files: **18**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [05] Documents\_TOSORT\01.Resources - Examples

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [05] Documents\_TOSORT\02.Guidance

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **12**
- Proposed destinations:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [05] Documents\_TOSORT\02.Guidance\_Errata Requirements Sources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [05] Documents\_TOSORT\02.Guidance\Stakeholder Desires

- Treatment: **SPLIT**
- Direct files: **11**
- Descendant files: **11**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[20] Monitoring and Alerting`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [05] Documents\_TOSORT\22.SAD

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [05] Documents\_TOSORT\23.GLAD

- Treatment: **MERGE REVIEW**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[00] Management\[90] Review\[10] Classification Required`

### [05] Documents\Documents

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [05] Documents\Documents - Guidance

- Treatment: **SPLIT**
- Direct files: **25**
- Descendant files: **25**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [05] Documents\Documents - Reference - Glossaries

- Treatment: **SPLIT**
- Direct files: **24**
- Descendant files: **24**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`
  - `TARGET\[80] Operations\[30] Maintenance\[10] Change and Maintenance`

### [05] Documents\Documents - Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [06] Spreadsheets

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **22**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [06] Spreadsheets\09.Desire Discovery

- Treatment: **SPLIT**
- Direct files: **5**
- Descendant files: **7**
- Proposed destinations:
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [06] Spreadsheets\09.Desire Discovery\00.Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [06] Spreadsheets\09.Desire Discovery\00.Resources\_Errata Sources

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [06] Spreadsheets\10.Requirements Definition

- Treatment: **SPLIT**
- Direct files: **9**
- Descendant files: **13**
- Proposed destinations:
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [06] Spreadsheets\10.Requirements Definition\01.RESOURCES

- Treatment: **SPLIT**
- Direct files: **4**
- Descendant files: **4**
- Proposed destinations:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`
  - `TARGET\[30] Discovery\[50] Requirements\[30] Quality Requirements`

### [06] Spreadsheets\31.Risk Report

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[30] Discovery\[30] Stakeholders\[10] Stakeholders Personas and Journeys`

### [aa] Outputs

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **614**
- Proposed destination:
  - `TARGET\[00] Management\[10] Repository\[10] Indexes and Navigation`

### [aa] Outputs\41.Requirements

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [aa] Outputs\41.Requirements - General

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **8**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [aa] Outputs\41.Requirements - General\99.Archive

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **7**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [aa] Outputs\41.Requirements - General\99.Archive\Reference

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **6**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [aa] Outputs\41.Requirements - General\99.Archive\Reference\NFRs

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[30] Discovery\[50] Requirements\[10] Business and User Requirements`

### [aa] Outputs\41.Requirements - General\99.Archive\Reference\NFRs\Reviews

- Treatment: **MERGE**
- Direct files: **4**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [aa] Outputs\42.Requirements - Functional

- Treatment: **SPLIT**
- Direct files: **3**
- Descendant files: **3**
- Proposed destinations:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\43.Requirements - NonFunctional

- Treatment: **SPLIT**
- Direct files: **6**
- Descendant files: **6**
- Proposed destinations:
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [aa] Outputs\51.SAD

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **596**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [aa] Outputs\51.SAD\00.Guidance

- Treatment: **SPLIT**
- Direct files: **2**
- Descendant files: **2**
- Proposed destinations:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [aa] Outputs\51.SAD\01.Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **0**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [aa] Outputs\51.SAD\02.Diagrams

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **593**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`
  - `TARGET\[50] Design\[60] Technology\[10] Platforms and Infrastructure`
  - `TARGET\[60] Delivery\[30] Data and Content\[30] Content Media and Localisation`
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[60] Client Applications\[20] Mobile Clients`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service

- Treatment: **SPLIT**
- Direct files: **13**
- Descendant files: **49**
- Proposed destinations:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`
  - `TARGET\[50] Design\[20] Information\[10] Information Architecture`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[50] Design\[50] Assurance\[10] Security and Assurance Design`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\01.0.TEMPLATE FOLDER

- Treatment: **SPLIT**
- Direct files: **23**
- Descendant files: **23**
- Proposed destinations:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`
  - `TARGET\[60] Delivery\[30] Data and Content\[30] Content Media and Localisation`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\05.Definition Views

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **6**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\05.Definition Views\000.Discovery View - Generic Org Requirements

- Treatment: **SPLIT**
- Direct files: **4**
- Descendant files: **4**
- Proposed destinations:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`
  - `TARGET\[50] Design\[30] Functionality\[10] Capabilities and Functions`
  - `TARGET\[50] Design\[60] Technology\[10] Platforms and Infrastructure`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\0TO DO FILE

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\51.Service Client View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\90.Appendices View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [aa] Outputs\51.SAD\02.Diagrams\21.Service\90.Appendices View\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[50] Design\[10] Architecture\[20] Architecture Descriptions`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **51**
- Proposed destinations:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\00.Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\00.Resources\99.LEGACY.SOURCE

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\07.Discovery View

- Treatment: **SPLIT**
- Direct files: **2**
- Descendant files: **3**
- Proposed destinations:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\07.Discovery View\02.MODULES

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\07.Discovery View\02.MODULES\01.Base

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\08.Requirements View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\09.Capabilities View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\20.Integration View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\30.Development View

- Treatment: **SPLIT**
- Direct files: **28**
- Descendant files: **28**
- Proposed destinations:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\32.User Interface Layout View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\40.Documentation View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\45.Testing View

- Treatment: **MERGE**
- Direct files: **6**
- Descendant files: **6**
- Proposed destination:
  - `TARGET\[60] Delivery\[70] Verification\[10] Component and System Testing`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\50.Security View

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\51.Privacy View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\31.Client\89.Appendices

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **41**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[60] Client Applications\[20] Mobile Clients`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **40**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`
  - `TARGET\[60] Delivery\[60] Client Applications\[20] Mobile Clients`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\00.Images

- Treatment: **MERGE**
- Direct files: **4**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\01.Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\02.Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\03.Concepts

- Treatment: **SPLIT**
- Direct files: **4**
- Descendant files: **4**
- Proposed destinations:
  - `TARGET\[60] Delivery\[60] Client Applications\[20] Mobile Clients`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\04.Categorisation

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\05.Guidance

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\06.Organisation

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\07.Flows

- Treatment: **SPLIT**
- Direct files: **10**
- Descendant files: **10**
- Proposed destinations:
  - `TARGET\[00] Management\[90] Review\[20] Temporary and Unsorted`
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\08.Shared Views

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\10.Module Views (System Base)

- Treatment: **MERGE**
- Direct files: **9**
- Descendant files: **9**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\32.Client Interface\User Interface Layout View\11.Module Views (Resources)

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[60] Client Applications\[30] User Interfaces`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **452**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **448**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template

- Treatment: **SPLIT**
- Direct files: **3**
- Descendant files: **45**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[60] Client Applications\[10] Web and Client Applications`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\00._Document View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\01._Context View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\02._Delivery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\03._Qualities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\04._Discovery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\05._Definitions View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\06._Capabilities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\07._Use Cases View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\08._Functionality View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\08._Functionality View\02._Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\08._Functionality View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\09._Interoperability View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\09._Interoperability View\02._Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\09._Interoperability View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\10._Information View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\10._Information View\02._Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\10._Information View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\11.Sequence View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\12._Integration View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\12._Integration View\02._Resources

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\12._Integration View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\13._Deployment View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\14._Development View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\15._Implementation View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\16._Transition View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\21._C&A View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\21.COMMON

- Treatment: **MERGE**
- Direct files: **0**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\00.Template\21.COMMON\02.00.Document View

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **219**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\00._Document View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\01._Context View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\02._Delivery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\03._Qualities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **9**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View\04._Classification

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\04.Discovery View\05._Discovery View (Desires)

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **9**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View\04._Categorisation

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\05.Definition View\05.Definition View (Requirements)

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **10**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View\04._Classification

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\06._Capability View\05._Capabilities View (HL)

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **54**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\00.Images

- Treatment: **SPLIT**
- Direct files: **23**
- Descendant files: **23**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\04._Classification

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\05.Functionality View (Use Cases) (HL)

- Treatment: **SPLIT**
- Direct files: **24**
- Descendant files: **24**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\07.Use Cases View\06.Functionality View (Use Cases)

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\08.Functionality View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **12**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\08.Functionality View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\08.Functionality View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\08.Functionality View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\08.Functionality View\02._Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\08.Functionality View\03.Functionality View (Classification)

- Treatment: **MERGE**
- Direct files: **4**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\08.Functionality View\04.Functionality View (Use Cases)

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **39**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\04._Classification

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\05.Interoperability View (APIs)

- Treatment: **SPLIT**
- Direct files: **31**
- Descendant files: **31**
- Proposed destinations:
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\09.Interoperability View\06.Interoperablity View (Messages)

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **34**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\02.Resources

- Treatment: **SPLIT**
- Direct files: **2**
- Descendant files: **3**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\02.Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\04._Classification

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\05.Information View (Overview)

- Treatment: **SPLIT**
- Direct files: **10**
- Descendant files: **10**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\10.Information Views\06.Information View (Entities)

- Treatment: **SPLIT**
- Direct files: **14**
- Descendant files: **14**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[20] Configuration Storage and Caching`
  - `TARGET\[60] Delivery\[40] Core Service\[30] Identity Access and Sessions`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`
  - `TARGET\[60] Delivery\[90] Operational Enablement\[30] Diagnostics and Health`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **18**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View\01._Document

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View\02._Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View\04._Classification

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\11.Sequence View\05.Sequences View (Sequences)

- Treatment: **SPLIT**
- Direct files: **8**
- Descendant files: **8**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **9**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View\02._Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View\02._Resources\01._Legacy

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View\04._Categorisation

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\12.Integration View\05.Integrations View (Integrations)

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **15**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\00._Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\01._Document

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\02.Resources

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\02.Resources\01.Legacy

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\03._Concepts

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\04._Categorisation

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\05.Development Views (Constraints)

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\06.Development Views (Patterns)

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\08.Development Views (Services)

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\14._Development View\09.Development View (Models)

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\20.System Base\21._C&A View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **62**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\00._Document View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\01._Context View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\02._Delivery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\03._Qualities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\04._Discovery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\05._Definition View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\06._Capabilities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\07._Use Cases View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\08._Functionality View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\09._Interoperability View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\10._Information View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\11._Sequence View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\12._Integration View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\13._Deployment View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\14._Development View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\15._Implementation View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\16._Transition View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\21._C&A View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\Untitled folder

- Treatment: **SPLIT**
- Direct files: **5**
- Descendant files: **25**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\Untitled folder\342.00.100.Functionality View

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\Untitled folder\342.00.121.Media LM - Development Views

- Treatment: **SPLIT**
- Direct files: **5**
- Descendant files: **5**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[50] Integrations\[20] Messaging and Events`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\Untitled folder\Context View

- Treatment: **MERGE**
- Direct files: **5**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\Untitled folder\Information View

- Treatment: **MERGE**
- Direct files: **6**
- Descendant files: **6**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\22.Media\Untitled folder\Sequence Views

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources

- Treatment: **SPLIT**
- Direct files: **0**
- Descendant files: **47**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\00._Document View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\01.Context View

- Treatment: **SPLIT**
- Direct files: **3**
- Descendant files: **3**
- Proposed destinations:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`
  - `TARGET\[60] Delivery\[40] Core Service\[40] Registries and Work`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\02._Delivery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\03._Qualities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\04._Discovery View

- Treatment: **MERGE**
- Direct files: **6**
- Descendant files: **6**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\05._Definitions View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\06._Capabilities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\07.Use Cases View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **5**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\07.Use Cases View\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\07.Use Cases View\044.9.Discovery View - #Operations

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[80] Operations\[10] Service\[10] Operation and Support`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\08._Functionality View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\08._Functionality View\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\09._Interoperability View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\10._Information View

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **4**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\10._Information View\00.Images

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **1**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\11._Sequence View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\12._Integration View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\13._Deployment View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\14._Development View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\15._Implementation View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\16._Transition View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\23.Resources\21._C&A View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People

- Treatment: **MERGE**
- Direct files: **1**
- Descendant files: **37**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\00._Document View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\01._Context View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\02._Delivery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\03._Qualities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\04._Discovery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\05._Definition View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\06._Capabilities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\07._Use Cases View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\08._Functionality View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\09._Interoperability View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\10._Information View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\11._Sequence View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\12._Integration View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\13._Deployment View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\14._Development View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\15._Implementation View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\16._Transition View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\24.People\21._C & A View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **38**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\00._Document View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\01._Context View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\02._Delivery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\03._Qualities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\04._Discovery View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\05._Definitions View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\06._Capabilities View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\07._Use Cases View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\08._Functionality View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\09._Interoperability View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[40] Interoperability and Discovery`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\10._Information View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\11._Sequence View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\12._Integration View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[50] Integrations\[10] APIs and Endpoints`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\13._Deployment View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\14._Development View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\15._Implementation View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[80] Release and Deployment\[20] Deployment`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\16._Transition View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[70] Transition\[50] Transition\[10] Cutover and Stabilisation`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\05.Modules\32.Subscriptions\21._C&A View

- Treatment: **MERGE**
- Direct files: **2**
- Descendant files: **2**
- Proposed destination:
  - `TARGET\[60] Delivery\[40] Core Service\[10] Components and Modules`

### [aa] Outputs\51.SAD\02.Diagrams\41.Modules\98.Legacy

- Treatment: **MERGE**
- Direct files: **3**
- Descendant files: **3**
- Proposed destination:
  - `TARGET\[90] Closure\[10] Retirement\[10] Planning and Exit`

## Review requirements before migration

1. Review every `SPLIT` source folder because its files will not move as one block.
2. Resolve every `REVIEW` placement using document content rather than filename alone.
3. Build an old-SELF-to-New-SELF coverage matrix and prove that every existing SELF entry is preserved, split, merged with traceability, or intentionally retired.
4. Regenerate the file-level `index-shown.md` from the approved target taxonomy.
5. Re-run collision and full absolute path-length checks with the final filenames.
6. Only then copy into `TARGET`; do not delete or move source material during the first migration pass.

## Interpretation

This register is exhaustive as a source-folder landing proposal, but it is not approval to migrate. Filename-based classification can demonstrate coverage and expose mixed folders; it cannot replace human review of ambiguous document meaning. The detailed Delivery hierarchy is intentional and must not be flattened back into a generic Development category.
