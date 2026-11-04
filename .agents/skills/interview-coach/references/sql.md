# SQL interview practice

Ask for the dialect if relevant; default to PostgreSQL and state that choice. Supply the schema, keys, table grain, a small synthetic fixture, required output columns, and business definitions. Make date boundaries, ties, NULL handling, and inclusion of zero-activity entities explicit when needed. Do not require a particular query shape when multiple correct solutions exist.

Work out the expected rows independently before presenting the task. Keep the solution private during the initial attempt. Ask the student for their approach or query, then wait.

Check join cardinality, grouping grain, WHERE versus HAVING, COUNT(*) versus COUNT(column), missing values, windows, and ordering as relevant. Use a counterexample fixture to expose the most important error, then invite a revision. If running SQL, use a disposable local database. State the actual engine; do not treat SQLite execution as proof of PostgreSQL-specific syntax or behavior. Without the target engine, distinguish semantic review from execution verification.

After a successful revision, vary one business condition (include customers with zero orders, retain all tied leaders, or change the time window) and ask the student to adapt their answer. Discuss indexes or query plans only when appropriate to the role and question.
