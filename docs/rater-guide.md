# Survey Rater Guide v1

Trimmed for a 5-7 minute, ~30-50 respondent informal survey (Issue #75). This is
a lighter version of `docs/evaluation/human-rater-guide-v1.md` (which remains
the rigorous protocol for the 2-3 trained-rater, 40-item gold set used in Paper
B). Differences from that guide:

- no required evidence bullets (too slow for this format),
- no pairwise task,
- one fixed free-text question instead of structured component judgments,
- intended for a broad pool of programmers, not 2-3 calibrated raters.

Treat this survey's results as a **plausibility check at larger n**, not a
replacement for the gold-set protocol. Report it in the paper as a distinct,
separately-described data source.

## What you are judging

For each repository shown, judge **repository management quality**: how well
the project appears to maintain its code and collaboration process, based only
on the commit-graph snippet and analytics panel shown. You will not see the
repository's name, owner, or code.

Consider: issues/PRs handled or left stale, review activity, CI/release/doc
signals, commit pattern, and whether inactivity looks stable or neglected.

Do not judge: whether you'd personally use the package, whether it's famous (you
won't know), or popularity by itself.

## Rating scale (1-5)

1. Unmanaged / abandoned / severely neglected
2. Weak management, clear process problems
3. Mixed or acceptable but inconsistent
4. Well-managed
5. Exemplary management

## Label (pick one)

`healthy_active` / `stable_mature` / `chaotic_active` / `neglected` /
`abandoned_or_deprecated` / `insufficient_evidence`

## Confidence (0-1)

0.0-0.3 sparse/contradictory evidence · 0.4-0.6 tentative · 0.7-0.8 clear ·
0.9-1.0 very clear.

## The change-over-time question

For each repository, answer: **"Did this repository's management change over
time? If yes, roughly when, and what changed?"** Free text, 1-2 sentences is
enough. "No noticeable change" is a valid answer.

## Important edge cases (same as the rigorous guide)

- Low activity is not automatically bad — a stable, finished library can be
  low-activity and well-managed.
- A solo-maintainer repo without a PR/review workflow is not automatically
  bad if its backlog is low.
- Missing analytics fields are not automatically bad — lower your confidence
  instead of assuming poor management.
- High activity is not automatically good — a busy repo with a growing,
  unresolved backlog can be chaotic rather than healthy.
