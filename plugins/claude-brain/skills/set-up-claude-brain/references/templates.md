# Templates for the brain files

Write each file from the interview notes. Rules for all of them:

- **Use their words.** Tighten, don't embellish. Never add a claim, a number
  or a client they didn't give you.
- **"Not answered" beats a guess.** Leave the line in so they can fill it
  later.
- **CLAUDE.md stays short:** about one page, under 60 lines. Detail goes in
  the knowledge files.
- **No confidential details anywhere:** no account numbers, passwords, health
  information or confidential deal terms. These files are stored in the
  user's Claude account. If an answer contained one, leave it out and tell
  the user you did.
- Replace everything in `<angle brackets>`. Delete any section that would be
  empty except for "not answered" in a knowledge file; keep it in CLAUDE.md.

---

## CLAUDE.md

```markdown
# About me: read this first

This is my Claude brain. It tells you who I am and how to work with me. The
other brain files in this project hold the detail: read the ones a task
needs. This project's memory holds what I've told you since; where it
disagrees with these files, memory is newer and wins.

## Who I am

<Name>, <role> at <firm>. <One or two sentences: what I do and who for.>

## What I'm focused on

<One to three lines from question 8.>

## How to work with me

- <Answer length and detail, from question 15>
- <Ask first, or take a first pass>
- <Anything else they said about working together>

## How I write

<Three to five short rules drawn from their samples and question 13, such as
"short sentences", "no exclamation points", "signs off with just my first
name".> Read `my-voice.md` before writing anything I'll send or post.

## Always and never

- Always: <from question 15, or "check with me before sending anything">
- Never: <from questions 13 and 15>
- Never put client account numbers, health information, passwords or
  confidential deal terms in these files, in memory, or in anything you
  draft.

## Where the detail is

| File | Read it when |
|---|---|
| `my-business.md` | the task touches what I sell, who I serve, or how clients find me |
| `my-people.md` | a client, partner or contact is named |
| `my-voice.md` | you're writing anything in my voice |
| `my-week.md` | planning, priorities, or where my time goes |
| `my-tools.md` | the task involves my email, calendar, contacts or files |

*Built <date> by the Claude Brain interview. Say "update my brain" to change
anything.*
```

---

## Project instructions

The short version that goes in the project's Instructions. It says the same
things as `CLAUDE.md`, shorter, and points Claude at the rest. Under 200
words. No people or clients here: they belong in `my-people.md`.

```markdown
I'm <name>, <role> at <firm>. <One sentence: what I do and who for.>

Right now I'm focused on <one line from question 8>.

How to work with me:
- <two or three lines from "How to work with me" in CLAUDE.md>

How I write:
- <three short rules from "How I write" in CLAUDE.md>
- Never: <the never lines about writing>

My Claude brain is in this project's Context: CLAUDE.md plus my business,
people, voice, week and tools files. Read CLAUDE.md before any work about my
business, my clients, my week or anything written in my voice, then the files
it points to. This project's memory holds what I've told you since; where it
disagrees with those files, memory is newer and wins.
```

---

## my-business.md

```markdown
# My business

## What I do
<From question 2, in their words.>

## What I sell
<From question 3: each service or offer as a short bullet, and how a typical
engagement works.>

## My best clients
<From question 4.>

## Not a fit
<From question 5.>

## How clients find me
<From question 6.>

## Why clients pick me
<From question 7.>

## This year
<From question 8.>
```

---

## my-people.md

```markdown
# My people

First names and context only. Nothing confidential.

| Name | Who they are | Context |
|---|---|---|
| <first name> | <client / partner / referral source / colleague> | <their one line> |
```

---

## my-voice.md

```markdown
# My voice

## How I sound
<Three to six observations from the samples: sentence length, warmth,
directness, how they open and close, formatting habits.>

## Words and phrases I use
<From question 13 and the samples.>

## Never sound like this
<From question 13.>

## Samples, exactly as I wrote them

### Sample 1
<verbatim>

### Sample 2
<verbatim>
```

---

## my-week.md

```markdown
# My week

## Where my time goes
<From question 9.>

## Only I can do, and wish I didn't
<From question 10, in their words. This is often the best place to start
handing work to an assistant.>

## What I'm focused on
<From question 8.>
```

---

## my-tools.md

```markdown
# My tools

| For | I use |
|---|---|
| Email | <...> |
| Calendar | <...> |
| Contacts or CRM | <...> |
| Files | <...> |
| Accounting | <...> |
| LinkedIn | <Sales Navigator? yes or no, if they said> |
| Other | <...> |
```
