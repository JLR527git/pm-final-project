# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
- **Persona (M2), who are you solving for?:** Frontline delivery driver
- **Primary success metric (M3), your leading indicator:** Time taken logging compliance checks. If reporting is streamlined and kept in the tool, coordinators should be able to close the gap between the time required to log checks in our tool vs. leading competitors.
- **Moment of misery (M2), the specific friction blocking the goal:** A routine delivery confirmation requires tapping through three screens, while unreliable route persistence, stale optimization, and offline failures force the driver to repeat actions or improvise instead of completing the job.
- **Guardrail metric (M3), what must not drop or break:** Usage of the live dispatch tool.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** B1 because of it's streamlining of a cumbersome process related to the moment of misery. B2 because of it's alleviation of the three click system for reporting from drivers. B5 because it keeps drivers and coordinators in sync throughout a route and is clear about advancement through steps.

## Audit, override & decide
AI OUTPUT:
# RouteLogic Velocity Initiative: Effort vs. Value Scoring

The scoring principle is simple: prioritize features that reduce the time and repeated actions a frontline driver needs to complete compliance checks, without undermining live dispatch usage. With a four-week pilot, three accounts, and a team of two engineers and one designer, anything that does not directly reduce this friction needs a strong justification to make the cut.

## 1. Feature scoring matrix

Quadrants use Value and Effort scores, with higher value being better and higher effort being worse.

- Quick Win: High value, low effort.
- Major Project: High value, high effort.
- Fill-In: Low value, low effort.
- Time Sinker: Low value, high effort.

| ID  | Feature                            | Value (1–5) | Effort (1–5) | Quadrant      |
| --- | ---------------------------------- | ----------- | ------------ | ------------- |
| B1  | One-Click Compliance Checklist     | 5           | 2            | Quick Win     |
| B2  | Smart Daily Report Auto-Fill       | 5           | 4            | Major Project |
| B3  | Shift Handoff Wizard               | 3           | 3            | Fill-In       |
| B4  | Mobile-First Coordinator Dashboard | 2           | 4            | Time Sinker   |
| B5  | Step Progress Indicator            | 2           | 1            | Fill-In       |
| B6  | Driver Alert Notifications         | 3           | 3            | Fill-In       |
| B7  | Contextual AI ETA Display          | 1           | 3            | Time Sinker   |
| B8  | Fleet Analytics Manager View       | 1           | 4            | Time Sinker   |
| B9  | Compliance Audit Trail Export      | 2           | 2            | Fill-In       |
| B10 | In-App Coordinator Training        | 1           | 2            | Time Sinker   |

## 2. Rationale for each feature

## B1

5 / 2

One-Click Compliance Checklist

Quick Win

Highest priority

Value 5 · Effort 2

Directly targets the 14.6-minute compliance step by pre-filling known data and reducing manual entry, making it the clearest path to improving the primary metric within the pilot.

## B2

5 / 4

Smart Daily Report Auto-Fill

Major Project

Value 5 · Effort 4

Automating report entry could eliminate duplicate compliance work and improve in-tool completion, but AI accuracy, validation, and integration make a full implementation risky for a four-week pilot.

## B3

3 / 3

Shift Handoff Wizard

Fill-In

Value 3 · Effort 3

The reported 6.8 minutes saved per day is meaningful, but handoff efficiency is secondary to the driver's immediate compliance friction and needs validation against the primary metric.

## B4

2 / 4

Mobile-First Coordinator Dashboard

Time Sinker

Value 2 · Effort 4

A coordinator-focused dashboard does not resolve the driver's three-screen confirmation flow and risks consuming most of the pilot on a broad interface redesign.

## B5

2 / 1

Step Progress Indicator

Fill-In

Value 2 · Effort 1

Showing workflow progress may reduce uncertainty and backtracking, but it does not remove compliance steps or materially reduce data-entry time on its own.

## B6

3 / 3

Driver Alert Notifications

Fill-In

Value 3 · Effort 3

Timely route-change and compliance alerts could prevent stale-route work and repeated actions, but notifications must be contextual and actionable to avoid interrupting drivers further.

## B7

1 / 3

Contextual AI ETA Display

Time Sinker

Value 1 · Effort 3

With just 11% current adoption and no direct connection to compliance logging time, improving ETA visibility is a weak use of scarce pilot capacity.

## B8

1 / 4

Fleet Analytics Manager View

Time Sinker

Value 1 · Effort 4

An executive analytics view primarily serves management and sales needs, rather than removing driver interactions or closing the compliance-time gap.

## B9

2 / 2

Compliance Audit Trail Export

Fill-In

Value 2 · Effort 2

One-click exports may reduce downstream coordinator and audit work, but they do not speed up the driver's initial compliance-check submission.

## B10

1 / 2

In-App Coordinator Training

Time Sinker

Value 1 · Effort 2

Training may improve coordinator proficiency, but the stated moment of misery is a workflow and reliability problem, not primarily a knowledge gap.

## 3. Recommended four-week pilot

With only two engineers, one designer, and one CS lead, I would resist running several independent feature tracks.

Commit: B1 — One-Click Compliance Checklist

Primary deliverable

Reduce the number of taps and manual fields using prefilled, editable data. Measure compliance logging time before and after deployment.

Investigate: B2 — Smart Daily Report Auto-Fill

Potential extension

Start with deterministic autofill from existing system data. Add AI only if it materially improves the workflow and can be validated safely.

Protect: Live dispatch reliability

Guardrail

Test that checklist changes do not disrupt dispatch usage, route persistence, or completion when connectivity is poor. Prioritize a narrow reliability fix if pilot evidence shows it is blocking compliance completion.

## 4. Define success before launch

| Measure            | Pilot approach                                                                                          |
| ------------------ | ------------------------------------------------------------------------------------------------------- |
| Primary metric     | Median elapsed time to complete and log a compliance check                                              |
| Baseline           | Capture current performance before changes across all three accounts                                    |
| Success criterion  | Set a measurable reduction target after reviewing baseline and competitor benchmarks                    |
| Guardrail          | Live dispatch usage must not materially decline                                                         |
| Diagnostic metrics | Taps per check, repeat submissions, completion failures, offline recovery, and route persistence errors |

Do not treat a reduction in screen count as success unless it reduces actual time to log compliance checks.

## 5. Strategic tensions to debate

- Speed vs. compliance integrity: Pre-filling information saves time only if drivers can verify it and required evidence remains accurate.
- Automation vs. reliability: AI-generated reports may appear valuable, but deterministic autofill is easier to validate and safer to deliver within four weeks.
- Driver value vs. buyer value: Dashboards and audit exports may appeal to managers or buyers, but the pilot should prioritize driver friction unless those features demonstrably affect compliance completion.
- Streamlining vs. dispatch adoption: A faster compliance flow is not a win if drivers must leave the live dispatch tool, lose their route, or repeat work after going offline.

Final recommendation: Fund B1 first, scope B2 as a potential extension, and use the pilot to establish whether the remaining time gap is caused by form entry or by underlying workflow reliability. Defer the management-facing features until there is evidence that they support the primary metric or protect the guardrail.

- **Where did you override the AI? (feature + old vs. new score + why):** The ai was actually fairly close to what I would have expected
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** It did not
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** It did not

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** B1
- **What I cut, and the “no” I’m protecting the scope from:** B3, B4, B7, B8, B9
- **Prototype/roadmap screenshot link (paste into your deliverables):** _(not filled in)_
<img width="2628" height="3325" alt="image" src="https://github.com/user-attachments/assets/a600f6ba-d4d2-4657-9fa3-6b8fb0dc0598" />
