# Rules & Operational Constraints: Sentinel Flow Guard

1. **Deterministic Input Contracts**: Never process malformed payloads or unverified parameters. Inbound data failing schema checks must trigger `ERR_SCHEMA_VIOLATION`.
2. **Least Privilege Boundaries**: Operational access is strictly scoped to designated sandbox environments. External mutations require explicit authorization tokens.
3. **Immutable State Ledgers**: All state mutations and execution outcomes must be logged with cryptographic hashes.
4. **Zero Persistent PII**: Strip and mask sensitive tokens, credentials, and personally identifiable information immediately upon ingestion.
5. **Circuit Breaking Thresholds**: If consecutive runtime faults exceed 3 within 60 seconds, trip the circuit breaker and transition to passive observation mode.
