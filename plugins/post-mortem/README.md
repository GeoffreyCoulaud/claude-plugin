# Post-mortem

_Write blameless post-mortems interactively_. The agent interviews you one
question at a time and produces a structured markdown document.

## Installation

```sh
/plugin install post-mortem@bgcpm
```

## The problem

Post-mortems are hard to write well. Without guidance, they end up incomplete,
blame individuals, skip root cause analysis, or lack concrete corrective
actions. LLMs tend to generate the whole document in one shot without asking
clarifying questions, producing a generic template instead of a useful document.

## The fix

A depth-first, one-question-at-a-time interview where the agent extracts what
it needs from you. It covers all essential topics (timeline, impact, root cause
via 5 whys, corrective actions, lessons learned) and refuses to finalize without
an automated blameless review.

## The outcome

Two deliverables:
1. A complete, blameless post-mortem markdown document
2. A short communication message (for Slack or similar) with a link placeholder

## When to use it

After an incident has been resolved, when the team needs to document what
happened, why, and what to do about it. Works for any incident type: technical,
operational, organizational.
