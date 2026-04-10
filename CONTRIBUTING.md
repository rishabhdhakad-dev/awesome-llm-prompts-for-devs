# Contributing

Thanks for helping improve `awesome-llm-prompts-for-devs`.

## Fork and Clone

1. Fork the repository on GitHub.
2. Clone your fork locally:

```bash
git clone https://github.com/<your-username>/awesome-llm-prompts-for-devs.git
cd awesome-llm-prompts-for-devs
```

3. Create a branch for your change:

```bash
git checkout -b feat/your-prompt-name
```

## Folder Structure

- `README.md` contains the project overview and the top-level prompt showcase.
- `prompts/PROMPTS_INDEX.md` is the category map for all prompt packs.
- `prompts/<category>/README.md` contains prompts for a single developer use case.
- Keep related prompts together in the same category folder.
- Use one prompt per section so they are easy to copy, search, and maintain.

Example structure:

```text
prompts/
  PROMPTS_INDEX.md
  code-review/
    README.md
  debugging/
    README.md
  architecture/
    README.md
  bash-scripting/
    README.md
  sql-queries/
    README.md
  data-science/
    README.md
  machine-learning/
    README.md
  interview-prep/
    README.md
```

## Prompt Template Format

Use the exact structure below for each prompt:

````text
### Prompt Title
**Use case:** one line
**Works with:** All LLMs / specific ones

```text
Full prompt text here with [PLACEHOLDERS] in brackets
```
````

Keep placeholders in square brackets so users can quickly adapt the prompt.

## Rules for Good Prompts

- Make the prompt specific to a real developer task.
- Set a clear role, such as "Act as a senior engineer".
- Include context fields like language, framework, scale, or constraints.
- Ask for an output format so the answer is structured.
- Prefer actionable guidance over vague advice.
- Keep the prompt reusable across projects whenever possible.
- Avoid prompts that are too broad, too short, or missing the final output shape.

## PR Title Format

Use one of these styles:

- `docs: add security review prompts`
- `feat: add debugging prompt set`
- `chore: improve README structure`

For larger additions, prefer:

`feat: add <category> prompt pack`

## Before You Open a PR

- Check that your markdown renders cleanly.
- Verify that the prompt text follows the repository template.
- Keep changes focused on one category or one documentation improvement.
- Update counts or links if you add new categories or rename files.

Thanks again for contributing.
