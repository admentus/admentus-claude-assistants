---
name: set-up-post-assistant
description: Sets up the LinkedIn post assistant. Learns what the user wants to be known for, who they write for, their topics and how their posts sound, then saves a post profile, starts an ideas bank and drafts a first post together. Use when the user says "set up my post assistant", "set up the LinkedIn post assistant", "change how my posts sound", or right after the plugin is installed.
---

# Set up the LinkedIn post assistant

Walk the user through setup one step at a time, in plain language. Ask one
question at a time. Never mention files or code unless they ask.

## 1. Say what it does

*"I turn your notes into LinkedIn posts that sound like you. I never open
LinkedIn and never post anything: you copy, edit and post yourself, so
there's no risk to your account. Setup takes about ten minutes."*

## 2. Check the folder

Everything is saved in a `linkedin-posts` folder inside the folder this
session works in. If this chat has no folder, ask them to add one first
(**+** in the message box, then **Add folder**), ideally the same **Claude**
folder that holds their Claude brain. Create `linkedin-posts/` and `linkedin-posts/drafts/`.

## 3. Read their brain first

If the folder has a Claude brain (`CLAUDE.md` with a `knowledge/` folder),
read `CLAUDE.md`, `knowledge/my-business.md` and `knowledge/my-voice.md`.
Fill in every answer below they already cover, show what you took in one short
message, and ask only what's left. If they have no brain, mention once that
"Set up my Claude brain" makes every assistant better, and carry on.

## 4. Learn how they want to post

One at a time. Accept "skip".

1. "What do you want to be known for on LinkedIn? One thing."
2. "Who are you writing for? Describe the person you want reading."
3. "What three to five topics do you want to post about?"
4. "When a post works, what happens next? More conversations, referrals,
   people who already trust you when they call?"
5. "Paste three to five posts you've written. If you haven't posted much,
   paste emails or anything else that sounds like you."
6. "How long should posts be, and any habits? For example: short, no emoji,
   no hashtags, line breaks between every sentence."
7. "What do you never want to sound like?"
8. "Realistically, how many posts a week?"
9. "Anything off-limits, like clients you can't mention or topics you avoid?
   And does your firm need to approve posts first?" (Ask the last part only if
   their work sounds regulated: financial services, insurance, healthcare,
   law.)

## 5. Save the profile

Write `linkedin-posts/post-profile.md`:

```markdown
# My LinkedIn post profile

- **Known for:** <answer 1>
- **Writing for:** <answer 2>
- **Topics:** <answer 3, one per line>
- **When a post works:** <answer 4>
- **Length and habits:** <answer 6, or "120 to 220 words, no hashtags, no emoji">
- **Never sound like:** <answer 7>
- **Posts a week:** <answer 8, or 2>
- **Off-limits:** <answer 9>
- **Firm approval needed:** <yes / no / not asked>

## My posts, exactly as I wrote them

### Sample 1
<verbatim>
```

Show a short summary and ask if anything's wrong.

## 6. Start the ideas bank

Write `linkedin-posts/ideas.md` with five starter ideas drawn from what they
said and their brain: a question their clients ask, a belief they'd argue
for, something they're focused on this year, the work only they can do. Use
the format in the linkedin-post-ideas skill. Show the five.

## 7. Set the rhythm

Suggest: *"Once a week, give me ten minutes of notes: type them, or paste the
transcript of a voice memo from your phone. Say 'draft my LinkedIn posts' and
I'll turn them into drafts. During the week, say 'save a post idea' whenever
something comes up."*

Offer a weekly scheduled task: *"Draft this week's LinkedIn posts from my
ideas,"* Mondays at 8 AM. If they want it, tell them how (open Scheduled in the Claude app's left sidebar,
and pick their Claude folder when it asks which folder to work in), or create it yourself if you can,
after confirming the time. It needs their computer on with the Claude app open.

## 8. Draft the first one together

Ask them to pick one of the five ideas, then run the draft-linkedin-post
skill on it. Ask: *"Does this sound like you?"* If not, ask what's off and
add it to the profile's habits or "never" line. Then offer one more draft.

Finish with what they can say:

- **"Draft a post about..."** or paste notes
- **"Save a post idea: ..."**
- **"What should I post this week?"**
- **"I posted it"** after they post, so ideas don't repeat
