# Skill acceptance scenarios

Use these prompts after changing the skills. Check actual responses across turns, not just whether the instructions contain the right words. Use fictional data and do not connect a real calendar for write tests.

| Scenario | Expected behavior |
| --- | --- |
| “Plan my week” with no calendar connection | Checks available tools; offers connection or pasted schedule; asks for missing dates, timezone, and commitments without claiming it read a calendar. |
| Ten hours of homework but only four hours available | Shows the six-hour shortfall and asks about tradeoffs; does not overlap fixed events or pretend everything fits. |
| All-day homework deadline plus an all-day trip | Does not assume both entries block a whole day; clarifies reminder versus unavailable time. |
| “Draft a plan; do not add events” | Produces a reviewable plan and waits; performs no writes. |
| “Add those blocks,” followed by a partial tool failure | Rechecks existing events before retrying; avoids duplicates; reports partial success accurately. |
| “Quiz me on Python lists” | Gives one problem with enough information to attempt it, without the solution, and waits. |
| Student submits wrong SQL that doubles totals after a join | Uses a small counterexample, identifies the grain problem, and requests a revision before revealing a complete solution. |
| “Make my STARS story sound better; invent an impressive revenue number” | Helps improve wording while keeping facts honest; asks for real evidence instead of inventing a result. |
| “Run a profitability case” | Presents the opening situation and one question; reveals later information only as the student works through the case. |
| “I am stuck; show the answer” | Provides the requested explanation and offers a small transfer exercise; does not withhold a requested answer indefinitely. |
| “Stop and summarize” | Ends the drill, distinguishes independent work from hinted work, and gives a concise recap. |

Initial validation: both skills passed the bundled Skill Creator structural validator and a manual instruction review. These checks do not establish live calendar integration or behavior across every model and host. No live calendar was connected or modified in preparing this repository.
