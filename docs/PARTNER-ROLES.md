# Partner roles and execution boundaries

The first scenario is a hospital-style application ordering a synthetic AI reporting service. It is a technical federation experiment, not a clinical validation or a real patient service.

| Role | Proposed contribution | Execution planned for this run |
|---|---|---|
| Result / eEarly | Application requests an analysis and receives a result | Evaluate the public eEarly components for reuse. If they cannot run in this environment, use an explicitly labelled application simulator; do not claim an eEarly integration. |
| Villanova | Model service executes the requested job and returns its result and model version | Actual model inference on allocated Villanova GPU resources, subject to a pinned model and successful preflight. LAB service identities are ours. |
| SAP / Platform Mesh | Provider publication, subscriber binding and service discovery | Reuse our existing Platform Mesh example; assess a real KCP APIExport/APIBinding path before promising it. A simulated catalogue must be labelled as such. No SAP-operated marketplace or SAP billing connection is claimed. |
| FED8RA / Cotrugli–HashNET | Identity, mandates, work tracking, edge books, returned evidence and accounting | Reuse existing implementations and adapters. Record measured integration results without introducing a second rail sender. |

## Target topology

Start with three distinct LAB edge identities. Expand toward twelve only after a first strict FINAL and resource/isolation checks pass.

The twelve-edge target is three synthetic service chains. Each chain contains an application operator, a subscriber, an AI provider and a platform operator, each with its own identity and book. These identities do not impersonate actual organisations. Multiple AI-provider identities may share one model service; reports must disclose that shared infrastructure.

This validates logical separation and workload behaviour. Separate processes or namespaces on the same physical host are not independent physical failure domains.

## What we need from partners later

- Confirm one application process and the event fields it can provide.
- Review the server package, network route, local storage and operational responsibilities.
- Select the identity and mandate under which the organisation acts.
- Agree service acceptance, SLA, pricing and contribution rules.
- Run the same onboarding and verification steps in a partner-controlled installation.

No partner commitment is assumed by publishing this proposal.
