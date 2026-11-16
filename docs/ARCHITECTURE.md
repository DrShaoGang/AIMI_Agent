# System Architecture

## Overview

AIMI is organized as a three-stage metadata workflow:

```text
Existing metadata
       |
       v
Stage 1: Diagnose
  Readiness Agent -> Metadata Analysis Agent
       |
       v
Stage 2: Enhance
  Knowledge Retrieval Agent -> Metadata Enrichment Agent -> Validation Agent
       |
       v
Reviewed, standards-aligned metadata

Stage 3: Governance and dissemination spans the complete workflow.
```

## Stage 1: Diagnostic assessment

### Readiness Agent

The Readiness Agent evaluates records against measurable indicators such as:

- Identifier presence
- Schema completeness and conformance
- Structured field usage
- Controlled-vocabulary alignment
- Provenance completeness
- Suitability for coordinated agent processing

### Metadata Analysis Agent

The Metadata Analysis Agent performs deeper structural and semantic inspection. It identifies missing required elements, inconsistent field usage, ambiguity, and schema misalignment. Diagnostic outputs include the issue, its relative severity, and a recommended remediation priority.

## Stage 2: Structured enhancement

### Knowledge Retrieval Agent

The Knowledge Retrieval Agent grounds proposed improvements in authoritative sources. It supports vocabulary disambiguation, identifier matching, semantic mapping, and reproducible alignment with professional standards.

### Metadata Enrichment Agent

The Metadata Enrichment Agent converts diagnostic findings and retrieved knowledge into structured enhancements. It may populate missing descriptive elements, establish explicit relationships among entities, and create schema-compliant field values.

### Validation Agent

The Validation Agent checks generated changes for structural consistency, schema compliance, accuracy, and transformation quality. Validation feedback supports iterative refinement and routes uncertain or sensitive decisions to human review.

## Stage 3: Governance and dissemination

Governance is not a final checkpoint; it is a cross-cutting system layer. The project will formalize:

- Field-level modification permissions
- Confidence-reporting standards
- Decision-trace requirements
- Audit logging
- Criteria for human review
- Explanation interfaces
- Documentation and release practices

## Potential specialized agents

Subject to time and resources, the architecture may be extended with specialized agents for dataset-level descriptions, multimodal objects, spatial materials, audiovisual content, and research software. These extensions are considered additional activities rather than core deliverables.

## Implementation status

This document describes the proposed architecture. Detailed interfaces, schemas, deployment patterns, and technology decisions will be documented as implementation begins.
