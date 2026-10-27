# Villanova-hosted FED8RA experiment — preparation opened 27 October 2026

**Status: PREPARING. The 48-hour clock has not started.**

| Item | State |
|---|---|
| Duration | 48 hours, plus separately reported finality drain |
| Target | 3 initial edge identities, scaling toward 12 after preflight |
| Data | Synthetic workload; no patient/customer data |
| Source candidate | 2026.10.20-rc3 |
| Existing edge and live rail | Already exercised in earlier runs; this run connects new instances |
| GPU inference | Preparation batch completed on two B200 GPUs; scored-run batches not started |
| GPU availability | Previous inference runs completed; new batches use the shared scheduler |
| CPU scheduler probe | Passed in preparation |
| Unprivileged network namespace | Available in preparation |
| Reachability to mTLS entry | Endpoint reached; unauthenticated request rejected |
| Source integrity / strict crypto availability | Passed in preparation |
| Packaging tests | 7/7 passed after adding test dependencies and public-key fixtures |
| Outbound transport from isolated edge namespaces | Network probe passed; mTLS endpoint correctly rejects a request without a certificate |
| Dedicated LAB identities and credentials | Separate identities prepared; connection activation pending |
| First event and strict FINAL from these new Villanova instances | Pending connection preflight |
| Co-Tru application integration for this run | Existing business-engine tests: 16/16 pass; integrated execution pending |
| Result application / catalogue integration | Explicitly simulated application and catalogue roles in this run |
| 48-hour start / end | Not set |
| Verdict | NOT RUN |

The existing live edge/rail capability is the foundation of this run. Preparation checks cover the new Villanova installation; the connected 48-hour run is still ahead. The first two test attempts lacked the test runner and then public-key fixtures; these setup failures were corrected before the seven-test pass. Runtime source files were not changed.

Next: complete isolated transport and assigned identities, qualify one event through strict FINAL, validate the connected business scenario, then record the actual topology and start the bounded run.

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

The new edge connection and first strict proof return are still pending. **No 48-hour result is claimed.**
