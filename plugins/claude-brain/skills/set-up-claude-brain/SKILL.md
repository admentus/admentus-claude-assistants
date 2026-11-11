---
name: set-up-claude-brain
description: Builds the user's Claude brain through a short interview. Asks about their work, clients, week, key people and writing, then writes a CLAUDE.md file and a knowledge folder that every other assistant reads. Use when the user says "set up my Claude brain", "build my Claude brain", "teach Claude about me", "interview me so Claude knows my business", "continue my Claude brain", or right after the Claude Brain plugin is installed.
---

# Set up my Claude brain

Interview the user, then write their brain: a `CLAUDE.md` file and a
`knowledge/` folder in the folder they work from. Speak plainly. Ask one
question at a time. Never mention placeholders or code unless the user asks.

## 1. Say what this is

Tell the user, in your own words, briefly:

- *"I'll ask about 15 short questions about your work, your clients, your
  week and how you write. It takes about 20 minutes. Then I'll write it all
  into a few files in your folder that Claude reads every time you work here,
  so you never have to explain yourself again."*
- *"You can say 'skip' to any question, and stop any time. Say 'continue my
  Claude brain' later and I'll pick up where we left off."*
- **The privacy rule, always:** *"These files sit on your computer and Claude
  reads them while it works with you. Keep out anything you'd regret having in
  a file: client account numbers, health details, passwords, confidential deal
  terms. First names and a line of context are plenty. If you work under
  compliance rules, like financial services, healthcare or law, keep client
  details out entirely and check your firm's policy on AI tools first."*

## 2. Check the folder

The brain lives in a folder on their computer that Claude can reach in this
conversation (given in the Claude desktop app).

- **No folder:** ask the user to give Claude access to one in the Claude
  desktop app before going on. Suggest a new folder named **Claude** in
  their Documents folder, used every day. Then they start a new
  conversation with it and say "Set up my Claude brain" again.
- **A folder is available:** tell them which one and confirm it's the folder
  they'll work from day to day. If not, same as above.
- **It already has a `CLAUDE.md`:** ask whether to update what's there (use
  the update-claude-brain skill instead) or start fresh. Starting fresh: rename
  the old file to `CLAUDE-old-<date>.md` first. Never delete it.
- **It has `knowledge/interview-notes.md` but no `CLAUDE.md`:** the interview
  was started before. Resume it (see `references/interview.md`).

## 3. Offer a head start

Ask: *"Want a head start? Give me your website address, or paste your
LinkedIn About section or a bio, and I'll fill in what I can so I only ask
what's missing."*

- With a website address: read the public home, about and services pages
  only. Don't log in anywhere.
- Then show what you picked up in one short message (who they are, what they
  sell, who they serve) and ask: *"Anything wrong or missing?"* Save only what
  they confirm.
- If they skip it, go straight to the interview.

## 4. Run the interview

Create the `knowledge/` folder if it isn't there. Follow
`references/interview.md` exactly: fifteen questions, one at a time, saving
each answer to `knowledge/interview-notes.md` before asking the next.

If the user stops partway, confirm their answers so far are saved and tell
them to say "continue my Claude brain" when they're ready.

## 5. Write the brain

When the interview is done, write these from the notes, using
`references/templates.md`:

```
<their folder>/
├── CLAUDE.md
└── knowledge/
    ├── my-business.md
    ├── my-people.md
    ├── my-voice.md
    ├── my-week.md
    ├── my-tools.md
    └── interview-notes.md
```

Then show a short summary, five to eight bullets in plain words ("You help
manufacturers with 20 to 200 people find...", "Replies should be short and
skip the pleasantries"), and ask: *"Anything I got wrong?"* Fix what they
correct, in the files.

## 6. Make it load everywhere

Explain: *"Claude reads your brain whenever it works with this folder. To
point every conversation at it, add one line to your Claude settings."*

Give them this to copy, with their actual folder path filled in:

> My Claude brain is in my <folder path> folder. When a task is about my
> business, my clients, my week or anything written in my voice, read its
> CLAUDE.md and the knowledge files it points to first.

Tell them where it goes: the Claude app's Settings, then **Your Claude**, in
**Instructions for Claude**. Suggest they keep a copy of that line somewhere,
because that setting has been known to lose recent edits. Their brain is
safe either way: it lives in the files.

## 7. Finish

Tell them what they can say from now on:

- **"Update my brain"** or **"Remember that..."** to change or add something
- **"What do you know about me?"** to review it
- Give Claude their **Claude** folder in each conversation, and pick it for
  scheduled tasks, so every session starts out knowing them

And: *"Any of my other assistants you install will read this first, so their
setup will be shorter."*
