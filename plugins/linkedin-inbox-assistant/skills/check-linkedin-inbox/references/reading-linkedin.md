# Reading LinkedIn safely and accurately

Read this before touching the browser. Each rule here was learned from a real
run that went wrong.

## Navigate once

Opening `https://www.linkedin.com/messaging/` makes LinkedIn open the top
conversation by itself, and that marks it read. Every extra navigation to the
messaging page marks another one read. So load the page once per run, then move
inside the page (scroll, switch tabs, click rows). Note which conversation was
open when the page settled and report it.

## The list loads as you scroll, and skips rows you scroll past too fast

The conversation list only builds rows near what's on screen. Scroll past a
row too quickly and it never loads, so no reading method will see it.

- Scroll in steps smaller than the visible list, so each view overlaps the last.
- Each view must share at least one name with the previous one. If two views
  share no name, part of the list was skipped: scroll back and read the gap.
- Read from the top down. Everything new is at the top, because LinkedIn sorts
  by most recent. This assistant never needs to go deep.

## Don't trust an empty list until it has finished loading

LinkedIn shows "No messages yet" while the list is still loading. Wait. An
empty inbox is real only when the page has settled and still shows it.

## Who wrote last

The preview line under each name says who sent the last message:

| Preview starts with | Who wrote last |
|---|---|
| `You:` | the user |
| `<Their first name>:` | them |
| neither | unclear: never guess |

An InMail or sponsored badge can sit where the prefix would be. No prefix means
the row didn't say, not that they wrote last.

## Unread dots are unreliable

Loading the page marks the top conversation read, and every conversation you
open becomes read. Use "who wrote last" to decide who is waiting. Treat the
unread dot as a hint only.

## Time labels

- Today's messages show a clock time, such as `10:42 AM`.
- This week's show a day name, such as `Tue`.
- Older ones show a date, such as `Nov 3`.
- A label like `1w` covers 7 to 13 days. Report it as shown; don't turn it into
  a date.

## Click by name, never by position

Rows sit next to checkboxes and menus that can archive or delete a
conversation. Find the element you want by its visible name or label, confirm
it's the right one, then click it. Never click a spot estimated from a
screenshot.

If a click lands somewhere unexpected (a menu opens, a checkbox ticks, a
compose box appears), stop. Describe what appeared in the report. Don't click
again to undo it: a second blind click is how a stray checkbox becomes a
deleted conversation.

## Tabs yes, filters no

Focused and Other are different sets of conversations: read both, switching
with the tab menu in the page (find it by its label). Don't navigate to a tab's
web address, which counts as another navigation. Filters such as Unread are
subsets of what you already read: skip them.

## Sales Navigator has its own inbox

Replies to messages sent from Sales Navigator land at
`https://www.linkedin.com/sales/inbox`, not in the regular messaging page.
Read it only if the user uses Sales Navigator. Loading it also opens and marks
read its top conversation.

## Stop pages

Stop the run the moment any of these appears, do nothing on the page, and
report it:

- a sign-in page or "Sign in to view"
- "Join LinkedIn" or any page asking to log in
- "Let's do a quick security check", a puzzle, or a CAPTCHA
- anything saying "unusual activity"
- anything saying the account is restricted or limited

Never sign in, retry, reload repeatedly, or try another route. Those pages are
LinkedIn's early warning, and pushing through them is how an account gets
restricted.

## Stay on the job

Read the conversation list and the conversations you draft for. Nothing else:
no profiles, no feed, no notifications page, no search results, no links
inside messages.
