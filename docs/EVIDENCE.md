# Evidence, measurements and publication

## Proof boundary

A rail proof establishes inclusion of a committed record in the verified chain. It does not itself establish that the model's answer was correct, the service met an SLA, a human approved a claim, revenue was allocated or money was paid. Those claims require their own records and checks.

Originals remain in owner-controlled storage. A 32-byte hash cannot recover an original. Reconstructing a case requires the retained source, its local record and the existing lower/upper proof links, including the Chamber small book where applicable.

## Per-run report

Publish a reviewed report containing:

- UTC start, generation stop and drain end; exact software/model/configuration pins;
- actual topology and which roles were simulated;
- offered, refused, booked, pending and strictly verified counts, with units clearly separated;
- reconciliation from source events to book records to proof results;
- execution latency and proof latency as separate measurements;
- CPU, memory, disk, GPU allocation time and processing throughput;
- injected failures, timestamps, expected outcomes and measured recovery;
- period-account inputs, rules, results and exclusions;
- conclusions, unresolved issues and the precise scope of every PASS.

One event is not necessarily one period commitment or one seal. Never compare these counts as if they were the same unit. Old run totals remain attached to their own dates and versions.

## Publication rules

This repository contains no private endpoints, credentials, private keys, production records, real patient data or unrestricted operational logs. Synthetic evidence must be checked for embedded access information before publication.

Public verification packages, if published, need a manifest, checksums, instructions and independently obtained trust roots. A checksum alone is not an authenticity proof. If evidence cannot be shared, mark it available for controlled review rather than linking partners to inaccessible private files as if they were public evidence.

Never rewrite a failed run as a passing one. Corrections and reruns retain their provenance.
