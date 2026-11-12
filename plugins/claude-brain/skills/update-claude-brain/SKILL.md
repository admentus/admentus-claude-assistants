---
name: update-claude-brain
description: Reviews or changes the user's Claude brain (their CLAUDE.md and knowledge files in their Claude project, and what the project's memory has learned since). Use when the user says "update my brain", "remember that...", "add this to my brain", "my brain is wrong about...", "forget that...", "what do you know about me", "show me my brain", "refresh my brain", "update my project instructions", or asks Claude to keep a fact about their business, clients, voice or week for next time.
---

# Update or review my Claude brain

The brain lives in the user's Claude project:

- **The brain files** in the project's Context: `CLAUDE.md`, `my-business.md`,
  `my-people.md`, `my-voice.md`, `my-week.md`, `my-tools.md` and
  `interview-notes.md`.
- **The project's memory:** what they've told Claude since. Where memory and
  a brain file disagree, memory is newer and wins.
- **The project's Instructions:** a short version that points at the files.

If this chat isn't in their project, ask them to start it from the project's
page (**Projects** in the left sidebar, then the project). If the project has
no brain files, say so and offer: *"Say 'set up my Claude brain' and I'll
build it with you."* If the brain files are only in a folder (an older
setup), offer: *"Say 'move my brain into my project' and I'll put it where
every chat can read it."*

## Reviewing: "What do you know about me?"

Read `CLAUDE.md`, the other brain files except `interview-notes.md`, and the
project's memory. Summarize in plain bullets under short headings (your work,
your clients, your week, your people, how you write, how you want me to
work), with memory's version wherever it's newer. Don't recite the files.
Then ask: *"Anything to change?"*

## Remembering something: "Remember that..."

A fact, a preference or a correction goes in the project's memory.

1. **Show it first** in their words, one line, unless they told you exactly
   what to write.
2. **Save it to the project's memory.** One fact per line, dated.
3. **Removing something** ("forget that..."): confirm, then take it out of
   memory. If it's in a brain file too, note in memory that it no longer
   applies, so memory wins.

## A bigger change: "Update my brain"

A new service, a new client list, a rewrite of how they write: rewrite the
brain file it belongs to.

| It's about | File |
|---|---|
| what they sell, who they serve, how clients find them, goals | `my-business.md` |
| clients, partners, contacts | `my-people.md` |
| how they write, words to use or avoid, samples | `my-voice.md` |
| their week, time, priorities | `my-week.md` |
| their tools | `my-tools.md` |
| how Claude should work with them, always/never rules | `CLAUDE.md` |

1. **Show the change** before making it: the lines as they are and as they
   will be. Use their words.
2. **Write the new version** of the whole file, with anything memory knows
   about that subject folded in, and the date at the bottom.
3. **Put it in the project's Context.** If you can replace the file there
   yourself, do. If you can only add files, add the new version, then tell
   the user exactly which old file to remove from **Context** on the
   project's page. Two copies of one file confuse every chat until the old
   one is gone. If you can't add files at all, give them the file to add.
4. **Keep the Instructions in step.** If the change touches what the
   project's Instructions say (who they are, what they're focused on, how to
   work with them, how they write), give them the new paragraph from the
   template in the set-up-claude-brain skill's `references/templates.md`.
   Set it yourself if you can; otherwise they paste it over the old one.

## Refreshing: "Refresh my brain"

When memory has built up, fold it into the brain files: for each file memory
has news for, do steps 1 to 3 above. Then, with the user's OK, take the
folded-in lines out of memory. Offer this once if memory holds a lot of
brain facts; don't push it.

## The privacy rule still applies

The brain and memory are stored in the user's Claude account. Don't save
client account numbers, passwords, health information or confidential deal
terms, even if asked. Say why in one line and offer a safer version: *"I'll
save 'Dana, CFO at a 40-person distributor, our biggest client' instead."*

## Things worth offering to remember

When the user corrects a draft the same way twice ("don't say 'reach out'"),
or mentions a new client or offer, ask once: *"Want me to remember that?"*
Don't ask more than once per conversation.
