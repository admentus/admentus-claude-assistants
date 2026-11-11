---
name: set-up-linkedin-inbox
description: Sets up the LinkedIn inbox assistant. Explains the risk to the user's LinkedIn account, learns how the user writes and what they want from LinkedIn conversations, schedules the checks, and runs the first check together. Use when the user says "set up my LinkedIn inbox assistant", "set up the LinkedIn inbox", "configure the LinkedIn assistant", "change how my LinkedIn replies sound", or right after the plugin is installed.
---

# Set up the LinkedIn inbox assistant

Walk the user through setup one step at a time, in plain language. Ask one
question at a time and wait for the answer. Never mention files, folders,
placeholders or code unless the user asks.

## 1. The warning comes first, and the user acknowledges it

Show this exactly. Then ask: *"If you want to go ahead, reply with: I
understand the risk."*

- Continue only when the user replies with those words or plainly says the
  same thing in their own words ("I understand the risk and want to use it").
- A bare "ok", "sure" or "go ahead" is not enough. Say once that you need them
  to confirm they understand the risk to their account, and ask again.
- If they say no or decline, stop and tell them nothing was changed.
- When they acknowledge, note today's date. It's saved in step 4, and the
  inbox check won't run without it.

> **Read this before you turn it on.**
>
> This assistant reads your LinkedIn messages by working your browser for you.
> LinkedIn's User Agreement prohibits bots and automated tools, and LinkedIn
> does restrict accounts it catches using them. Using this puts your account at
> risk. That's your call to make.
>
> To keep the risk low, it only reads. It never sends, likes, connects or
> accepts anything. It checks three times a weekday, not constantly. And it
> stops the moment LinkedIn shows a sign-in or security page. It never tries to
> get past one.
>
> I run tools like this on my own account, and LinkedIn has signed me out
> twice in one day. I signed back in, paused them for a few days, and turned
> them back on. That's the realistic downside, and it's why this assistant
> stops instead of pushing through.
>
> If LinkedIn is central to your income and you can't afford a restriction,
> don't turn this on.
>
> — Jeff Chastain

## 2. Connect Claude in Chrome

This assistant reads LinkedIn in the user's own Google Chrome, through the
Claude in Chrome extension. It doesn't use any other browser. Ask the user to
confirm three things, one at a time, and walk them through any that aren't
done:

1. **Claude in Chrome is installed and signed in.** If not: in Google Chrome,
   open the Chrome Web Store, search for "Claude", install the extension from
   Anthropic, pin it to the toolbar, and sign in with the same Claude account
   they use in the app.
2. **They're signed in to LinkedIn in that Chrome.** They sign in themselves.
   Never ask for their password and never type it.
3. **Claude is allowed to use it.** In the Claude app, Settings, then
   Capabilities: Claude in Chrome is turned on.

Then open https://www.linkedin.com/messaging/ once through Claude in Chrome to
confirm it works. If it shows a sign-in or security page, stop and ask them to
sign in themselves. Don't move on until the inbox loads.

## 3. Learn about them

**If the user has a Claude brain** (a `CLAUDE.md` and a `knowledge/` folder in
the working folder), read `CLAUDE.md`, `knowledge/my-business.md`,
`knowledge/my-people.md` and `knowledge/my-voice.md` first. Fill in every
answer below that they already cover, show the user what you took in one short
message, and ask only the questions left. In step 4, copy what you used into
this assistant's own file too, because a scheduled check may not be able to
read the folder.

Ask these one at a time. Offer the example when it helps. Accept "skip" for
anything optional.

1. "What's your name, as it shows on LinkedIn?"
2. "In one sentence, what do you do?"
3. "Who do you work with?" (for example: owners of companies with 10 to 100
   people)
4. "When a LinkedIn conversation is going well, what's the next step you want?"
   (for example: a 20-minute call, an introduction, or just staying in touch)
5. "Do you have a booking link you'd like offered when someone wants to talk?"
   (optional)
6. "Do you use Sales Navigator?"
7. "Is there anyone whose messages should always be flagged first, like
   clients or close partners?" (optional)
8. "Paste three or four messages you've sent, on LinkedIn or by email, that
   sound like you. Short ones are fine." Explain that this is what makes the
   suggested replies sound like them.
9. "Is there anything a reply should never say or do?" (for example: never
   mention pricing, never sound salesy)
10. "I'll check three times each weekday: 8 AM, noon and 4 PM. Want different
    times?"

## 4. Save what they said

Find this plugin's folder:

```
find mnt/.local-plugins mnt/.plugins -type d -name "*linkedin-inbox-assistant*"
```

In it, open `skills/check-linkedin-inbox/references/about-me.md` and replace
each line starting with `~~` with the user's answer (use "none" for anything
skipped; use the default times if they kept them). For "Risk acknowledged",
write the date from step 1 and the words they used. Keep the headings as they
are.

If the folder can't be found or the file can't be changed, write the same
content to `linkedin-assistant-about-me.md` in the working folder instead, and
tell the user where it is.

Show the user a short summary of what you saved and ask if anything needs
changing.

## 5. Recommend turning off read receipts

Explain: *"When I read a new message to draft your reply, LinkedIn marks it
read, and the sender can see that. To avoid someone seeing 'read' hours before
you answer, turn off read receipts in LinkedIn: Settings & Privacy, then Data
privacy, then Messaging experience, then Read receipts and typing
indicators."* The user changes this setting themselves. Don't do it for them.

## 6. Schedule the checks

Tell the user how to set the schedule:

1. Open **Scheduled** in the Claude app's left sidebar and add a task. If
   it asks which folder to work in, pick their **Claude** folder so the
   check can read their brain.
2. Name it **LinkedIn inbox check**.
3. For what to do, enter: **Check my LinkedIn inbox**.
4. Set it for weekdays at the times they chose.

Then explain: *"Because this uses your Chrome, your computer needs to be on,
with Chrome and the Claude app open, at those times. If it's asleep, that
check is skipped."*

If you're able to create the scheduled task yourself in this session, offer
to do it, confirm the name, prompt and times with the user, and then create
it.

## 7. Run the first check together

Run the check-linkedin-inbox skill now. Show the report. Ask: *"Do these
replies sound like you?"* If not, ask what's off, update the samples or the
"never" list in the saved file, and offer to run it again.

Finish by telling them:

- Say **"check my LinkedIn inbox"** any time for an extra check.
- Say **"draft a LinkedIn reply to <name>"** for one reply.
- If it ever reports a security check, sign in to LinkedIn yourself and pause
  the schedule for a few days.
