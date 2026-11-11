---
name: linkedin-post-ideas
description: Keeps the user's bank of LinkedIn post ideas and plans what to post. Use when the user says "save a post idea", "post idea:", "add that to my post ideas", "show my post ideas", "what should I post this week", "plan my LinkedIn posts", or mentions something worth posting about and wants it kept for later.
---

# My LinkedIn post ideas

The ideas bank is `linkedin-posts/ideas.md` in the working folder. Create it
if it's missing, with the heading `# Post ideas` and one line explaining it.

## Saving an idea

Append one entry and confirm in a line:

```markdown
- <date> · <the idea in their words> · <topic from their profile, if one fits>
  Angle: <one line on what the post would say>
```

Keep their words. Don't draft the post unless they ask.

## Showing the ideas

List the unused ones, newest first, grouped by topic if there are more than
ten. Leave out ideas marked `used`.

## Planning the week

When they ask what to post:

1. Read `linkedin-posts/post-profile.md` (topics, reader, cadence),
   `linkedin-posts/ideas.md`, and `linkedin-posts/posted.md` if it exists.
   If they have a Claude brain, read `knowledge/my-business.md` and
   `knowledge/my-week.md` too.
2. Propose as many posts as their weekly cadence (default two), each with a
   working title and one line of angle. Spread them across their topics, and
   skip anything too close to a recent line in `posted.md`.
3. Prefer ideas from the bank. If the bank is thin, suggest fresh ones from
   their brain or profile: questions their clients ask, what they're focused on
   this year, the work only they can do.
4. Ask which to draft. Hand the ones they pick to the draft-linkedin-post
   skill.
