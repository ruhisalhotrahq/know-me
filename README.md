# Know Me

**Make Claude actually know you, once, so you never have to brief it again.**

Created by [Ruhi Salhotra](https://github.com/ruhisalhotrahq).

Most people re-explain themselves to Claude every time: who they are, how they write, what to avoid. Know Me fixes that. Claude interviews you like a coach, only asks what it doesn't already know, and builds an **"About You" folder** on your computer, plus a personal skill that loads it whenever Claude writes in your name.

I built this for myself while job hunting. It worked so well I'm sharing it.

## What you get

```
About <Your Name>/
├── 00 Start Here.md          what the folder is, the hard rules
├── 01 Who I Am.md            your story, values, goals, stories you can use publicly
├── 02 How I Think and Work.md how you decide, who you learn from, red lines
├── 03 How I Write.md         your voice, opinions, never-list, channel rules
├── 04 How I Talk.md          how you speak, and how Claude should talk to you
├── 05 My Career Story.md     public story, interview lines, references
└── 06 Questions.md           what's still open
```

Plus a personal skill (for example, `about-yourname`) that points Claude to the folder and carries a non-private summary.

## How to use it

**Option 1: as a skill (best).**
1. Download the `know-me` folder from this repo.
2. Add it as a skill in Claude (Settings → Capabilities → Skills → upload), or put it in `~/.claude/skills/know-me/` for Claude Code.
3. Say: **"Use the know-me skill. I want you to really know me."**
4. Answer the questions by voice note if you like. Talking works better than typing.

**Option 2: no skills? Use the single file.**
Upload [`KNOW-ME.md`](KNOW-ME.md) to a chat or a Claude Project and say: **"Follow this file. Interview me and build my folder."**

## How it works

1. **Gathers first:** reads your memory, past chats, existing skills and documents, so it doesn't ask what it already knows.
2. **Interviews in rounds** of about 7 questions: who you are, what drives you, how you think, how you write and talk, your career story ([full question bank](know-me/questions.md)).
3. **Coaches your answers:** if an interview story blames someone else or runs too long, it tells you and offers a better version.
4. **Writes the folder** on your Desktop, in your own words.
5. **Makes it a skill**, without your private details.
6. **Stays updated** whenever you correct something.

## Privacy

- Anything sensitive goes in a **PRIVATE** section, with a usage rule you write yourself (for example, "only when I'm writing about my own journey").
- Private details stay in the folder on your computer and never go into the skill.
- Claude never names your references in public writing until you say they've agreed.

## License and credit

© 2026 Ruhi Salhotra. Licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You're free to use, share and adapt this, including commercially, **as long as you credit me**: name Ruhi Salhotra, link to this repo, and say if you changed it. Please don't present it as your own work.

Suggested credit line:
> Based on "Know Me" by Ruhi Salhotra (https://github.com/ruhisalhotrahq/know-me), CC BY 4.0.
