# Proposed SELF Repository Order

This is the working, text-based proposal for organising the repository. It is intended for review before any existing documents or media are moved.

## Core decisions

- Use decimal identifiers; do not use letters as overflow digits.
- Use dots between SELF hierarchy levels, for example `[50.20]`.
- Use square brackets to distinguish ordering and state metadata from the descriptive name.
- Let folders carry the SELF hierarchy.
- Let document filenames carry only their local order within the folder; do not repeat the folder's full SELF identifier.
- Treat documents as the primary folder contents.
- Store supporting diagrams, editable drawing sources, and exported images in `_media` beneath the relevant document folder.
- Prefer useful subject containment over mixing unrelated material, while avoiding repetition in descendant names.

## Proposed naming syntax

### Lifecycle folder

```text
[50] Solution Design
```

### Subject folder

```text
[50.20] Information Design
```

### Document

```text
[010 - DRAFT] Information Modelling Guidance.docx
[020 - REVIEW] Data Quality Guidance.docx
[030 - APPROVED] Information Architecture Guidance.docx
```

The document number is local to its containing subject folder. The filename does not repeat `50.20`, because that context is already supplied by the path.

### Supporting media

```text
[50] Solution Design/
└─ [50.20] Information Design/
   ├─ [010 - DRAFT] Information Modelling Guidance.docx
   ├─ [020 - REVIEW] Data Quality Guidance.docx
   └─ _media/
      ├─ 010-conceptual-model.drawio
      ├─ 010-conceptual-model.png
      ├─ 020-data-quality-model.drawio
      └─ 020-data-quality-model.png
```

Media may begin with the owning document's local number when this makes the relationship clearer. Media filenames do not need status metadata unless the media itself has an independently managed review state.

## Number widths

SELF hierarchy components use two digits because each level can contain up to 100 ordered positions:

```text
00 to 99
```

Document order uses three digits:

```text
010, 020, 030 ... 990
```

This provides substantially more insertion space. For example, a document inserted between `020` and `030` can be numbered `025`. The number is an ordering address, not a count.

Use wider initial gaps where growth is likely:

```text
050, 100, 150, 200
```

Use ordinary gaps where little growth is expected:

```text
010, 020, 030
```

Do not renumber established material merely to remove gaps.

## Proposed lifecycle groups

| Range | Lifecycle group | Scope |
|---:|---|---|
| 00 | Repository and cross-cutting management | Indexes, conventions, governance, decisions, risks, issues and shared management material |
| 10 | Environmental sensing and strategic direction | External drivers, opportunities, problems, policy direction, intended outcomes and strategic framing |
| 20 | Investment and project initiation | Funding, business cases, sponsorship, mandates, project preparation and governance setup |
| 30 | Discovery and solution definition | Context, stakeholders, needs, requirements, capabilities, constraints and definition of the problem |
| 40 | Procurement and selection | Procurement preparation, market engagement, response evaluation, selection and contracting |
| 50 | Solution design | Architecture, information, functionality, interfaces, security, infrastructure and operability design |
| 60 | Delivery and implementation | Delivery preparation, development, configuration, integration, testing, deployment and implementation |
| 70 | Operational readiness and transition | Readiness assessment, handover, training, release, service acceptance and transition |
| 80 | Operation and improvement | Service management, monitoring, support, maintenance, benefits, evaluation and continual improvement |
| 90 | Retirement and closure | Replacement, migration, decommissioning, records retention, closure and lessons learned |

## Initial subject order

The spacing is deliberate. It allows later subjects to be inserted without renumbering established paths.

### 00 Repository and cross-cutting management

- `[00.10] Repository Guidance`
- `[00.20] Governance and Decisions`
- `[00.30] Management Registers`

### 10 Environmental sensing and strategic direction

- `[10.10] Environmental Sensing`
- `[10.30] Problem and Opportunity`
- `[10.50] Strategic Framing`

### 20 Investment and project initiation

- `[20.10] Investment Framing`
- `[20.30] Financing`
- `[20.50] Project Initiation`

### 30 Discovery and solution definition

- `[30.10] Context Discovery`
- `[30.30] Stakeholders and Users`
- `[30.50] Requirements and Capabilities`
- `[30.70] Solution Definition`

### 40 Procurement and selection

- `[40.10] Procurement Preparation`
- `[40.30] Market Engagement`
- `[40.50] Evaluation and Selection`
- `[40.70] Contracting`

### 50 Solution design

- `[50.10] Architecture Direction`
- `[50.20] Information Design`
- `[50.30] Functionality and Interaction`
- `[50.40] Integration and Interfaces`
- `[50.50] Security Privacy and Assurance`
- `[50.60] Technology and Deployment`
- `[50.70] Operability and Support`

### 60 Delivery and implementation

- `[60.10] Delivery Preparation`
- `[60.30] Build and Configuration`
- `[60.50] Verification and Validation`
- `[60.70] Deployment and Implementation`

### 70 Operational readiness and transition

- `[70.10] Operational Readiness`
- `[70.30] Handover and Enablement`
- `[70.50] Transition`

### 80 Operation and improvement

- `[80.10] Service Operation`
- `[80.30] Maintenance and Change`
- `[80.50] Benefits and Evaluation`
- `[80.70] Continual Improvement`

### 90 Retirement and closure

- `[90.10] Retirement Planning`
- `[90.30] Migration and Decommissioning`
- `[90.50] Closure and Retention`

## State metadata

The proposed visible states are:

- `DRAFT` for incomplete material open to substantial change.
- `REVIEW` for material ready for structured review.
- `APPROVED` for material accepted as the current authoritative version.
- `SUPERSEDED` for retained material that has been replaced.

Example:

```text
[010 - DRAFT] Information Modelling Guidance.docx
```

Changing state will rename the file in Git. That is acceptable if state visibility is more valuable than path stability, but it should be a deliberate repository rule. Git will normally recognise a content-preserving rename, although links to the old path must still be updated.

## Migration constraint

Do not move existing repository material solely on the basis of this draft. First agree the lifecycle groups, subject order, naming syntax, permitted states, and `_media` convention. Then prepare a complete current-path-to-target-path mapping and review ambiguous or duplicate material before copying it into `TARGET`.
