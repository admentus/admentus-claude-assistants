---
name: set-up-linkedin-inbox
description: Sets up the LinkedIn inbox assistant. Explains the risk to the user's LinkedIn account, learns what the user wants from LinkedIn conversations, saves the settings in their Claude project, schedules the checks, and runs the first check together. Use when the user says "set up my LinkedIn inbox assistant", "set up the LinkedIn inbox", "configure the LinkedIn assistant", "change how my LinkedIn replies sound", "move my LinkedIn settings into my project", or right after the plugin is installed.
---

# Set up the LinkedIn inbox assistant

Walk the user through setup one step at a time, in plain language. Ask one
question at a time and wait for the answer. Don't mention files, folders,
placeholders or code unless a step needs the user to click something.

If the user said "move my LinkedIn settings into my project", go to **Moving
older settings into the project** at the end instead.

## 1. The warning comes first, and the user acknowledges it

Show this exactly. Then ask: *"If you want to go ahead, reply with: I
understand the risk."*

- Continue only when the user replies with those words or plainly says the
  same thing in their own words ("I understand the risk and want to use it").
- A bare "ok", "sure" or "go ahead" is not enough. Say once that you need them
  to confirm they understand the risk to their account, and ask again.
- If they say no or decline, stop and tell them nothing was changed.
- When they acknowledge, note today's date and their words. Both are saved in
  step 5, and the inbox check won't run without them.

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

## 2. Check the project

The settings are saved in the user's Claude project, so the check finds them
on whichever computer runs it. Ask: *"Did you start this chat from your
Claude project's page?"*

- **Yes:** look at the project's Context.
  - **`linkedin-inbox-settings.md` is already there:** they're changing
    their settings. Read it, use its answers as the defaults below, and save
    over it in step 5.
  - **No settings in Context, but the chat's folder has
    `linkedin-assistant-about-me.md`:** an older setup. Use **Moving older
    settings into the project** instead.
- **No, or not sure:** ask them to start the chat from their project's page
  (**Projects** in the left sidebar, then the project) and say "Set up my
  LinkedIn inbox assistant" there. No project yet: **Projects**, then **+**,
  then **Start from scratch**, named **My Work**. If they'd rather not use a
  project, carry on and save the settings in the chat's folder in step 5. With
  no folder either, a project is the only place the settings can be kept.

## 3. Connect Claude in Chrome

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

## 4. Learn what they want

**If the user has a Claude brain** (`CLAUDE.md` and `my-*.md` files in the
project's Context, or, from an older setup, `CLAUDE.md` with a `knowledge/`
folder in the working folder), read `CLAUDE.md`, `my-business.md`,
`my-people.md` and `my-voice.md`, and check the project's memory. The brain
answers questions 1, 2, 3 and 8: skip them, show the user in one short message
what you took, and ask the rest. If the brain names clients or close
partners, offer them as the answer to question 7.

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
9. "Is there anything a LinkedIn reply should never say or do?" (for example:
   never mention pricing, never sound salesy)
10. "I'll check three times each weekday: 8 AM, noon and 4 PM. Want different
    times?"

## 5. Save the settings

Write `linkedin-inbox-settings.md` from `references/settings-template.md` in
this skill's folder. Put the date and words from step 1 in "Risk
acknowledged". With a Claude brain, leave out the "About me" section.

Then put it in the project's Context:

- **If you can add files to the project's Context yourself,** do it. If an
  older copy is already there, replace it if you can; if you can only add,
  add the new one and tell the user exactly which old file to remove from
  **Context** on the project's page.
- **Otherwise,** write it to the chat's folder and walk them through it: on
  the project's page, click **Add** next to **Context** and add
  `linkedin-inbox-settings.md`.
- **No project** (they chose to go without): leave it in the chat's folder.

Never save anything inside the plugin's own folder: an update replaces it.

Show the user a short summary of what you saved and ask if anything needs
changing.

## 6. Recommend turning off read receipts

Explain: *"When I read a new message to draft your reply, LinkedIn marks it
read, and the sender can see that. To avoid someone seeing 'read' hours before
you answer, turn off read receipts in LinkedIn: Settings & Privacy, then Data
privacy, then Messaging experience, then Read receipts and typing
indicators."* The user changes this setting themselves. Don't do it for them.

## 7. Schedule the checks

Tell the user how to set the schedule:

1. On their project's page (**Projects** in the left sidebar, then their
   project), click **Add** next to **Scheduled**. Without a project, open
   **Scheduled** in the left sidebar and add a task there, picking the folder
   that holds the settings file.
2. Name it **LinkedIn inbox check**.
3. For what to do, enter: **Check my LinkedIn inbox**.
4. Set it for weekdays at the times they chose.

Then explain: *"Because this uses your Chrome, your computer needs to be on,
with Chrome and the Claude app open, at those times. If it's asleep, that
check is skipped. If you use Claude on more than one computer, look at the
check's run history under Scheduled after a day: it should run on one
computer only, the one where Chrome is signed in to LinkedIn."*

If you're able to create the scheduled task yourself in this session, offer
to do it, confirm the name, prompt and times with the user, and then create
it.

## 8. Run the first check together

Run the check-linkedin-inbox skill now. Show the report. Ask: *"Do these
replies sound like you?"* If not, ask what's off:

- **How they write:** with a Claude brain, save it to the project's memory
  ("remember that..."); without one, update "How I write" in the settings.
- **Something a LinkedIn reply must never do:** add it to "LinkedIn replies
  never" in the settings.

Offer to run it again.

Finish by telling them:

- Say **"check my LinkedIn inbox"** any time for an extra check.
- Say **"draft a LinkedIn reply to"** and a name for one reply.
- If it ever reports a security check, sign in to LinkedIn yourself and pause
  the schedule for a few days.

## Moving older settings into the project

For "move my LinkedIn settings into my project", or a project chat whose
folder has `linkedin-assistant-about-me.md` while the project's Context has
no `linkedin-inbox-settings.md`:

1. Read the old file. If its "Risk acknowledged" line has no date and words,
   this isn't a move: run setup from step 1.
2. Write `linkedin-inbox-settings.md` from the template, carrying "Risk
   acknowledged" over exactly as recorded. With a Claude brain, leave out
   the "About me" section and tell the user their name, work and writing now
   come from the brain.
3. Show it, then add it to the project's Context as in step 5.
4. Once it's in Context, ask, then rename the old file to
   `linkedin-assistant-about-me-old-<date>.md`. Never delete it.
5. Tell them the check now finds its settings on any computer in the
   project.
