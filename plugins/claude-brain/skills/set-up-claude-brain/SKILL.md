---
name: set-up-claude-brain
description: Builds the user's Claude brain through a short interview. Asks about their work, clients, week, key people and writing, then writes a CLAUDE.md file and a knowledge folder in their Claude project, plus short project instructions that work on every device. Use when the user says "set up my Claude brain", "build my Claude brain", "teach Claude about me", "interview me so Claude knows my business", "continue my Claude brain", "move my brain into a project", or right after the Claude Brain plugin is installed.
---

# Set up my Claude brain

Interview the user, then write their brain: a `CLAUDE.md` file and a
`knowledge/` folder in their Claude project's folder, and a short version of
it for the project's instructions. Speak plainly. Ask one question at a time.
Never mention placeholders or code unless the user asks.

## 1. Say what this is

Tell the user, in your own words, briefly:

- *"I'll ask about 15 short questions about your work, your clients, your
  week and how you write. It takes about 20 minutes. Then I'll write it into
  a few files in your project's folder, and give you a short paragraph for
  the project's instructions. Every chat you start in the project will know
  you, so you never have to explain yourself again."*
- *"You can say 'skip' to any question, and stop any time. Say 'continue my
  Claude brain' later and I'll pick up where we left off."*
- **The privacy rule, always:** *"These files sit on your computer and Claude
  reads them while it works with you. Keep out anything you'd regret having in
  a file: client account numbers, health details, passwords, confidential deal
  terms. First names and a line of context are plenty. If you work under
  compliance rules, like financial services, healthcare or law, keep client
  details out entirely and check your firm's policy on AI tools first."*

## 2. Check the project and its folder

The brain lives in a Claude project: the user's office for everything they do
with Claude. Every chat started in the project opens with the project's
folder, its instructions and its memory. The folder holds the brain's files.

Ask: *"Did you start this chat from your project's page?"* Check that this
chat has a folder you can write to.

- **Yes, and there's a folder:** tell them which folder and go on.
- **No project yet, or no folder in this chat:** walk them through it one
  step at a time, then have them say "Set up my Claude brain" in a new chat
  started from the project's page:
  1. Click **Projects** in the left sidebar, then **+**.
  2. Choose **Start from scratch**. If they already keep a folder for Claude,
     choose **Use an existing folder** and pick it.
  3. Name it **My Work**, or their business name. Save its folder in
     Documents. If they use more than one computer, save it in OneDrive,
     Dropbox, iCloud Drive or Google Drive instead.
  4. On the project's page, look at **Context**. If it doesn't list the
     folder, click **Add** next to it and pick the folder.
  5. Start a new chat in the message box on the project's page.
- **The folder has a `CLAUDE.md` but no `project-instructions.md`:** the
  brain was built before it lived in a project. Confirm the project and
  folder as above, then skip to step 6.
- **It has both:** ask whether to update what's there (use the
  update-claude-brain skill instead) or start fresh. Starting fresh: rename
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
<their project's folder>/
├── CLAUDE.md
├── project-instructions.md
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

## 6. Put the short version in the project's instructions

Explain: *"Your project follows you to your phone and your other computers.
Your folder doesn't. So here's a short version of your brain for the
project's instructions. In this project, Claude will know the basics wherever
you open it, and read the full detail from your folder when it's there."*

Write `project-instructions.md` from its template in `references/templates.md`
(or from `CLAUDE.md`, when you skipped here from step 2). Keep it under 200
words. Keep client names and anything private out of it: project
instructions are stored in the user's Claude account, not only on their
computer.

Then put it in the project:

- **If you can set the project's instructions yourself** in this session,
  show the text, ask, and set it.
- **Otherwise,** show the text in one block to copy and tell them: on the
  project's page, click **Add** next to **Instructions** (or click the
  instructions already there to edit them), paste, and save. If the project
  already has instructions, paste below what's there. A copy stays in their
  folder as `project-instructions.md`.

## 7. Finish

Tell them what they can say from now on:

- **"Update my brain"** or **"Remember that..."** to change or add something
- **"What do you know about me?"** to review it

And how to use it:

- **Start every chat from your project** (**Projects** in the left sidebar,
  then the project). That's what makes a chat know you. A chat outside the
  project doesn't.
- **Add scheduled tasks from the project's page** (**Add** next to
  **Scheduled**), so they run with the folder and instructions too.
- **On your phone or the website,** chats in the project know the basics
  from the instructions but can't open your files.
- **On a second computer,** with the folder in a synced drive: the project
  shows up there on its own, but the folder has to be added on each
  computer. Open the project, click **Add** next to **Context** and pick the
  folder.

And: *"Any of my other assistants you install will read this first, so their
setup will be shorter."*

Don't suggest putting the brain, or a pointer to it, in Claude's account-wide
settings (**Instructions for Claude**). Those apply to every chat on every
device, inside the project or not. The project's instructions are the place.
