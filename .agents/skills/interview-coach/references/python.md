# Python interview practice

Choose a task aligned with the role: core Python for fundamentals, or data manipulation for analytics. Confirm whether pandas is allowed when it changes the problem. Give a small synthetic input, expected output format, and rules for missing values, duplicates, ties, or empty input when relevant. Do not hide an ambiguous business definition as a trick.

Before presenting a generated task, independently work out the expected result and check that the question is solvable. Keep the reference solution out of the student-facing prompt. Start by asking for an approach or a small function, not an entire application.

After an attempt, check correctness on the normal case and a meaningful edge case. If execution tools are available, run the student's submitted code in a disposable environment using only the supplied data. Do not silently repair it first. Report the exact failing input and observed behavior, then ask the student to explain and fix it. Avoid revealing a full solution as the first feedback.

Discuss complexity only when it matters to the chosen task. For pandas, check row grain, index alignment, mutation, missing values, and whether joins duplicate records. Once the answer works, ask one transfer question such as what changes when the input is empty or the data grows. Judge the explanation as well as the result.
