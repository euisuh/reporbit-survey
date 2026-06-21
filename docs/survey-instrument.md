# Survey Instrument v1

Exact question wording and flow. Target completion time: 5-7 minutes. Convert
to a Google Form / Typeform with this structure; do not reorder sections.

## Section 1 — Consent

See `consent-v1.md`. One checkbox, required.

## Section 2 — Demographics (~30s)

1. Name or pseudonym (optional, free text).
2. Years of programming experience (number, or buckets: 0-1 / 1-3 / 3-5 /
   5-10 / 10+).
3. "How confident are you in judging whether an open-source repository is
   well-managed?" (1-5: not at all confident → very confident).

## Section 3 — Repository items (repeated 2-3 times, one per assigned repo)

Each item is shown as:
- a header: "Repository {{letter}}" (A/B/C, re-randomized per respondent —
  never reveals the underlying repo identity or which pool slot it came from),
- the commit-graph snippet (blinded — see `assignment-protocol-v1.md`),
- the analytics panel (blinded — repo name/owner/contributor names stripped,
  real dates and counts kept).

Questions per item (identical wording every time — fixed task, not rotated):

1. "On a scale of 1-5, how well-managed does this repository appear?" (1-5,
   per the scale in `rater-guide-v1.md`)
2. "Which label best fits?" (single choice: healthy_active / stable_mature /
   chaotic_active / neglected / abandoned_or_deprecated / insufficient_evidence)
3. "How confident are you in this rating?" (0-1 slider or 5-point bucket)
4. "Did this repository's management change over time? If yes, roughly when,
   and what changed?" (free text, optional month field)

## Section 4 — Closing (optional)

5. "Any comments on what made a repository look well- or poorly-managed?"
   (free text, optional, skip-friendly)

## Pacing target

- Section 1: 30s
- Section 2: 30s
- Section 3 × 2 items: ~4 min (2 min/item)
- Section 3 × 3rd item (if included): +1.5-2 min
- Section 4: optional, 0-30s

If pilot timing on the first ~5 respondents runs over 7 minutes with 3 items,
drop to 2 items per respondent and increase total respondent count instead
(per `assignment-protocol-v1.md` Section 2, this keeps per-repo rating counts
roughly stable).
