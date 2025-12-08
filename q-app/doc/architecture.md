# Architecture Overview

The Career Coaching Assistant Q App consists of:

## 1. Amazon Q Business Application
- Core engine for LLM-based retrieval, RAG, and Q Apps.
- Includes admin guardrails and content filters.

## 2. Q App Workflow
- Input Cards:
  - Upload CV
  - Upload Job Description
  - Coach Notes
- Output Cards:
  - Skill Gap Analysis
  - Training Recommendations
  - Learning Schedule

## 3. Data Sources
### a. PDF Course Catalog
- Static catalog stored in Amazon Q Business storage.

### b. S3 Catalog
- Extended course catalogs stored in S3:
  - `/data/`
  - `/data/Medicine/` (restricted)
- S3 Data Source configured with daily sync.

## 4. Security & Access Control
- ACL file applied at S3 data source level.
- USER-level restriction:
  - career.coach.one → allowed
  - career.coach.two → denied

## 5. Guardrails
- Blocked keywords added to prevent harmful or irrelevant output.
