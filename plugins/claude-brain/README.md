# Claude Brain

*Version 0.1.0 · November 2026 · from Jeff Chastain, Admentus*

A 20-minute interview that teaches Claude your practice, your clients and your
voice. It writes what it learns into a few plain files in a folder on your
computer. Claude reads them every time you work there, so you stop explaining
yourself, and every other assistant you install starts out knowing you.

It's the same setup I run my own practice on: one short file Claude always
reads, and a set of knowledge files it reads when a task needs them.

## What you need

- A paid Claude plan (Pro or above)
- The Claude desktop app, for Mac or Windows (claude.ai/download)

## Install it

1. In the Claude desktop app, start a new chat, click **+** in the message
   box, and choose **Add plugins**.
2. Click **Add** (top right), then **Add marketplace**, then **Add from a
   repository**. Enter **admentus/assistants**, leave **Sync automatically**
   on, and click **Sync**. (Skip this if you've added it before.)
3. Click **Add** next to **Claude brain**.
4. Start a new chat, click **+** in the message box, choose **Add folder**,
   and pick a folder called **Claude** in your Documents (create it if it
   isn't there).
5. In that chat, say: **Set up my Claude brain.**

## What it asks

About fifteen questions, one at a time: what you do and for whom, what you
sell, your best clients, how they find you, where your week goes, the people
Claude should know, a few things you've written, and how you want Claude to
work with you. Say "skip" to anything. Stop any time and say "continue my
Claude brain" later.

Give it your website address first and it fills in what it can, so it only
asks what's missing.

## What it writes

```
Claude/
├── CLAUDE.md              the short version Claude always reads
└── knowledge/
    ├── my-business.md     what you sell, who you serve, how clients find you
    ├── my-people.md       key clients and partners, first names only
    ├── my-voice.md        how you write, with your own samples
    ├── my-week.md         where your time goes
    ├── my-tools.md        email, calendar, CRM, files
    └── interview-notes.md your answers as you gave them
```

They're plain text. Open them, read them, change them.

## Things to say

- **Update my brain** or **Remember that...** to change or add something
- **What do you know about me?** to review it
- **Continue my Claude brain** to finish an interview you stopped

## Keep it clean

These files sit on your computer, and Claude reads them while it works with
you. Leave out client account numbers, health details, passwords and
confidential deal terms. First names and a line of context are plenty. If you
work under compliance rules (financial services, healthcare, law), keep
client details out entirely and check your firm's policy on AI tools first.
