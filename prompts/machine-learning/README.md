# Machine Learning Prompts

### Model Selection Advisor
**Use case:** Choose an ML model for a business problem.
**Works with:** All LLMs

```text
Act as a senior machine learning engineer.

Recommend a model for:

[PROBLEM STATEMENT]

Context:
- Data type: [TABULAR/TEXT/IMAGE/TIME SERIES]
- Dataset size: [SIZE]
- Latency needs: [LATENCY]
- Interpretability needs: [NEEDS]

Compare baseline and advanced model options, then recommend a practical path.

Output format:
1. Problem framing
2. Candidate models
3. Recommended choice
4. Tradeoffs
5. Evaluation plan
```

### Training Pipeline Design
**Use case:** Plan an ML training workflow from data to deployment.
**Works with:** All LLMs

```text
Act as an ML platform engineer.

Design a training pipeline for:

[USE CASE]

Context:
- Input data: [DATA]
- Update cadence: [CADENCE]
- Deployment target: [TARGET]

Cover preprocessing, split strategy, training, validation, model registry, and
retraining.

Output format:
1. Pipeline overview
2. Training steps
3. Validation strategy
4. Deployment considerations
5. Failure modes
```

### Feature Engineering Assistant
**Use case:** Suggest useful features without leaking target information.
**Works with:** All LLMs

```text
Act as a senior data scientist.

Suggest features for this dataset:

[DATASET DESCRIPTION]

Context:
- Prediction target: [TARGET]
- Known features: [FEATURES]
- Constraints: [CONSTRAINTS]

Recommend feature ideas, transformations, and leakage checks.

Output format:
1. Feature ideas
2. Transformations
3. Leakage warnings
4. Prioritized next steps
```

### Evaluation Framework
**Use case:** Define how to measure ML model quality responsibly.
**Works with:** All LLMs

```text
Act as a machine learning evaluation specialist.

Create an evaluation plan for:

[MODEL OR USE CASE]

Context:
- Metric goals: [METRICS]
- Business impact: [IMPACT]
- Error tolerance: [TOLERANCE]

Include offline metrics, slice-based analysis, robustness checks, and monitoring
after deployment.

Output format:
1. Evaluation goals
2. Primary metrics
3. Secondary checks
4. Production monitoring plan
```

### Inference Optimization
**Use case:** Reduce model latency or cost in production.
**Works with:** All LLMs

```text
Act as an ML systems engineer.

Optimize inference for:

[MODEL / SERVICE]

Context:
- Runtime: [RUNTIME]
- Latency target: [TARGET]
- Cost constraints: [CONSTRAINTS]

Recommend batching, quantization, caching, model simplification, or serving
changes. Explain tradeoffs.

Output format:
1. Bottlenecks
2. Optimization options
3. Recommended plan
4. Risks and validation
```
