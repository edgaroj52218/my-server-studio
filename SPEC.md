# Lesson 01 specification

## STUDIO-001 · Launch a tested calculator on an existing server

**Status:** Supplied image launched and verified; local Linux fast checks passed. Prediction, browser observation, keep decision and accuracy review recorded; check interpretation and hosting GitHub completion remain pending.
**Next step:** Publish the reviewed hosting branch and complete PR/full CI while preserving the learner check-interpretation gap.
**Instructor implementation:** [issue #9](https://github.com/kaw393939/373_hosting/issues/9).
Create your own issue from the [lesson template](.github/ISSUE_TEMPLATE/studio-calculator.md).

## Agreed result

Launch the selected published calculator image through your existing Traefik
network and a nonconflicting HTTPS hostname. Preserve unrelated services and
host access. Do not add another proxy/updater or build a substitute image.
The [release selection](studio/calculator-release.json) supplies the expected
commit and image digest independently of the running website.
An explicitly agreed adoption of a matching existing deployment is recorded
as adoption, not a fresh launch. This bounded lesson does not certify the whole
server baseline or a vulnerability-free image.

- **Public hostname:** `calc.edgarstevenojeda.site` (learner selected).
- **New launch or adopted deployment, and reason:** Newly launched after explicit learner approval of the final plan. The preserved [first-launch report](studio/launch-evidence.json) records `launched`, `new_launch: true` and actual release checks.
- **Own issue / feature branch:** [Hosting issue #1](https://github.com/edgaroj52218/my-server-studio/issues/1); `codex/studio-001-calculator` (local).
- **Agreed scope or actual access/configuration gap:** Learner approved the supplied-image plan for existing `hosting-web`, preserving existing services. Launch and repeat verification passed; private server access stays in ignored settings. Full hosting CI/E2E remains pending.

The supplied release's exact image, commit, source and publication links are in
the [release selection](studio/calculator-release.json). The learner's separate
[application PR #1](https://github.com/edgaroj52218/is373_ci_cd/pull/1) and
[publication run](https://github.com/edgaroj52218/is373_ci_cd/actions/runs/42091003609)
were optional image-publication work; that image is not selected for this
assignment and its passing checks do not establish hosting completion.

Private SSH targets and configuration stay in ignored local state. Share only
reviewed, selected evidence; never commit credentials or raw server output.

## Evidence to keep

| Evidence | Actual result / link |
|---|---|
| Prepared Black/Pylint/pytest and real-image browser checks | Native Windows fast check failed on Unix-only OS/signal interfaces. Prepared fast check then passed on the laptop's existing Docker in an isolated Linux container: Black, Pylint and 96 tests passed; 2 E2E tests deselected, not passed. The container was removed. Hosting PR full CI/E2E remains pending. |
| Hosted image/commit, trusted HTTPS, valid and rejected API cases | Launch and repeat verification passed; [latest sanitized evidence](studio/evidence.json), [preserved first launch](studio/launch-evidence.json). Latest operation is `already-managed`, distinct from original creation. |
| Preservation of unrelated services | Launch report checked six existing containers unchanged for identity, state and published ports; broader behavior is outside this check. |
| Own prediction, check interpretation, browser observation and keep/revise reason | [LEARNING.md](LEARNING.md): prediction, observed 42 in both displays for 6 × 7, and keep reason recorded; check interpretation remains pending after AI hint/explanation. |
| Accuracy review before publishing learner excerpts | Learner approved the displayed draft before its first commit/push; see LEARNING.md Review. |
| Actual PR, latest CI, merge and issue closure | Pending |

Link the exported `studio/evidence.json`, actual CI and issue/PR when available.
CI does not deploy this server. A fixture, green check, timestamp, closed issue
or AI assertion alone does not establish the full result. `status` reports
recorded evidence and readiness for instructor review; it does not grade,
certify authorship or establish understanding.

## Optional instructor history

The records below are background, not steps to repeat. Their original anchors
remain here so earlier links continue to work.

## HOST-001 · Keep the Traefik dashboard private

[Historical requirement and evidence](book/changes/hosting-spec-history.md#host-001--keep-the-traefik-dashboard-private).

## HOST-002 · Controlled host maintenance

[Historical requirement and evidence](book/changes/hosting-spec-history.md#host-002--controlled-host-maintenance).

## HOST-003 · Companion image security maintenance

[Historical requirement and evidence](book/changes/hosting-spec-history.md#host-003--companion-image-security-maintenance).
