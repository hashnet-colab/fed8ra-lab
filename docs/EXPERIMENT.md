# A 48-hour federation experiment

## One connected business process

1. A LAB AI provider publishes a versioned service, price and test SLA.
2. A LAB application discovers the service and orders under an existing mandate.
3. A bounded GPU job processes synthetic input and returns the result with the job ID and model version.
4. The application checks the result against explicit acceptance criteria.
5. Each party records its own actions through its existing edge. The shared rail receives the existing 32-byte objects.
6. The result's proof is retrieved and strictly verified, including a separate offline verification.
7. Accepted, eligible obligations enter the existing period-account and netting process. Settlement is a separate step; no money moves.

An initial workload is synthetic oximetry reporting. Test categories and numeric bindings are computed by code; the model writes a constrained report. These fixed test rules are not a medical diagnosis or clinical validation.

## Schedule and resource limits

- Preflight is outside the scored run: package pins, identities, route, trust, restart persistence and first FINAL must pass first.
- Start with three edge instances; expand toward twelve only when admission, isolation and resource measurements pass.
- The scored duration is 48 elapsed hours, with explicit UTC start/end timestamps. Do not reset the start to hide a failure.
- Use bounded scheduler jobs on compute nodes. No persistent services on the login node.
- GPU work is intermittent, within the owner's limit of four GPUs and approximately half the memory per GPU. CPU edge work continues between inference batches.
- Workload rate is measured during preflight, then fixed and recorded. There is no invented throughput target.
- Stop generation at the planned end; allow a separately reported finality-drain interval. Pending records remain pending if the drain deadline expires.
- Persist originals, books, checkpoints and evidence across scheduled process restarts. The run must not rely on a laptop or a long-lived SSH session.

## Controlled events

| Event | Required observation |
|---|---|
| Normal delivery | Correct job/result binding, acceptance and returned proof |
| Bad or incomplete result | Refusal or human-review state; no accepted obligation from a failed delivery |
| Mandate ceiling before/after restart | Existing authorised limits remain effective; prior spending is restored |
| Duplicate submission | Same event does not create a second booking or obligation |
| Same identity, changed content | Conflict is refused or held for review |
| Edge/process restart | The same book and unfinished job resume without replacement identities |
| Temporary transport outage | Pending remains visible, then recovers; no claim of immediate finality |
| Altered proof | Strict verification refuses it |
| Higher concurrency | Measure latency, memory, CPU, backlog and recovery without unbounded load |

Fault injection affects only this experiment's instances and routes. It never stops shared rail services or other users' jobs.

## Accounting

Close two explicitly defined 24-hour LAB accounting periods, or use the existing engine's UTC-day rule and report the resulting periods accurately. Do not change business rules merely to fit the clock.

Eligibility follows the existing acceptance and objection-window rules. If an obligation is not yet eligible at close, carry it forward and report it. A mandate's spending at order time is not the same total as accepted obligations eligible for netting.

Record gross obligations, eligible amounts, pending/disputed items, SLA credits where implemented, net positions and period identifiers. Test revenue-allocation rules must be explicit and conserve the distributable amount. If a backend allocation path is not connected, mark it NOT EXERCISED; a browser illustration is not a completed allocation.

## Human decisions

No model signs a Chamber decision. A reviewable case may be prepared using the existing process; opinions, recommendation and the authorised human decision remain separate. The run does not need an invented dispute to be useful.

## Completion

A useful result accounts for every offered job and event, retains failures, and links each verified result to its exact originals and software versions. A run may complete with findings. PASS requires its declared checks to pass; completion alone is not a passing verdict.
