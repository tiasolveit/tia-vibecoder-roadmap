# Prompt Basics

Read this before track 1. Ten minutes here saves you ten hours later.

## Why prompts matter

AI does not guess what you want. It reacts to exactly what you wrote. The same
model gives a useless answer to a lazy question and an excellent answer to a
specific one. The difference is not the model. It is the prompt.

Good news: prompting is a learnable skill, and the pattern below covers most
of what you need.

## The 4-part prompt formula

Every strong prompt has four parts. Missing one is why prompts fail.

| Part | Question it answers | Purpose |
|------|--------------------|---------|
| **Context** | What is the situation? | Grounds the answer in your reality |
| **Task** | What do you want done? | The single objective |
| **Rules** | What are the constraints? | Stops the wrong kind of output |
| **Output** | What format do you need? | Makes the result usable |

### Context

Not your whole life. Just what the AI cannot guess: who you are, what you are
building, what already exists, what you have tried.

> I am building a SaaS for freelancers. I am the only developer.

### Task

One objective. Not five. If you need five things, send five prompts.

> Suggest features I could add to help freelancers bill their clients.

### Rules

This is where quality comes from. Constraints force the model out of generic
territory. Include limits on scope, tone, cost, audience, and what to avoid.

> Keep each feature realistic for one developer to build in a weekend. Group
> them by freelancer type. Skip anything that needs a mobile app.

### Output

Say exactly what you want back: a numbered list, a table, a single paragraph,
JSON, a diff, a file. This is the step most people skip, and it is why their
answers are unusable.

> Return a numbered list grouped by freelancer type. One line per feature. No
> preamble, no closing summary.

## Example prompt

Here is the full formula applied to one real task.

```
Context: I am building a SaaS for freelancers who invoice clients monthly.
I am a solo developer using Next.js and Supabase. I have no budget for paid
APIs and no audience yet.

Task: Suggest 50 features the product could have.

Rules:
- Realistic for a solo developer to build in one sprint.
- Must work without paid third-party APIs.
- Group them by freelancer type (solo, agency, contractor).
- Include a mix of must-have and nice-to-have.
- Skip anything that requires a native mobile app.

Output: A clean numbered list grouped by freelancer type. One line per
feature. No preamble and no closing summary.
```

Notice the output section. Same request without it gives you an essay you have
to rewrite. With it, you get something you can paste into your notes.

## Tips

- **Be specific.** Replace "make it better" with "make the empty state show a
  call to action".
- **Give examples.** Show one input and one output you like. The model will
  match the pattern.
- **Ask it to think first.** Add "think step by step before answering" for
  problems that need reasoning. It improves accuracy on anything multi-step.
- **Iterate, do not restart.** Follow up in the same conversation. "Now shorten
  it", "now make it sound friendlier", "drop items 4 and 9". Context
  accumulates and you keep the good parts.
- **Push back.** If the answer is wrong, say what was wrong. One line of
  correction beats three new prompts.
- **Paste real code and real errors.** AI is far better when it can see the
  actual thing, not your description of it.

## Common mistakes

| Mistake | Why it fails | Fix |
|---------|--------------|-----|
| Vague prompts | Model fills the gap with the most average answer possible | Name the audience, the goal, and the limit |
| No rules | Model invents solutions that are too big, too slow, or too costly | Add three constraints you actually have |
| No output format | You get prose you must rewrite by hand | State the format and say "no preamble" |
| Five tasks at once | Each answer gets shallow | One prompt, one task |
| Restarting every time | You throw away useful context | Follow up in the same thread |
| Trusting the first draft | The first pass is a sketch, not an answer | Ask for a second, stricter pass |
| Not checking facts | The model is confident and sometimes wrong | Verify anything you depend on |

## Next

You are ready for track 1.

- [🟢 Track 1: Vibecoder Beginner](01-beginner.md)