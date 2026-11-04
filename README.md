# Student skills for planning and interview practice

Two reusable Codex skills for students. Use them to plan a realistic week and practice interviews through attempts, feedback, and revisions. Both work one step at a time and wait for your input.

| Skill | What it does |
| --- | --- |
| [Weekly Planner](.agents/skills/weekly-planner/SKILL.md) | Combines calendar commitments, homework, interviews, and priorities into a weekly plan, then revises it with you. |
| [Interview Coach](.agents/skills/interview-coach/SKILL.md) | Runs behavioral STARS, Python, SQL, and business case practice, one question at a time. |

These are instruction-based skills, not a standalone app. They use your existing Codex access; the repository does not require an API key or install Python dependencies.

## Start in this repository

1. Clone the repository. In Mac Terminal or Windows PowerShell:

   ```text
   cd ~/dso576
   git clone https://github.com/USC-DSO-576-YA/student-skills.git
   cd student-skills
   ```

   If you do not have `~/dso576`, use another existing folder you prefer.
2. Open the cloned `student-skills` folder as a project in Codex, or open it in VS Code and use Codex there. CLI users can run `codex` from this folder.
3. Start a new chat and use one of the prompts below. The repo's `.agents/skills` folder makes its skills discoverable when you work in this repository. In the CLI or IDE, type `$` to select a skill or use `/skills`. If a skill does not appear, restart Codex.
4. Answer the first question. The skill should wait for your response before advancing.

To use the skills in other projects, ask Codex:

```text
Use skill-installer to install weekly-planner and interview-coach from
https://github.com/USC-DSO-576-YA/student-skills.
Their folders are .agents/skills/weekly-planner and .agents/skills/interview-coach.
Do not overwrite an existing customized skill without showing me the differences.
```

Installing a skill does not connect accounts or schedule anything automatically.

## Plan your week

```text
Use $weekly-planner. Help me plan next week around my calendar,
homework, and interviews. Read my connected calendar if available.
Ask for any missing deadlines and time estimates. Show me a realistic
plan, then revise it with me. Do not add calendar events yet.
```

**Connect your own calendar:** Use your host's Plugins or connector settings to connect the calendar you use. Google Calendar, Outlook Calendar, and iCloud Calendar were listed in the plugin directory when this repository was prepared; availability and permissions can vary by account. Authorize your own account and select which calendar to use. The skill checks available tools rather than assuming a provider.

Without a connection, paste your availability and commitments. Homework may not be on your calendar, so supply assignment deadlines or relevant course files too. The skill does not automatically gain access to Brightspace, email, or other students' information.

A small starting example (fictional):

```text
My timezone is America/Los_Angeles. Plan the week starting November 9, 2026.
Classes: Monday and Wednesday 1–3 pm.
Homework: SQL assignment due Thursday at 11:59 pm; about 3 hours left.
Interview: Friday 10–11 am; I want 2 hours of Python practice beforehand.
I can study 2 hours each weekday evening. Keep Saturday free.
Please check what fits and ask me about anything missing.
```

Once satisfied, you can explicitly ask it to add the agreed study blocks to a named calendar. It should show the exact events, avoid duplicates, and report what was actually created. A weekly plan is not an automatic recurring reminder.

## Practice an interview

Choose one mode:

```text
Use $interview-coach for a behavioral interview for a business analyst role.
Use STARS. Ask one question, wait for my answer, then help me revise
my weakest part before moving on. Use only my real experiences.
```

```text
Use $interview-coach for a 20-minute beginner Python practice session.
Focus on lists, dictionaries, and functions. Give me one problem at a time.
Do not show the solution before I try; offer a hint if I get stuck.
```

```text
Use $interview-coach for an intermediate PostgreSQL interview.
Give me a small schema and sample rows. Start with joins and aggregation.
Wait for my query, check it, and let me fix it before the next question.
```

```text
Use $interview-coach for a business case about declining profit.
Reveal the case one stage at a time. Let me ask questions, calculate,
and recommend an action. Give feedback after each attempt.
```

Here, **STARS** means Situation, Task, Action, Result, and **So what** (reflection or learning). If your career coach uses another final S, tell the skill to use that version.

Default coaching cycle: **question → your attempt → specific feedback → your revision → reassessment**. You can ask for a hint, a full example, an easier question, or a stop at any time. For a more realistic mock interview, ask it to save feedback until the end. Session lengths are targets; the skill should not pretend to have timed you.

## Keep your information private

This repository is public. Do not commit resumes, calendar exports, credentials, interview stories, or personal practice results. Keep them in your private chat or a local `personal/` folder, which this repository ignores. Ignoring a folder is not encryption; anyone with access to your computer can still read it. Never force-add personal files to Git.

No calendar events, messages, or invitations are sent merely by installing these skills. The planner asks for a concrete calendar-write instruction before creating study blocks. Technical practice uses synthetic data, not a live company database.

## Customize and update

Read a skill's `SKILL.md` to see its instructions. Interview modes have separate references so only the relevant guidance is loaded. You can change the tone, practice difficulty, or planning preferences in your prompt without editing the files.

To get future updates, run `git pull` from the clone when your working tree is clean. Skills installed separately in your personal skill directory do not update just because this clone changes; update those through your installer too.

Maintainers: retain the one-step-at-a-time behavior, the no-fabricated-achievements rule, and the distinction between planning and calendar writes. Check changes against the scenarios in [VALIDATION.md](VALIDATION.md).

Skill discovery and installation guidance: [official Codex skills documentation](https://developers.openai.com/codex/skills/). Setup checked November 4, 2026.
