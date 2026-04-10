# Bash Scripting Prompts

### Bash Script Generator
**Use case:** Create a reliable shell script from a task description.
**Works with:** All LLMs

```text
Act as a senior DevOps engineer writing production-ready shell scripts.

Create a Bash script for:

[TASK]

Context:
- Operating system: [OS]
- Shell: [bash/zsh]
- Inputs: [INPUTS]
- Desired output: [OUTPUT]

Write safe Bash that handles errors, validates inputs, and uses clear
functions. Prefer portable commands and explain any non-obvious syntax.

Output format:
1. Script
2. Usage instructions
3. Safety notes
4. Assumptions
```

### Shell Debugger
**Use case:** Diagnose why a shell script is failing.
**Works with:** All LLMs

```text
Act as a senior shell engineer debugging this Bash script:

[YOUR SCRIPT]

Context:
- Error message: [ERROR]
- Expected behavior: [EXPECTED]
- Runtime environment: [ENVIRONMENT]

Find quoting bugs, subshell issues, variable expansion problems, and portability
issues. Recommend a safe fix and explain the root cause.

Output format:
1. Root cause
2. Broken lines
3. Corrected script
4. Verification steps
```

### Cron Job Builder
**Use case:** Build a cron-friendly command or script wrapper.
**Works with:** All LLMs

```text
Act as a senior systems engineer.

Design a Bash script that can run safely from cron:

[TASK]

Context:
- Frequency: [FREQUENCY]
- Log location: [LOG PATH]
- Retry policy: [POLICY]

Handle locking, logging, exit codes, and environment differences between an
interactive shell and cron.

Output format:
1. Script
2. Cron entry
3. Logging strategy
4. Failure handling
```

### Text Processing Pipeline
**Use case:** Build a grep/sed/awk pipeline for log or file processing.
**Works with:** All LLMs

```text
Act as a senior Linux engineer.

Create a Bash pipeline for:

[PROCESSING GOAL]

Context:
- File type: [FILE TYPE]
- Input size: [SIZE]
- Required output: [OUTPUT]

Use standard Unix tools where appropriate. Keep the pipeline readable and
explain each stage.

Output format:
1. Pipeline
2. Explanation
3. Safer alternatives if needed
```

### Deployment Helper
**Use case:** Automate a common deployment or release step.
**Works with:** All LLMs

```text
Act as a release engineer.

Write a Bash script for:

[DEPLOYMENT TASK]

Context:
- Target: [TARGET]
- Credentials approach: [APPROACH]
- Rollback requirement: [YES/NO]

Include preflight checks, error handling, logging, and rollback guidance.

Output format:
1. Script
2. Preflight checklist
3. Rollback notes
4. Operational warnings
```
