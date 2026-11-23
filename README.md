# Stakeholder Communications Playbook

How I communicate technical work to the people who have to decide on it —
business owners, engineers, reviewers, and leadership. The principle is
simple: a stakeholder should never have to reverse-engineer what you mean,
what you need from them, or what happens if they say no.

This is a personal playbook, drawn from real work: validating AI answers with
business owners, reviewing estimates with engineers, getting designs approved,
and writing status updates that people actually read. No client names, no
client material — just the patterns.

## Principles

1. **Lead with the decision, not the work.** The first line says what you
   need: approve, choose, confirm, or just know. The work behind it comes
   second.
2. **Show your evidence, not your confidence.** A number with its source, a
   claim with its test, a recommendation with its alternatives. Confidence
   without evidence is a request to be trusted; evidence lets them verify.
3. **Name what is unknown.** "No observed usage is unknown, not zero" applies
   to communication too. Say what you checked, what you couldn't check, and
   what would change the answer.
4. **Give the trade-off in their terms.** Latency vs. groundedness becomes
   "faster answers, more wrong answers." A vendor choice becomes "we own the
   maintenance, or we pay for it." Never ask a stakeholder to decide on a
   technical axis they don't own.
5. **Make the next step concrete.** Who does what, by when, and what happens
   if it slips. A message without a next step is a status report, not a
   request.
6. **Write it down, version it.** Decisions live in a log with the date, the
   decider, and the alternatives considered. A decision nobody can find later
   is a decision that gets re-litigated.

See `docs/principles.md` for the full write-up with examples.

## Templates

- `templates/status-update.md` — a weekly update people read in 60 seconds.
- `templates/decision-log.md` — one decision, with alternatives and owner.
- `templates/design-review-request.md` — asking for a design review, with
  the questions you actually need answered.
- `templates/review-request.md` — asking a reviewer to approve or request
  changes on a saved revision.
- `templates/incident-update.md` — telling stakeholders something broke, and
  what happens next.
