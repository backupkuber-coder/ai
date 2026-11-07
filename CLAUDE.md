# CLAUDE.md

## Instagram agent skills

`.claude/skills/ig-*` are the 13 skills from
https://github.com/Jakeschincariol/instagram-agent-skill (MIT, vendored at
commit d03c56b; license in `.claude/skills/LICENSE-instagram-agent-skill`).

The skills read and write `~/.claude/instagram/` (voice.md, swipe.md, log.md).
Cloud sessions start with an empty home directory, so in this repo **use the
repo's `instagram/` folder instead** wherever a skill says `~/.claude/instagram/`:

- `instagram/voice.md` - the voice profile. Read it before writing anything.
- `instagram/swipe.md` - written by `/ig-viral`, read by `/ig-reel` and `/ig-plan`.
- `instagram/log.md` - appended by `/ig-reel` on "yes", read by `/ig-audit`.

The Python tools live next to each SKILL.md and need only python3
(e.g. `python3 .claude/skills/ig-reel/hookscore.py hooks.txt`).

`/ig-reel` overlaps with the account's own `script` skill. When the user says
`/ig-reel`, use ig-reel's workflow and tools, but keep the voice and the
accuracy and safety rules from `instagram/voice.md`.
