# LinkedIn Inbox Assistant

*Version 0.1.0 · November 2026 · from Jeff Chastain, Admentus*

Three times each weekday it checks your LinkedIn messages and tells you who
wrote. For each new message, it drafts a reply you can copy, edit and send
yourself. It never sends anything.

---

## ⚠️ Read this before you turn it on

This assistant reads your LinkedIn messages by working your browser for you.
LinkedIn's User Agreement prohibits bots and automated tools, and LinkedIn
does restrict accounts it catches using them. **Using this puts your account
at risk.** That's your call to make.

To keep the risk low, it only reads. It never sends, likes, connects or
accepts anything. It checks three times a weekday, not constantly. And it
stops the moment LinkedIn shows a sign-in or security page. It never tries to
get past one.

I run tools like this on my own account, and LinkedIn has signed me out twice
in one day. I signed back in, paused them for a few days, and turned them back
on. That's the realistic downside, and it's why this assistant stops instead
of pushing through.

**If LinkedIn is central to your income and you can't afford a restriction,
don't turn this on.**

Setup shows you this warning first and asks you to confirm you understand the
risk. The assistant won't read LinkedIn until you have.

---

## What you need

- A paid Claude plan (Pro or above)
- The Claude desktop app, for Mac or Windows
- Google Chrome with the **Claude in Chrome** extension. The assistant reads
  LinkedIn in your own Chrome, so it won't work without it.
- LinkedIn signed in, in that Chrome
- A computer that's on, with Chrome and Claude open, during your check times

## Set up Claude (once, if you're new to it)

1. Sign up for a paid Claude plan (Pro or above) at claude.ai.
2. Download the Claude desktop app from claude.ai/download, install it and
   sign in.
3. In Google Chrome, open the Chrome Web Store, search for **Claude**, and
   install the Claude in Chrome extension from Anthropic. Pin it and sign in
   with the same Claude account.
4. Make sure you're signed in to LinkedIn in that Chrome.
5. In the Claude app, open **Settings**, then **Capabilities**, and turn on
   **Claude in Chrome**.

## Install the assistant

1. In the Claude desktop app, start a new chat, click **+** in the message
   box, and choose **Add plugins**.
2. Click **Add** (top right), then **Add marketplace**, then **Add from a
   repository**. Enter **admentus/assistants**, leave **Sync automatically**
   on, and click **Sync**. (You only do this once. It adds all of my
   assistants.)
3. Click **Add** next to **LinkedIn inbox assistant**.
4. Start a new chat. If you have a Claude brain, click **+**, choose **Add
   folder** and pick your **Claude** folder. Then say: **Set up my LinkedIn
   inbox assistant.**

If I sent you a `.plugin` file instead, choose **Upload plugin** instead of
**Add marketplace** in step 2, and skip step 3.

Setup takes about ten minutes. It asks how you write and what you want from
LinkedIn conversations, helps you schedule the checks, and runs the first one
with you.

## What it tells you

```
LinkedIn: 2 new messages, 1 waiting on you

NEW
1. Dana · 10:42 AM
   What they said: asked whether you work with firms her size
   Suggested reply:
   > Hi Dana, yes, most of the firms I work with are in that range...
   Why: answers her question first, then offers a short call

WAITING ON YOU
- Mark · Tue · "Thanks, let's find a time next week"

Nothing was sent.
```

## Things to say

- **Check my LinkedIn inbox** for an extra check any time
- **Draft a LinkedIn reply to <name>** for one reply
- **Set up my LinkedIn inbox assistant** to change how replies sound

## What it never does

Send, like, react, connect, accept, follow, archive, delete, or mark anything
unread. Visit profiles. Click links inside messages. Sign in for you or ask for
your password.

## One thing it can't avoid

Reading a message marks it read in LinkedIn, and the sender can see that.
Setup shows you how to turn off read receipts so nobody sees "read" hours
before you answer.

## If it stops for a security check

Open LinkedIn yourself and sign in or finish the check. Pause the scheduled
check for a few days (**Scheduled** in the left sidebar). Turn it back on when
LinkedIn looks normal.
