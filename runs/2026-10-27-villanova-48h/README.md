# Villanova-hosted FED8RA experiment — 27 October 2026

**Status: RUNNING. The scored clock started 27 October at 21:43:29 UTC.**

| Item | Observed / configured state |
|---|---|
| Generation window | 27 Oct 21:43:29 UTC → 29 Oct 21:43:29 UTC |
| Finality drain | Up to one additional hour, reported separately |
| Live edge instances | 12, with separate identities, books, queues and retained originals |
| Topology | Three logical business chains, four LAB roles each |
| GPU | Two B200 cards per intermittent batch; 50% memory per model server; serialized jobs |
| Schedule | 48 orders every four hours; 576 planned over 48 hours |
| Models | Qwen3-32B primary; Villanova-2B comparison; every delivery checked |
| Data / roles | Our synthetic LAB data and identities; Result/eEarly and SAP/Platform Mesh roles simulated |
| Candidate | Unchanged 2026.10.20-rc3 |
| Source/package checks | Source hashes verified; seven packaging tests passed |
| Connected preflight | 15/15 records strictly FINAL across three books |
| Real business preflight | Order → GPU execution → checked delivery → one accepted obligation |
| Independent verification | Three offline proof checks, original hashes and nine business-source digests passed |
| Negative proof controls | Changed seal, wrong edge and wrong content rejected |
| Retry/conflict controls | Repeated submission added no booking; changed content under same identity refused |
| First scored batch | 48 real GPU jobs completed; 47 deliveries accepted, one declared bad delivery rejected |
| Money / revenue allocation / human Chamber decisions | No money moved; allocation and Chamber decisions NOT EXERCISED |
| Verdict | IN PROGRESS — completion and PASS are separate |

This is a real infrastructure run using our LAB identities, not a claim of independently operated partner installations. Access to Villanova compute is not partner acceptance. GPU execution, separate local books and the operational rail are real. The run continues without the Mac.

The preflight is outside the 48-hour scored interval. Its independent verifications checked the retained original, local record and 4,605-seal chain from pinned genesis. All fifteen preflight records were FINAL before the scored clock began. New scored records have their own finality wait.

The fixed workload uses the existing Co-Tru business engine, mandate gate and objection window. Each batch contains one declared bad delivery which must be rejected. At +12h one test edge is restarted; at +24h one test tunnel is paused for 75 seconds. Shared rail services remain untouched. Later UTC-day accounts may still be awaiting the existing 24-hour objection window when the run ends.

Machine-readable [launch snapshot](status.json) is timestamped; it is not a live polling endpoint. Full results will preserve failures and pending records.

## GPU preparation result — 27 October

The finite preparation job completed at **21:12:48 UTC**, using two B200 GPUs and synthetic/public inputs. Model servers were stopped after completion. These results are outside the 48-hour scored run.

| Synthetic reporting task, category supplied by code | Qwen3-32B | Villanova-2B |
|---|---:|---:|
| Responses | 60 | 60 |
| All strict checks, including exact output template | 59 | 0 |
| Category appears exactly once and matches input | 60 | 11 |
| Request/transport errors | 0 | 0 |

This measures one deliberately narrow reporting contract, not general model capability or clinical accuracy. The planned primary business output is Qwen, with Villanova-2B retained for comparison. Every delivery is checked; a failed output does not create an accepted obligation.

Pinned revisions:
- Qwen/Qwen3-32B: `9216db5781bf21249d130ec9da846c4624c16137`
- VillanovaAI/Villanova-2B-2603: `18280c7836baee3ce26bf3d91dad9fff4b33b539`

The subsequent three-edge connection and business proof-return preflight passed. **The 48-hour run is ongoing; no final verdict is claimed.**
