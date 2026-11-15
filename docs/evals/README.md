# Evaluation reports

One page per phase gate (DEV-PLAN §8, TEST-PLAN §17): scope, what was independently verified, measurements with
their environment, and the limits of the acceptance. The technical lead writes and accepts each report. A page marked
**draft** has been assembled from the team's gate audits and is awaiting that acceptance.

**Build names and IDs.** Most pages record measurements made before release 17.0 (3 November 2026). The build names
they use, and the commit and image IDs they quote, are explained in [TEST-PLAN](../TEST-PLAN.md#build-names-and-ids).

| Gate | Phase | Page | State |
|---|---|---|---|
| 0 | Foundation | [gate-0.md](gate-0.md) | **reached** (2026-11-12): on 15b's evidence the four IDs and the CI gates pass (2026-10-12); the product owner approved the four documents, MS0, on 12 Nov 2026 |
| 1 | Walking skeleton | [gate-1.md](gate-1.md) | **reached** (2026-10-12), on 15b's evidence: 36 of 36 IDs pass, PERF-001 inside its target; the demo's change step isn't scripted |
| 2 | Robustness | [gate-2.md](gate-2.md) | **reached** (2026-11-12): on 15b's evidence 49 of 50 live IDs pass on their tests (2026-10-12), and the one condition, a soak that completes every end-of-run check, was met by cycle 17's 24-hour soak (1 to 2 Nov 2026) |
| 3 | Safety | [gate-3.md](gate-3.md) | **reached** (2026-10-12), on 15b's evidence, Docker mode: 20 of 20 live IDs pass (6 void with approvals); the demo's network half passed |
| 4 | Team | [gate-4.md](gate-4.md) | reached (2026-09-28) |
| 5 | Local-model quality | [gate-5.md](gate-5.md) | reached on 15b (2026-10-11): every local-model run passed, M6 met, the phase demo accepted |
| 6 | Extensions | [gate-6.md](gate-6.md) | reached (2026-09-27) |
| 7 | Channels | [gate-7.md](gate-7.md) | reached on c15 (2026-10-08) |
| 8 | Firecracker | [gate-8.md](gate-8.md) | reached on 15b (2026-10-11); PERF-012's microVM half (Gate 9's row) waived by the product owner; the microVM host-key test is a known gap |
| 9 | PRD metrics M1–M8 | [gate-9.md](gate-9.md) | reached on 15b (2026-10-11), with the product owner's waiver of PERF-012's microVM half |
| 10 | Agent teams | [gate-10.md](gate-10.md) | **draft for 18.0** (2026-11-15): the criteria and what decides each; agent teams experimental and off by default (PRD §12 item 32, 12 Nov 2026) and what that means for the verdict; the third 24 h soak with teams in its mix (15 to 16 Nov) to be filled; the evaluation read keep experimental; the October record kept below |
| 11 | Computer use | [gate-11.md](gate-11.md) | **draft for 18.0** (2026-11-15): the criteria and what decides each; the small items since 21 Oct closed or recorded (Caps Lock, Ctrl+A, the reader's frame, the paste-in limit, a changed cap's reach); the grounding evaluation of 14 Nov (coordinates stay off); the third 24 h soak with Desktop tasks in its mix (15 to 16 Nov) to be filled; the October record kept below |

Other measurements, kept current before each `main` update:

| Measurement | Page |
|---|---|
| Live provider suite (E2E-PROVIDER-014) | [providers.md](providers.md) |
| Agent waves (E2E-WAVE-001, E2E-WAVE-002) | [waves.md](waves.md) |
| Comparison with the open reference (E2E-CMP-003, PRD M6) | [comparison.md](comparison.md) |
| Agent teams: E2E-AGENTS-020 and the v1.1 evaluation (ADR-0034 proposal J), plan | [agent-teams.md](agent-teams.md) |
| Computer use: the grounding evaluation (ADR-0039), measured 12 and 15 Oct 2026 | [computer-grounding.md](computer-grounding.md) |
