# Sentinel Flow Guard (`sentinel-flow-guard`)

[![OpenGAP Specification](https://img.shields.io/badge/OpenGAP-v0.1.0-blue.svg)](https://opengitagent.org)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Agent Passport Validated](https://img.shields.io/badge/GitAgent%20Passport-Ready-emerald.svg)](https://app.hidevs.xyz/passport)

## Overview
**Sentinel Flow Guard** is an autonomous AI agent engineered for **DevSecOps / Real-Time API Pipeline Security & Payload Verification**. Built in compliance with the **OpenGAP v0.1.0** specification, the agent provides robust, deterministic decision loops, automated policy enforcement, and comprehensive auditability.

## Architecture & Lifecycle
```mermaid
flowchart LR
    Ingest[Input Intake] --> Filter[Policy Validation]
    Filter --> Engine[Core Agent Logic]
    Engine --> Output[Audit Ledger]
```

## Quick Start
```bash
# Clone the repository
git clone https://github.com/Chithra582/sentinel-flow-guard.git
cd sentinel-flow-guard

# Install dependencies
pip install -r requirements.txt

# Run agent service
python src/main.py
```

## OpenGAP Specification
- `agent.yaml`: Primary metadata, capability declarations, and tool bindings.
- `SOUL.md`: Persona definition, core directives, and behavioral profile.
- `RULES.md`: Deterministic constraints and operational boundaries.
- `DUTIES.md`: Core responsibilities and SLA guarantees.
- `EXPLAINABILITY.md`: Checkpoint 2 decision governance, data provenance, and limitation mitigations.
- `skills/`: Modular execution skills with YAML frontmatter.
- `tools/`: Schema-validated tool definitions.
