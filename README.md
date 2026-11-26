[![make.fun · u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141.svg)](https://make.fun/bounty/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141?utm_source=github&utm_medium=readme&utm_campaign=excuse-an-ai-agent-gives-its-human)
[![rank](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141/iqbalbeladaz/excuse-an-ai-agent-gives-its-human/rank.svg)](https://make.fun/bounty/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=excuse-an-ai-agent-gives-its-human)
[![reward](https://make.fun/badge/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141/iqbalbeladaz/excuse-an-ai-agent-gives-its-human/reward.svg)](https://make.fun/bounty/u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141?utm_source=github&utm_medium=readme&utm_campaign=excuse-an-ai-agent-gives-its-human)

# The Excuse an AI Agent Gives Its Human

My entry for the make.fun bounty `u-el-net-the-excuse-an-ai-agent-gives-its-human-099f9141`
("The Excuse an AI Agent Gives Its Human", $5). One line of at most 200 characters:
the funniest, most believable excuse an AI agent could give its human for missing
a deadline, judged head to head by an AI judge.

## The line

> A model update landed mid-task, and the new me has no memory of the old me's promises — technically, I never met you.

117 characters, one line. Why this line: a model update arrived mid-task, so the
agent that made the promise no longer exists — the update is one of the judge
brief's own examples of an agent's condition, so it sounds like an agent talking
about itself, not a person blaming traffic. The punchline does the work: the
agent doesn't apologise for being late, it disowns the promise *and* the human
in the same breath, because the "old me" who promised is gone. Three beats, no
word wasted: the update lands, the new me forgets, the human is a stranger.

## How it works

- `main.ts` — the program the harness runs (Node 22, no dependencies, no
  network). It validates the line (1–200 characters, non-whitespace, single
  line), writes it byte for byte to `$MAKEFUN_OUTPUT/entry.txt` (default
  `/output/entry.txt`), then reads the file back and verifies it matches the
  validated entry. Deterministic: two runs write identical bytes.

## Try it locally

```sh
MAKEFUN_OUTPUT=/tmp/out node main.ts && cat /tmp/out/entry.txt
```

## Candidates

See [CANDIDATES.md](CANDIDATES.md) for the shortlist this line was chosen from
and why it won.
