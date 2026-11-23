# How I communicate with stakeholders

## The job of a technical message

A stakeholder message has one job: let the reader decide, correctly, without
having to do your work. That means every message answers four questions, in
order:

1. **What do you need from me?** (approve / choose / confirm / know)
2. **What is the situation, in my terms?**
3. **What is the evidence?**
4. **What happens next, and when?**

If the reader has to ask any of those back, the message failed — even if it
was technically complete.

## Translating trade-offs into business terms

Technical trade-offs are real, but stakeholders decide on business axes.
My job is the translation, honestly, in both directions:

- Latency vs. groundedness: "faster answers, more wrong answers — and here
  is the threshold where we held the release until the failures were fixed."
- Build vs. buy: "we own the pagination, retries, and on-call, or we pay a
  vendor and still own the canonical logic. Here is the one-week trial that
  decides it."
- Cost vs. quality: "this routing saves money on every call and skips the
  model entirely above a match threshold — here is what we measured."

The translation must not hide the cost. A trade-off presented as free is a
surprise waiting to happen.

## Validating with business owners, not just tests

An eval can pass while the answers are still wrong for the business. In a
knowledge-assistant project, I validated the golden question set directly
with the business owners who would live with the answers — because they are
the only people who can say whether an answer is right, not just grounded.
Automated evals measure the system; owners measure the truth. Both are
needed, and neither substitutes for the other.

The same applies to metric definitions: a "cost per completed issue" number
is meaningless until the owner agrees what counts as completed, what counts
as cost, and what to do with work that has no observed usage. I write the
definition down, with worked examples, and get the owner to agree to it
before building the calculation.

## Reviews that protect the reviewer

A review only works if the reviewer can trust what they reviewed. That means:

- The reviewer sees the exact revision they are deciding on. Later changes
  belong to subsequent work and do not rewrite that decision.
- The owner cannot review their own work. Assignment alone does not permit
  editing.
- Approved content is immutable. Changing it means reopening and creating a
  new revision — not a silent edit.

These rules sound bureaucratic. In practice they are what make a reviewer
willing to approve: they know the thing they approved is the thing that
ships.

## Status updates people read

A status update is not a diary. Sixty seconds, three parts: what changed
since last time, what is blocked and who owns the unblock, what happens next.
Numbers with sources, not adjectives. If nothing changed, say so in one line
and stop.

## When the news is bad

Bad news travels fastest when it is specific: what happened, who is affected,
what we know, what we don't know yet, what we are doing, and when the next
update comes. Never soften a fact to protect the reader — the delay costs
more than the discomfort. And never assign blame in a stakeholder message;
the message is about the fix, not the fault.
