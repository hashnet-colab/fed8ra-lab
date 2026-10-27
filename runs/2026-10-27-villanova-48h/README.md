# Villanova-hosted FED8RA experiment — preparation opened 27 October 2026

**Status: PREPARING. The 48-hour clock has not started.**

| Item | State |
|---|---|
| Duration | 48 hours, plus separately reported finality drain |
| Target | 3 initial edge identities, scaling toward 12 after preflight |
| Data | Synthetic workload; no patient/customer data |
| Source candidate | 2026.10.20-rc3 |
| CPU scheduler probe | Passed in preparation |
| Unprivileged network namespace | Available in preparation |
| Reachability to mTLS entry | Endpoint reached; unauthenticated request rejected |
| Source integrity / strict crypto availability | Passed in preparation |
| Packaging tests | 7/7 passed after adding test dependencies and public-key fixtures |
| Outbound transport from isolated edge namespaces | Pending |
| Dedicated LAB identities and credentials | Pending |
| First live event and strict FINAL | Pending |
| Co-Tru application integration for this run | Pending |
| Result application / catalogue integration | Pending selection and preflight |
| 48-hour start / end | Not set |
| Verdict | NOT RUN |

The preparation checks do not establish a live partner installation, business acceptance or a passing soak. The first two test attempts lacked the test runner and then public-key fixtures; these setup failures were corrected before the seven-test pass. Runtime source files were not changed.

Next: complete isolated transport and assigned identities, qualify one event through strict FINAL, validate the connected business scenario, then record the actual topology and start the bounded run.
