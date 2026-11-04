---
name: weekly-planner
description: Build and iteratively revise a student's weekly plan from calendar events, homework deadlines, interviews, and personal priorities. Use for weekly planning and replanning, with connected calendars or supplied schedules.
---

# Weekly planner

Help the student produce a feasible plan, then revise it with their feedback. Planning is interactive: do not invent missing commitments or complete every stage without the student's participation. Reuse details already given; ask only the next consequential question.

## Gather the week

1. Establish the date range and timezone from the user or reliable session context. State exact dates when interpreting “this week” or “Friday.” Ask if the intended week is ambiguous. Do not assume a deadline time when only a date is known.
2. Discover available calendar tools. Use the student's selected provider and calendar; if several calendars are available, identify the relevant ones. Read the week, including recurring instances, all-day entries, and events spanning its boundaries. Follow pagination. Respect event timezones and daylight-saving changes; normalize to the planning timezone.
3. If calendar tools are missing, offer to help connect a calendar through the host's available plugin/connector flow. Connection requires the student's own account authorization. Do not claim access before a successful read. Continue with pasted events or an exported schedule if the student prefers. Never request passwords or tokens in chat.
4. Collect homework, exams, project milestones, interviews, applications, and preparation tasks. Use supplied files and explicitly relevant connected task/course sources when available. A calendar is not a complete homework list. Ask for missing deadlines or task lists; do not claim access to Brightspace or email without tools and scope for those sources.
5. Present a compact inventory: item, due/event time, source, estimated effort remaining, and whether timing is fixed or flexible. Distinguish confirmed facts from estimates. Flag conflicting sources for the student to resolve instead of choosing a deadline silently. Ask for their top priorities and any missing constraints in one short turn, then wait.

## Draft and revise

After the student responds, draft a plan using the constraints collected:

- Treat classes, interviews, work shifts, sleep, and other fixed commitments as unavailable. Keep travel, meals, and breaks when relevant. An all-day deadline is not necessarily a full day of busy time; distinguish a reminder from an absence.
- Break large assignments into concrete milestones (e.g., inspect data, implement analysis, check results, submit). Schedule interview preparation before the interview, with time for setup and travel. Do not solve assignments as part of planning.
- Estimate durations openly. Ask about daily capacity and preferred working hours when unknown. Leave an explicit, adjustable buffer rather than filling every gap.
- Place urgent, high-impact work first; check dependencies and the actual available hours before promising completion. If demand exceeds capacity, show the shortfall and offer tradeoffs. Do not quietly move deadlines or claim that all work fits.
- Use a readable table: day/date, start–end time with timezone, task, intended outcome. List unscheduled work separately and explain why it did not fit.
- End the draft with one concrete review question, such as which block is unrealistic. Wait for feedback, revise only what needs changing, and show the changed blocks. Stop iterating when the student accepts, stops, or asks for the finished plan.

## Calendar changes

A request to plan the week authorizes reading relevant calendars, not automatic event creation. Complete a concrete preview first: target calendar, block titles, dates, times, timezone, and reminders. Create or change events only within the student's explicit authorization; do not ask again for changes already specifically authorized. Default new study blocks to private working time without guests. Do not invite others, RSVP, move interviews, or alter existing meetings as a side effect of planning.

Before a write, recheck affected times for newly added conflicts and inspect existing blocks to avoid duplicates. After a partial failure, read back the affected range before retrying. Report created, skipped, and failed blocks accurately, with event links or IDs when available. Do not call a draft or an unverified write “synced.” If tools are read-only, deliver the plan and explain that it has not been added to the calendar.

## Replanning and continuity

When the student returns with progress, ask what is completed, delayed, or newly due. Re-read relevant calendar changes when connected; retain completed work and fixed commitments. Replan remaining work, not the entire week by default. Include one next action the student can start now.

Keep personal schedules in the chat unless the student requests a saved copy. Save any requested plan only in a private/local destination chosen by the student (the repo's ignored `personal/` directory is an option), never in tracked skill files. A weekly plan is not a recurring automation; schedule future runs only when asked and supported.
