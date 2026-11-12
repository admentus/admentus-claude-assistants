# Template: linkedin-inbox-settings.md

Setup writes this file from the user's answers and adds it to their project's
Context. The inbox check reads it on every run. Nothing is ever saved inside
the plugin itself: a plugin update replaces its files.

Rules:

- Replace everything in `<angle brackets>`. Write "none" for anything skipped.
- **Risk acknowledged** carries the date and the user's own words, exactly. It
  is the consent record: the check won't open LinkedIn without it.
- **With a Claude brain, leave out the last section.** The brain already has
  the user's name, work and writing, and it's what they keep up to date.
- No client account numbers, passwords, health details or confidential deal
  terms. The file is stored in the user's Claude account.

```markdown
# LinkedIn inbox assistant settings

The LinkedIn inbox assistant reads this on every run. Say "set up my LinkedIn
inbox assistant" to change it.

- **Risk acknowledged:** <date>, "<the words they used>"
- **Check times:** <weekdays at 8 AM, 12 PM and 4 PM, or their times>
- **A good next step in a LinkedIn conversation:** <answer>
- **My booking link (offer it only when they want to talk):** <link or none>
- **I use Sales Navigator:** <yes or no>
- **People to always flag first:** <first names, or none>

## LinkedIn replies never

<what a suggested reply must never say or do, or none>

## About me (only without a Claude brain)

- **Name, as it shows on LinkedIn:** <answer>
- **What I do, in one sentence:** <answer>
- **Who I work with:** <answer>

### How I write

Messages I've actually sent, so suggested replies sound like me:

<three or four messages, exactly as written>
```
