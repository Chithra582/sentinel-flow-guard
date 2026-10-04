---
name: "threat-signature-inspection"
description: "Scans payload vectors for known injection patterns and zero-day anomalies."
license: Apache-2.0
---

# Skill: Threat Signature Inspection

## Overview
Scans payload vectors for known injection patterns and zero-day anomalies.

## Execution Workflow
1. Validate incoming operational parameters and target identifiers.
2. Initialize sandboxed analysis harness and evaluate baseline metrics.
3. Apply domain-specific transformation logic and constraint verification.
4. Return standardized JSON response with status, latency, and telemetry payload.

## Error Handling
- Return `ERR_SKILL_TIMEOUT` if execution exceeds 5000ms.
- Return `ERR_VALIDATION_FAILURE` if parameters violate schema contracts.
