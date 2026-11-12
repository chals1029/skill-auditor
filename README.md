# Skill Auditor

Skill Auditor is an AI agent skill for evaluating whether another skill improves task outcomes. It guides an assistant through designing test cases, comparing runs with and without the target skill, and reporting evidence and limitations.

## What is included

- `SKILL.md` contains the instructions loaded by a compatible AI agent.
- The skill is instruction-only; it does not include an automated benchmark runner. A live comparison requires a suitable evaluation environment capable of isolating the baseline.

## Use

Install or copy this repository as a skill named `skill-auditor` in your agent's skills directory, following your agent's installation instructions. Then ask your assistant:

> Use Skill Auditor to evaluate my Visual QA skill.

If a fair comparison cannot be run, the skill instructs the assistant to report the blocker and provide a clearly labeled static audit instead of inventing results.
