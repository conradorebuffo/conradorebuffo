# Conrado Rebuffo

Systems and operations engineer. For the last decade I ran the accounting, billing and
inventory systems that small companies depend on — the kind of work where a wrong number is
someone's payroll. Since February 2026 I have been building the automation layer I always
wanted for that job.

## Konrad

A multi-agent orchestrator that runs my own operations: infrastructure, network devices,
business systems, security audits, knowledge capture. It plans work, executes it unattended
overnight, evaluates its own output with an independent read-only QA agent, and escalates to
me when it should not decide alone.

The parts I care about are not the agents, they are the guardrails:

- **Progressive autonomy** — every agent runs at one of four levels (`observer` → `advisor` →
  `assistant` → `partner`) behind a double lock: a global mode plus a per-agent ceiling.
  Nothing self-promotes.
- **Human checkpoints where they cost something** — queueing a plan *is* the approval.
  Outward-facing and irreversible actions (sending mail, opening a PR, contacting a person)
  are gated by design, not by convention.
- **Escalation paths that were actually exercised** — cross-provider fallback in two layers,
  a hang guard with early completion, Telegram alerts, and a rule against silencing errors
  that came out of a real four-month telemetry outage nobody noticed.
- **Everything is auditable** — commands, executions, costs, lessons and tool provenance all
  land in one database, because an automation you cannot reconstruct after the fact is not
  an automation, it is a rumour.

Six months in, from its own operational database: **124 unattended overnight executions,
89.5% completing without failure**, 740 of 803 overnight steps succeeded, mean independent
quality score 83.0 (n=277), 602 registered tools with a `draft → production` maturity ladder,
38,708 audited commands.

The repository is private. The numbers above come from its own instrumentation and I am happy
to walk through any of them.

## Before that

Eleven years of business systems for real companies, mostly unglamorous and mostly load-bearing:
ERP implementation and support (Tango, SAP Business One, ADempiere, OpenXava), accounting and
tax automation, receivables and payables, and a long tail of integrations with systems that
never had an API — which, in practice, is the same problem as integrating a partner portal.

Also incident response, including a ransomware case where the right answer was *not* to restore
the most recent backup but to reconstruct the timeline of the compromise first.

## Elsewhere

- LinkedIn: https://www.linkedin.com/in/conradorebuffo/
- Location: Córdoba, Argentina
