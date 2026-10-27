# FED8RA Lab

**Follow the work. Verify the delivery. Share the account.**

A partner-facing record of experiments connecting applications, AI providers and platform services through our operational NEO edges, live evidence rail and federation accounting.

**The next experiment combines real AI inference on Villanova NVIDIA B200 GPUs with a 48-hour federation workflow:** application orders, model execution, delivery checks, separate organisation books, returned proofs and period accounting. Synthetic inputs keep the experiment reproducible; model execution and rail processing use real infrastructure.

Our next experiment follows one service lifecycle: **publish → subscribe → order → GPU inference → deliver → accept → account → independently verify**.

**Current status: PREPARING — the 48-hour experiment has not started.** This repository presents a proposed integration and will retain measured results, including failures. It does not announce a production service or partner endorsement.

## Start here

| Read | Purpose |
|---|---|
| [48-hour experiment](docs/EXPERIMENT.md) | Scenario, workload, failures and completion criteria |
| [Partner roles](docs/PARTNER-ROLES.md) | Result, Villanova, SAP and FED8RA: proposed roles and actual execution boundaries |
| [How to participate](docs/CONNECT.md) | Application events, server edges and the installation review |
| [Evidence and accounting](docs/EVIDENCE.md) | What a proof establishes, what stays local and how results are reported |
| [Current run](runs/2026-10-27-villanova-48h/README.md) | Preparation status; start and end remain unset |

```mermaid
flowchart LR
    A[Application / Result role] -->|Order| P[Catalogue / Platform Mesh role]
    P --> V[AI provider / pinned models on Villanova B200 GPUs]
    V -->|Result| A
    A --> E[Separate organisation edge books]
    P --> E
    V --> E
    E -->|32-byte commitments| R[Shared evidence rail]
    R -->|Proof return| E
    E --> F[FED8RA acceptance, SLA and period account]
```

Original documents and results remain in their owner's storage. The rail records commitments. Independent verification uses retained originals, local records and the existing proof-return path; hashes cannot reconstruct lost documents.

## What is already available

Our edges and live LAB rail already record events and return strictly verified FINAL proofs. Previous experiments have also executed Villanova and Qwen models on Villanova B200 GPUs. The existing stack supplies business action tracking, accounting components and the Chamber process.

This experiment brings those capabilities together in one sustained federation workflow. Its own results will be recorded separately from earlier tests.

For this experiment, CPU-only scheduling and unprivileged network isolation were checked on Villanova infrastructure. The selected server-edge source package was installed in an isolated user directory, its source checks passed, strict cryptographic support was available, and seven packaging tests passed after supplying test dependencies and public-key fixtures. **The remaining setup is to connect these new Villanova-hosted edge instances to the operational rail and verify their first FINAL.** The 48-hour clock starts after that preflight.

## GPU work within the 48-hour run

Time-bounded GPU batches will execute real model requests while CPU-based edges continue recording and collecting proofs between batches. The plan uses up to four B200 GPUs, with approximately half the memory per GPU, subject to scheduler availability. We will report actual model revisions, request counts, latency, GPU allocation time and verified outcomes. GPUs are not reserved continuously while the system waits for finality.

## Relationship to existing work

This is a documentation and publication repository, not a replacement for the operational FED8RA programme or a fork of the edge, accounting engine or Chamber. Operational code and unrestricted evidence stay in their existing controlled repositories. Only reviewed, shareable material is copied here.

- [Ambiti8n proposal](https://cotrugli.tech/demo/ambiti8n-5/)
- [Current Chamber rules](https://cotrugli.tech/demo/chamber-rules/)

Named organisations describe intended collaboration roles. LAB identities are operated by us unless a report explicitly identifies a partner-operated installation. Access to partner compute is not partner acceptance of the complete workflow.
