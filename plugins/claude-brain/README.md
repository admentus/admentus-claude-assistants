# Claude Brain

*Version 0.2.0 · November 2026 · from Jeff Chastain, Admentus*

A 20-minute interview that teaches Claude your practice, your clients and your
voice. It writes what it learns into a few plain files in a Claude project on
your computer. Every chat you start in the project reads them, so you stop
explaining yourself, and every other assistant you install starts out knowing
you.

It's the same setup I run my own practice on: one short file Claude always
reads, and a set of knowledge files it reads when a task needs them.

## What you need

- A paid Claude plan (Pro or above)
- The Claude desktop app, for Mac or Windows (claude.ai/download)

## Install it

1. In the Claude desktop app, start a new chat, click **+** in the message
   box, and choose **Add plugins**.
2. Click **Add** (top right), then **Add marketplace**, then **Add from a
   repository**. Enter **admentus/admentus-claude-assistants**, leave **Sync
   automatically** on, and click **Sync**. (Skip this if you've added it
   before.)
3. Click **Add** next to **Claude Brain**.
4. Make a project: click **Projects** in the left sidebar, then **+**, then
   **Start from scratch**. Name it **My Work** (or your business name) and
   save its folder in Documents. Use more than one computer? Save it in
   OneDrive, Dropbox, iCloud Drive or Google Drive instead.
5. On the project's page, check that **Context** lists the folder. If it
   doesn't, click **Add** next to it and pick the folder.
6. Start a chat from the project's page and say: **Set up my Claude brain.**
7. At the end, paste the short paragraph it gives you into the project's
   **Instructions**.

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
My Work/
├── CLAUDE.md                the short version Claude always reads
├── project-instructions.md  the shorter version for the project's instructions
└── knowledge/
    ├── my-business.md       what you sell, who you serve, how clients find you
    ├── my-people.md         key clients and partners, first names only
    ├── my-voice.md          how you write, with your own samples
    ├── my-week.md           where your time goes
    ├── my-tools.md          email, calendar, CRM, files
    └── interview-notes.md   your answers as you gave them
```

They're plain text. Open them, read them, change them.

## Your phone and other computers

The project follows you to your phone, the website and your other computers.
The folder stays on the computer it's on. So:

- **On your phone or the website,** chats in the project know the basics from
  the project's instructions, but can't open your files.
- **On a second computer,** keep the folder in a synced drive. Open the
  project there, click **Add** next to **Context**, and pick the folder.

## Things to say

- **Update my brain** or **Remember that...** to change or add something
- **What do you know about me?** to review it
- **Continue my Claude brain** to finish an interview you stopped
- **Move my brain into a project** if you set it up before it used projects

Start every chat from your project. A chat outside it doesn't know you.

## Keep it clean

These files sit on your computer, and Claude reads them while it works with
you. Leave out client account numbers, health details, passwords and
confidential deal terms. First names and a line of context are plenty. The
project's instructions are stored in your Claude account, so they hold only
the basics and no client names. If you work under compliance rules (financial
services, healthcare, law), keep client details out entirely and check your
firm's policy on AI tools first.
