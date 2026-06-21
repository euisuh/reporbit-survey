# Survey Consent v1

Plain-language consent screen, shown before any survey question. Drafted as
Markdown for review now; convert verbatim to a Google Form intro page / PDF
before recruiting (Section "Conversion notes" at the end).

---

## RepOrbit Repository Management Survey — Consent to Participate

**What this is.** We are studying how programmers judge the management quality
of open-source repositories, and how well a short analytics summary plus a
commit-graph snippet supports that judgment. This is part of a research project
on visualizing and scoring repository health (RepOrbit).

**What you will do.** You will see 2-3 anonymized repositories (each shown as a
commit-graph snippet plus a small analytics panel — no repository name, owner,
or contributor names shown). For each one you will:
- rate how well-managed it appears (1-5 scale) and pick a label,
- say how confident you are in that rating,
- answer one short question about whether/when its management changed over time.

This takes about **5-7 minutes**.

**Voluntary participation.** Participation is voluntary and unpaid. You may
stop at any time without giving a reason, and may skip any question.

**Anonymity.** We do not collect your name unless you choose to provide one
(optional, for our records only). We collect your self-reported years of
programming experience and confidence rating. Your responses are stored
without any identifying link to you beyond what you optionally provide.

**Data use.** Responses are used in aggregate for research analysis and may be
referenced (in aggregate, anonymized form) in an academic paper. The identity
of the anonymized repositories shown to you will be disclosed in the published
research, but is not disclosed to you during the survey itself, to avoid
biasing your judgment with prior knowledge of the project.

**Risks.** We do not anticipate any risk beyond the time spent completing the
survey.

**Contact.** Questions about this research can be sent to:
`{{contact_email}}`

**Consent.** By continuing, you confirm that you are at least 18 years old, have
read the above, and voluntarily agree to participate.

[ ] I agree to participate.

---

## Conversion notes (for whoever builds the actual form)

- `{{contact_email}}` — fill in before publishing the form.
- If recruiting through a university account, confirm with your IRB/ethics
  office whether this qualifies for exempt review before distributing — this
  draft is written to be IRB-submittable but is not itself an IRB approval.
- Keep the consent screen as its own step; do not bury it inside the
  demographics page.
- If using Google Forms: set this as a section with one required checkbox
  question ("I agree to participate") and form-level setting "Collect email
  addresses: off" unless your IRB requires otherwise.
