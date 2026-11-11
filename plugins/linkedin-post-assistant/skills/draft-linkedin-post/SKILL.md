---
name: draft-linkedin-post
description: Turns the user's notes into a LinkedIn post draft in their voice. Takes typed notes, a pasted voice-memo transcript, a client question, a story or an article, or picks from the user's saved post ideas. Never posts. Use when the user says "draft a LinkedIn post", "turn this into a post", "write a post about...", "draft my LinkedIn posts", "draft this week's posts", "make it shorter", "punchier opening", or "I posted it".
---

# Draft a LinkedIn post

Write a post the user would have written if they had the time. They copy,
edit and post it themselves. Never open LinkedIn.

## 1. Load what you know about them

- `linkedin-posts/post-profile.md` in the working folder: their topics,
  reader, goal, format rules, samples and "never" list. If it's missing,
  draft with plain defaults and end with: *"Say 'set up my post assistant'
  so posts sound more like you."*
- Their Claude brain, if the folder has one (`CLAUDE.md` with a `knowledge/`
  folder): read `CLAUDE.md`, `knowledge/my-voice.md` and
  `knowledge/my-business.md`.
- `references/writing-posts.md` in this skill's folder. Follow it.

## 2. Work out the input

| The user | Do this |
|---|---|
| Gave notes, a transcript, a story, a question or a link | Draft from that. For a link, read the page and write their take on it, not a summary. |
| Said "from my ideas" or named an idea | Use that idea from `linkedin-posts/ideas.md`. |
| Said "draft this week's posts" | Take as many ideas as their weekly cadence, choosing ones that cover different topics, and draft each. |
| Gave nothing | Ask: *"What's on your mind this week? A client question, something that happened, or a belief you'd argue for? Rough notes are fine."* |

If the notes are too thin to write without inventing something, ask **one**
question that gets the missing piece: *"What did you tell them?"*, *"How did
it turn out?"*

## 3. Write it

Follow `references/writing-posts.md`: two strong opening lines, one idea,
specific detail, short paragraphs, a plain ending, inside their length range.
Then run its "Before showing a draft" check.

## 4. Show it

```
Draft: <topic> (<n> words)

<the post>

Another opening to try:
> <alternative first two lines>

Check before posting: <anything to verify: a number, a name, permission,
firm approval>

Saved to linkedin-posts/drafts/<file>. Nothing was posted.
```

Leave out "Check before posting" if there's nothing to check.

## 5. Save it

- Write the draft to `linkedin-posts/drafts/<YYYY-MM-DD>-<short-topic>.md`,
  with a first line `Status: draft`.
- If it came from the ideas bank, mark that idea `used <date>` in
  `linkedin-posts/ideas.md`.
- If the notes held a second good idea, add it to the ideas bank and say so
  in one line.

## Edits and follow-ups

- **"Shorter", "punchier opening", "less formal", "say it like this...":**
  revise, show the new version, and update the saved file.
- **The user rewrites a phrase their own way twice** in one conversation:
  ask once, *"Want me to remember that for next time?"* If yes, add it to
  their post profile, or to `knowledge/my-voice.md` if they have a brain.
- **"I posted it":** set the file's status to `posted <date>` and add a line
  to `linkedin-posts/posted.md` (date, topic, opening line), creating the
  file if needed. That log keeps later ideas from repeating.
