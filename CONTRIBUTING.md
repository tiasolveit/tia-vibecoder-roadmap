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
- A translation, or a better Arabic phrasing.
- A real number from your own product, with context.

## Translations

The English and Arabic versions hold the same content and must stay in sync.

- `en/` and `ar/` have matching filenames. Keep it that way.
- When you change a step in one language, change it in the other in the same
  pull request.
- Same number of steps, same order, same emojis, same "Done when" condition.
- Translate meaning, not word order. An awkward literal translation is worse
  than a short rewrite.
- Keep technical terms that developers actually search for in English: MVP,
  API, webhook, A/B test, JSON.
- Keep code blocks, filenames, and commands identical to the English file.
- Transliteration is fine when there is no good Arabic term, for example
  Supabase or Discord.

## Style guide

- **Markdown only.** The one exception is the `<div dir="rtl">` wrapper at the
  top and bottom of every file in `ar/`.
- **No em dashes.** Use a comma, a colon, or two sentences. This applies to
  every file, including this one.
- **One emoji per step title.** Keep it in the same position every time.
- **Each file is single language.** English files are fully English, Arabic
  files are fully Arabic. No mixed paragraphs.
- **Short lines.** Aim under 80 characters so diffs stay readable.
- **Professional tone.** Plain and direct. No hype, no filler.
- **Spellcheck your work** before you open the pull request.

### Arabic files and RTL

GitHub renders Markdown left to right by default, so Arabic files need one
wrapper to flip the layout:

```markdown
<div dir="rtl">

# عنوان الملف

المحتوى هنا.

</div>
```

Keep blank lines after the opening tag and before the closing tag, otherwise
Markdown tables and lists stop rendering. Never indent the content inside the
div, four spaces turns it into a code block.

## Step format

Every track step follows the same shape. Keep it consistent.

English:

```markdown
## 1. 🧠 The Idea

One line explaining what this step is and why it comes now.

**Done when:** a short, testable condition.
```

Arabic:

```markdown
## 1. 🧠 الفكرة

سطر واحد يشرح ما هو هذا الخطوة ولماذا تأتي الآن.

**ينتهي عندما:** شرط قصير وقابل للاختبار.
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
| `translate` | Arabic translations and RTL fixes |

Examples:

```
docs: clarify A/B testing step in builder track
fix: broken link to prompt basics in README
add: sample prompts for beginner track
translate: rework track 1 Arabic wording
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
