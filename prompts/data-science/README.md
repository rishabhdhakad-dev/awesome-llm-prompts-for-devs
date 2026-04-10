# Data Science Prompts

### EDA Planner
**Use case:** Plan exploratory data analysis for a new dataset.
**Works with:** All LLMs

```text
Act as a senior data scientist.

Design an exploratory data analysis plan for:

[DATASET DESCRIPTION]

Context:
- Data source: [SOURCE]
- Business question: [QUESTION]
- Target audience: [AUDIENCE]

Include checks for missing data, outliers, distributions, correlations, and
target leakage. Recommend visuals and summary tables.

Output format:
1. EDA goals
2. Analysis checklist
3. Suggested charts
4. Risks and data quality checks
```

### Experiment Analysis
**Use case:** Analyze the result of an A/B or multivariate test.
**Works with:** All LLMs

```text
Act as a product data scientist.

Analyze this experiment:

[EXPERIMENT DETAILS]

Context:
- Primary metric: [METRIC]
- Guardrail metrics: [GUARDRAILS]
- Sample size: [SIZE]
- Runtime: [DURATION]

Interpret the result cautiously. Call out statistical concerns, bias, and
practical significance.

Output format:
1. Result summary
2. Statistical interpretation
3. Business impact
4. Caveats
5. Recommendation
```

### Data Cleaning Helper
**Use case:** Write a reliable data cleaning checklist or script logic.
**Works with:** All LLMs

```text
Act as a data engineer and scientist.

Create a cleaning plan for:

[DATASET]

Context:
- File format: [FORMAT]
- Problem areas: [MISSING VALUES / DUPLICATES / INCONSISTENCY]
- Downstream use: [USE CASE]

Recommend preprocessing steps, validation rules, and a final schema check.

Output format:
1. Cleaning plan
2. Validation rules
3. Risks
4. Optional code outline
```

### Visualization Advisor
**Use case:** Choose the right chart for a data story.
**Works with:** All LLMs

```text
Act as a data visualization expert.

Help me visualize this dataset or analysis:

[DATA OR QUESTION]

Context:
- Audience: [AUDIENCE]
- Tool: [TOOL]
- Message: [MESSAGE]

Recommend the best chart type, labels, annotations, and caveats.

Output format:
1. Recommended chart
2. Why it fits
3. Design tips
4. Pitfalls to avoid
```

### Metrics Dashboard Spec
**Use case:** Design a data dashboard for a product team or exec audience.
**Works with:** All LLMs

```text
Act as a senior data analyst.

Design a dashboard for:

[PRODUCT OR TEAM]

Context:
- Core KPIs: [KPIS]
- Audience: [AUDIENCE]
- Refresh cadence: [CADENCE]

Define the layout, metric definitions, filters, and alert thresholds.

Output format:
1. Dashboard goals
2. Key panels
3. Metric definitions
4. Refresh and alerting notes
```
