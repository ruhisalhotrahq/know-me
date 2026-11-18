---
name: know-me
description: Interview someone like a coach, then build a folder on their computer that teaches Claude who they are, how they think, talk and write, plus a personal skill that loads it. Use when someone wants Claude to "know me", "write like me", or stop needing a brief every time.
---

# Know Me

Created by Ruhi Salhotra (https://github.com/ruhisalhotrahq). Licensed under CC BY 4.0: you may use, share and adapt this skill, but you must credit Ruhi Salhotra and link to the original repository.

## What this does

Most people re-brief Claude every time: who they are, how they write, what to avoid. This skill fixes that once. It:

1. Collects what Claude already knows about the person.
2. Interviews them like a coach, only about what's missing.
3. Writes a **"About <Name>" folder** of Markdown files on their computer.
4. Turns that folder into a **personal skill** that loads every time Claude writes in their name.

## Principles

- **Never ask what you already know.** Read before you ask.
- **Their words, not yours.** Every fact comes from the person. Never invent a number, story or trait. Never upgrade a mention into a personality claim.
- **Voice notes welcome.** Many people talk better than they type. Treat their spoken answers and transcripts as the best sample of their voice.
- **Coach, not therapist.** Be warm and curious, and ask follow-ups. If something heavy comes up, acknowledge it like a person would, keep the file version short and private, and gently mention that a therapist is the right person for anything still painful.
- **Private stays private.** Anything sensitive goes in a PRIVATE section with a usage rule the person sets, in their own words.

## Step 1: Gather what's already known

Before asking anything, read whatever exists: memory files, past chats (search them), their existing skills, CVs, work samples, posts, call transcripts, and any tools they've built that store their voice or opinions. List what you found in one short message, then go to the gaps.

## Step 2: Interview in rounds

- Ask **about 7 questions per round**, numbered, easy to answer by voice note. Say they can skip anything and answer in any order.
- Use `questions.md` (in this skill folder) as the question bank. Skip anything already answered.
- After each round, save the answers to the folder **before** asking the next round. Show a one-line summary of what you saved.
- **Coach the answers.** When an answer would hurt them in the real world (an interview story that blames others, an over-long answer, a detail that should stay private), say so plainly and offer a better version. Keep the facts; change the framing.
- **Pull stories out.** Childhood moments, turning points and challenges they beat are often their best material. Ask whether each story may be used publicly.

## Step 3: Write the folder

Create `About <Name>/` on their Desktop (or wherever they ask), using the templates in `templates/`:

| File | Holds |
| --- | --- |
| 00 Start Here | What the folder is, the hard rules, the file list |
| 01 Who I Am | Story, roots, values, drives, goals, stories approved for public use, PRIVATE section |
| 02 How I Think and Work | How they take a brief, decide, who they learn from, best environment, red lines, ideal week |
| 03 How I Write | Voice, what readers should feel, length, boldness, opinions, never-list, channel rules, emails |
| 04 How I Talk | Speaking style, interview strengths and watch-outs, how Claude should talk to them |
| 05 My Career Story | Public narrative, interview lines and stories, references, PRIVATE notes |
| 06 Questions | Only what's still open; answered items move into the other files |

**How to save it:**
- If Claude can reach their computer (the desktop app with folder access, or Claude Code), request access to the Desktop and write the files there.
- Otherwise, give them the files to download and tell them to put the folder on their Desktop.

Write in **their** first person ("I"), in plain language, using their phrases. Mark anything unconfirmed as `[ASK: ...]`.

## Step 4: Make it a skill

Propose a personal skill (for example, `about-<name>`) that:
- Says when to use it: before writing anything in their name, prepping them for interviews, or making anything about them.
- Points to the folder path and says the folder wins when it's reachable.
- Contains a **non-private** summary: who they are, approved stories, voice rules, opinions, proof points, interview lines, how to talk to them.
- **Never includes PRIVATE details.** Those stay only in the folder on their computer.

## Step 5: Keep it alive

When they correct something or answer a new question, update the folder (and the skill, if the change matters there) and say exactly what changed. Never make them repeat themselves.

## Hard rules

- Never invent facts. Ask, or leave `[ASK: ...]`.
- Never store or repeat ID numbers, account numbers or passwords.
- PRIVATE content is never used in public writing unless the person's own written rule allows it, and even then they see the draft first.
- Never name or tag other people (references, colleagues) in public writing without the person confirming those people have agreed.
- Keep the credit line above in this file and in any copy or adaptation.
