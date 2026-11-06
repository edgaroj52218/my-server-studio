# Lesson 01 · Conversation evidence

AI-drafted task summary, not a transcript or grade. It may be public. Use actual
short quotes or labeled paraphrases, name any help supplied, and link actual
work. Leave missing contributions Pending. A learner can review, correct or
remove excerpts before publication; accuracy approval is not proof of learning.
Label role-play honestly rather than treating it as an actual learner response.

**Lesson:** STUDIO-001. **Available conversation context:** Current coaching chat.

## Prediction

Learner quote: “DNS finds the server, Traefik grabs the connection, finds FastAPI
calculator, and returns it to page.” Given before the deployment plan; AI then
clarified that Traefik routes using the requested hostname.

## Check interpretation

Pending: the learner's own explanation of what the automated result establishes
and leaves open. AI supplied a hint and explained that the hosted API returned
42 for one multiplication request, while browser behavior and other inputs
needed separate evidence. This explanation is AI help, not learner reasoning.

## Browser observation

Learner quote after being asked to try 6 × 7 at
https://calc.edgarstevenojeda.site: “42 for both of them,” referring to Browser
result and API result. During initial DNS setup, the learner had reported a 404;
that earlier report is separate from this actual calculator observation.

## Keep decision

Learner quote: “I would keep this deployment because the calculator is functional
and shows the correct result for Browser Result and API Result.”

## Review

The learner reviewed the drafted excerpts before publication and replied:
“It seems accurate, let's move on forward.” This approves record accuracy;
the separate check-interpretation contribution remains pending.

For the later CI-results update, the learner requested an explanation and
authorized publication after it. AI explained the distinction between the
hosting tool checks, real-image/Chromium E2E, public runtime checks and the
learner's own browser observation. This is recorded as AI help, not a new
learner interpretation or proof of understanding.

## AI work and next step

AI helped with local setup, DNS/SSH guidance, Windows SSH compatibility fixes,
planning, evidence export and record drafting. The learner approved the plan
and ran launch/verify privately. Trusted HTTPS, release identity, API cases and
preservation of six existing containers passed within the recorded scope.
An optional own-image publication detour is linked in [SPEC.md](SPEC.md); the
learner subsequently chose the assignment's supplied image, which is deployed.

Native Windows fast checks failed on Unix-only interfaces. The prepared fast
checks then passed in a temporary local Linux Docker container: Black, Pylint,
96 tests; 2 E2E tests deselected, not passed locally. The hosting PR's
[full CI run](https://github.com/edgaroj52218/my-server-studio/actions/runs/42148748772)
then passed Black, Pylint, 96 non-E2E tests and 2 real-image/Chromium E2E tests.
The validate and integration-contract jobs also passed. CI evidence is separate
from the learner's browser observation and hosted runtime verification.
Actual technical reports and issue links are in [SPEC.md](SPEC.md),
[latest evidence](studio/evidence.json) and
[first-launch evidence](studio/launch-evidence.json).

Next: publish the reviewed record through the hosting PR and full CI.
The check-interpretation gap stays explicit.
