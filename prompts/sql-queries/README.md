# SQL Queries Prompts

### SQL Query Optimizer
**Use case:** Improve a slow or inefficient query.
**Works with:** All LLMs

```text
Act as a senior database engineer.

Optimize this SQL query:

[YOUR QUERY]

Context:
- Database: [DATABASE]
- Table sizes: [TABLE SIZES]
- Indexes: [INDEXES]
- Goal: [FAST READ / WRITE / REPORT]

Identify bottlenecks, missing indexes, poor join order, and unnecessary
subqueries. Recommend a faster version and explain tradeoffs.

Output format:
1. Query summary
2. Performance issues
3. Optimized query
4. Index suggestions
5. Validation steps
```

### Query Explain Assistant
**Use case:** Understand what a complex query does before changing it.
**Works with:** All LLMs

```text
Act as a senior analytics engineer.

Explain this SQL query in plain English:

[YOUR QUERY]

Context:
- SQL dialect: [DIALECT]
- Business goal: [GOAL]

Break down the query step by step, including filters, joins, aggregations, and
final output columns.

Output format:
1. Plain-English explanation
2. Step-by-step breakdown
3. Edge cases
4. Suggestions to simplify
```

### Reporting Query Builder
**Use case:** Design a query for an operational or executive report.
**Works with:** All LLMs

```text
Act as a data engineer.

Write a SQL query for this report:

[REPORT REQUIREMENT]

Context:
- Database: [DATABASE]
- Time window: [WINDOW]
- Metrics: [METRICS]
- Dimensions: [DIMENSIONS]

Return a production-ready query with aliases, grouping, and safe date handling.

Output format:
1. Query
2. Assumptions
3. How to validate the result
```

### SQL Refactor
**Use case:** Clean up a messy SQL statement without changing results.
**Works with:** All LLMs

```text
Act as a senior database architect.

Refactor this SQL:

[YOUR SQL]

Context:
- Dialect: [DIALECT]
- Constraints: [CONSTRAINTS]

Improve readability, consistency, and maintainability while preserving the
result set.

Output format:
1. Refactored SQL
2. What changed
3. Why it is safer or clearer
```

### Data Integrity Check
**Use case:** Validate a query against business rules and edge cases.
**Works with:** All LLMs

```text
Act as a data quality engineer.

Review this SQL or data logic:

[YOUR SQL]

Context:
- Tables involved: [TABLES]
- Business rules: [RULES]

Check null handling, duplicates, joins, filters, and grouping logic for data
quality risks.

Output format:
1. Integrity risks
2. Broken assumptions
3. Recommended fix
4. Validation queries
```
