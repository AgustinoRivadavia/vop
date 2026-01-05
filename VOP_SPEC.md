# Verified Origin Protocol (VOP) — Specification v1.0

## 1. Purpose
VOP defines a minimal, neutral protocol for recording and verifying
the declared origin of digital content.

## 2. Scope
This specification applies to digital media including but not limited to:
- video
- image
- audio
- text
- composite media

## 3. Design Principles
- Declaration over detection
- Origin over appearance
- Verification over judgment
- Minimalism and neutrality

## 4. Content Registration
A VOP registration consists of:
- a cryptographic hash of the content
- a timestamp
- a declared origin source
- optional metadata

No content files are stored by the protocol.

## 5. Origin Source Types
An origin source MUST be one of the following:

### 5.1 Generator
A content generation tool or system.
Example: Sora, DALL·E, Midjourney.

### 5.2 Entity
A human or artificial entity with a verifiable identifier.
Example: SIVS-000014.

### 5.3 Declared
An unverified or self-declared source.

## 6. Verification
Verification consists of recomputing the content hash and matching it
against registered records.

The protocol makes no claims beyond the existence of a matching declaration.

## 7. Non-Goals
VOP does not:
- detect AI-generated content
- assess authenticity or truthfulness
- rank or validate creators
- store or analyze media files

## 8. Security Considerations
VOP relies on cryptographic hashing to ensure content integrity.
Hash collisions are considered computationally infeasible.

## 9. Legal and Ethical Considerations
VOP records declarations and timestamps.
It does not assert authorship, truth, or ownership.

## 10. Versioning
This document defines VOP Specification v1.0.
Future versions MUST remain backward compatible.

---
Status: Draft
Author: AgustinoSape
