# Lesson 1 Homework — Profile Generator Script

**Estimated time:** 60–90 minutes
**File to edit:** `profile_builder.py`

## Your mission

Turn three simple questions into a stylish terminal "profile badge" — a
framed little card, printed entirely out of text, that shows off who you are.

## Step 1 — Collect three answers

Replace TODOs 1–3 in `profile_builder.py` with three `input()` calls, the
same way we practiced in the lesson. Give each question a friendly prompt.

Test after finishing this step alone, before touching the badge:

```
python profile_builder.py
```

If it asks three sensible questions and just prints plain answers back (no
badge yet), you're exactly on schedule — don't worry about the fancy part yet.

## Step 2 — Build the profile badge

Use f-strings (one or several `print()` calls) to turn `name`, `language`,
and `hobby` into a framed badge. A few ways to get there — pick whichever
feels most comfortable:

- **Simplest:** hard-code a border out of repeated characters, e.g. `"=" * 32`.
- **Neater:** paste box-drawing characters straight into your string —
  `║  ═  ╔  ╗  ╚  ╝  ╠  ╣` — and lay the rows out by hand.
- **Extra polish:** use an f-string alignment spec like `f"{name:<18}"` to
  left-pad a value to a fixed width, so every row lines up perfectly no
  matter how long the answer is.

Target output:

```
╔══════════════════════════════╗
║        PROFILE BADGE         ║
╠══════════════════════════════╣
║ Name:      Levani             ║
║ Language:  Python             ║
║ Hobby:     Chess              ║
╚══════════════════════════════╝
```

Get the three values printing correctly first, then spend your remaining
time making it pretty — that order saves the most frustration.

## Self-check checklist

- [ ] Running `python profile_builder.py` asks 3 questions.
- [ ] Output displays a neatly framed profile badge in the terminal.

## Frustration circuit-breaker

Seeing a **File Not Found** error when you try to run the script? Almost
always one of these three things:

1. You're not `cd`'d into the folder that actually contains
   `profile_builder.py` — run `pwd` then `ls` (or `dir` on Windows) to check.
2. The filename is spelled slightly differently than you typed (check
   underscores vs. dashes, and capitalisation).
3. You typed `python` when your machine needs `python3` (or vice versa).

Stuck for more than five minutes? Stop, don't spiral — watch the 1-minute
video clip provided, or send a screenshot of the exact error in chat.
