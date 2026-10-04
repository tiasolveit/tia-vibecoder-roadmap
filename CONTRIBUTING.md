# Contributing

Thanks for helping. This is a documentation repo, so contributions are mostly
writing, fixing, and translating.

## How to contribute

1. **Fork** the repo on GitHub.
2. **Clone** your fork locally.
3. **Create a branch** with a clear name.

   ```bash
   git checkout -b fix-beginner-step-4
   ```

4. **Make your change.** Keep it focused. One topic per pull request.
5. **Commit** using the format below.
6. **Push** and open a pull request against `main`.
7. Describe what you changed and why. Link the issue if there is one.

If you are not sure whether something belongs here, open an issue first and
ask. That is faster than writing something that does not fit.

## What is worth contributing

- A step that confused you.
- A broken or outdated link.
- A missing sample prompt for a step.
- A translation, or a better Arabic title.
- A real number from your own product, with context.

## Style guide

- **Markdown only.** No HTML unless there is no other way.
- **No em dashes.** Use a comma, a colon, or two sentences. This applies to
  every file, including this one.
- **One emoji per step title.** Keep it in the same position every time.
- **Arabic title, English body.** Step titles are short and in Arabic. The
  explanation under each title is one line, in English.
- **Short lines.** Aim under 80 characters so diffs stay readable.
- **Professional tone.** Plain and direct. No hype, no filler.
- **Spellcheck your work** before you open the pull request.

## Step format

Every track step follows the same shape. Keep it consistent.

```markdown
## 1. 🧠 Title in Arabic

One line in English explaining what this step is and why it comes now.

**Done when:** a short, testable condition.
```

## Commit messages

Use this format:

```
<type>: <short description>
```

Types:

| Type | Use for |
|------|---------|
| `docs` | Content changes |
| `fix` | Typos, broken links, wrong info |
| `add` | New steps, new files |
| `remove` | Deleting content |
| `refactor` | Restructuring without changing meaning |

Examples:

```
docs: clarify A/B testing step in builder track
fix: broken link to prompt basics in README
add: sample prompts for beginner track
```

Keep the subject line under 72 characters. Use the imperative mood.

## Code of conduct

Be kind. That is the whole rule.

- Assume good intent.
- Critique the work, never the person.
- No harassment, no insults, no dismissive comments.
- Beginners are welcome. Everyone was a beginner once.
- Disagree in the technical detail, then agree on the outcome.

If something happens that violates this, open an issue or contact the
maintainers directly. Reports are handled privately and seriously.