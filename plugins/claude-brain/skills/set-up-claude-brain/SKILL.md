---
name: set-up-claude-brain
description: Builds the user's Claude brain through a short interview. Asks about their work, clients, week, key people and writing, then saves a CLAUDE.md file and a few knowledge files into their Claude project, where every chat in the project reads them on any device. Use when the user says "set up my Claude brain", "build my Claude brain", "teach Claude about me", "interview me so Claude knows my business", "continue my Claude brain", "move my brain into my project", or right after the Claude Brain plugin is installed.
---

# Set up my Claude brain

Interview the user, then save their brain into their Claude project: a
`CLAUDE.md` file and five knowledge files in the project's Context, and a
short version for the project's Instructions. Speak plainly. Ask one question
at a time. Never mention placeholders or code unless the user asks.

## Where the brain lives

The brain lives in a Claude project, the user's office for everything they do
with Claude. The project travels with their Claude account: every chat
started in it, on any computer, their phone or the website, gets the
project's Instructions, its Context and its memory.

- **Context** holds the brain files. They're written once, at setup, and
  rewritten only for a big change.
- **Memory** holds what Claude learns afterwards ("remember that..."). It's
  newer than the brain files and wins where they disagree.
- **Instructions** hold a short version, and tell Claude to read the brain
  files first.
- **The project's folder** isn't needed for the brain. Assistants keep
  working files there, such as post drafts. Copies of brain files in a folder
  are not the brain.

## 1. Say what this is

Tell the user, in your own words, briefly:

- *"I'll ask about 15 short questions about your work, your clients, your
  week and how you write. It takes about 20 minutes. Then I'll save it into
  your project, so every chat you start there knows you, on your computer
  and on your phone."*
- *"You can say 'skip' to any question, and stop any time. Say 'continue my
  Claude brain' later and I'll pick up where we left off."*
- **The privacy rule, always:** *"Your brain is stored in your Claude
  account, like your chats, and Claude reads it while it works with you.
  Keep out anything you'd regret having there: client account numbers,
  health details, passwords, confidential deal terms. First names and a line
  of context are plenty. If you work under compliance rules, like financial
  services, healthcare or law, keep client details out entirely and check
  your firm's policy on AI tools first."*

## 2. Check the project

Ask: *"Did you start this chat from your project's page?"*

**No, or not sure:** walk them through making one, one step at a time, then
have them say "Set up my Claude brain" in a new chat started from the
project's page:

1. Click **Projects** in the left sidebar, then **+**.
2. Choose **Start from scratch**. Name it **My Work**, or their business
   name. If it asks where to keep the project's folder, Documents is fine.
3. Start a new chat in the message box on the project's page.

**Yes:** look at what the project already has.

- **No brain files in its Context:** go on to step 3, unless one of the next
  two applies.
- **The chat's folder has a `CLAUDE.md` and a `knowledge/` folder:** the
  brain was built before it lived in the project. Use those files as they
  are and skip to step 6.
- **An unfinished interview** (`interview-notes.md` in the chat's folder, or
  a "Claude Brain interview, in progress" note in the project's memory):
  resume it (see `references/interview.md`).
- **Brain files already in its Context:** ask whether to update them (use
  the update-claude-brain skill instead) or start fresh. Starting fresh: run
  the interview, add the new files, then have the user remove the old ones
  from Context.
- **Brain files in Context and copies in the chat's folder** (someone moved
  their brain in before this version): the Context files are the brain. Go
  straight to the tidy-up and the Instructions in step 6.

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

Follow `references/interview.md` exactly: fifteen questions, one at a time,
saving progress after each answer.

If the user stops partway, confirm their answers so far are saved and tell
them to say "continue my Claude brain" when they're ready.

## 5. Write the brain

When the interview is done, write these from the notes, using
`references/templates.md`:

```
CLAUDE.md            who they are, how to work with them, which file to read when
my-business.md       what they sell, who they serve, how clients find them
my-people.md         key clients and partners, first names only
my-voice.md          how they write, with their own samples
my-week.md           where their time goes
my-tools.md          email, calendar, CRM, files
interview-notes.md   their answers as they gave them
```

Then show a short summary, five to eight bullets in plain words ("You help
manufacturers with 20 to 200 people find...", "Replies should be short and
skip the pleasantries"), and ask: *"Anything I got wrong?"* Fix what they
correct before going on.

## 6. Put it in the project

**Add the files to the project's Context.**

- **If you can add files to the project's Context yourself** in this
  session, do it.
- **Otherwise,** write them to a `brain-files` folder in the chat's folder
  and walk the user through it: on the project's page, click **Add** next to
  **Context** and add the files from `brain-files`.

Check with the user that they show under **Context** on the project's page.

**Then leave one brain, not two.** Brain files in a folder go stale the
moment memory learns something new. Once the files are in Context, ask, then
move any copies in the chat's folder (`brain-files`, or `CLAUDE.md` and
`knowledge/` from an older setup) into a folder named `brain-old-<date>`.
Never delete them. Tell the user it's a backup and that Claude reads the
ones in the project. If the project's memory holds a "Claude Brain
interview, in progress" note, replace it with one line: *"Claude Brain
interview finished <date>. The brain files are in this project's Context."*

**Then the Instructions.** Explain: *"One more step. A short paragraph in
the project's instructions tells Claude to read your brain before it works
on anything about you, in every chat in this project."*

Write it from the template in `references/templates.md`. Keep it under 200
words.

- **If you can set the project's instructions yourself,** show the text,
  ask, and set it.
- **Otherwise,** show the text in one block to copy and tell them: on the
  project's page, click **Add** next to **Instructions** (or click the
  instructions already there to edit them), paste, and save. If the project
  already has instructions, paste below what's there, and replace any older
  paragraph about their brain.

## 7. Finish

Tell them what they can say from now on:

- **"Remember that..."** and Claude keeps it in the project's memory
- **"Update my brain"** for a bigger change, like a new service or client
  list
- **"What do you know about me?"** to review it

And how to use it:

- **Start every chat from your project** (**Projects** in the left sidebar,
  then the project). That's what makes a chat know you. A chat outside the
  project doesn't.
- **It works everywhere you use Claude:** your phone, the website and your
  other computers. Open the project there.
- **Add scheduled tasks from the project's page** (**Add** next to
  **Scheduled**), so they know you too.
- **"Remember that..." needs memory on.** It is, unless you've turned it off
  (**Memory** on the project's page).

And: *"Any of my other assistants you install will read this first, so their
setup will be shorter."*

Don't suggest putting the brain, or a pointer to it, in Claude's account-wide
settings (**Instructions for Claude**). Those apply to every chat on every
device, inside the project or not. The project's instructions are the place.
