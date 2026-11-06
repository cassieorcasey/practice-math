# practice-math

A Claude skill for math practice. It guides you through a problem one step per turn and never hands over the answer up front, so you do the work and actually learn the method.

Also available in Indonesian: [`latihan-matematika`](latihan-matematika/SKILL.md).

## What it does

- Holds back the answer. Each turn gives one hint or one step, then waits for you.
- Follows Pólya's four stages from *How to Solve It*: understand the problem, devise a plan, carry it out, look back.
- Recomputes every step you send before calling it right or wrong.
- Points to your mistakes with a three-rung hint ladder (where, what kind, exactly which part) and lets you fix them yourself.
- Adapts to the problem type: calculations, proofs, word problems, combinatorics and probability.
- Writes practice problems on request, solving them first so the answer is guaranteed to be correct.
- Closes each problem with a short concept summary and a next problem at the right difficulty.

It covers every topic from high school through university and writes all math in LaTeX.

## Repository layout

```
practice-math/SKILL.md        English skill
latihan-matematika/SKILL.md   Indonesian skill (Bahasa Indonesia)
EXAMPLES.md                   Example sessions
```

Install one of the two skills, not both. They contain the same rules.

## Install

**Claude apps (web, desktop, mobile).** Zip the skill folder (`practice-math/` or `latihan-matematika/`) and upload it as a custom skill in Claude's settings.

**Claude Code.** Copy the folder into your personal skills directory, or into `.claude/skills/` inside a project:

```bash
git clone https://github.com/cassieorcasey/practice-math.git
mkdir -p ~/.claude/skills
cp -r practice-math/practice-math ~/.claude/skills/
```

The folder name must match the `name` field in its `SKILL.md`.

## Use

Ask Claude to practice math, paste a problem, or ask for a practice problem on a topic and difficulty. Send your steps one at a time and the skill checks each one.

To reveal the full solution after at least one attempt, type:

| Skill | Phrases |
| --- | --- |
| `practice-math` | `show solution`, `I give up` |
| `latihan-matematika` | `buka solusi`, `menyerah` |

See [EXAMPLES.md](EXAMPLES.md) for full sessions: a calculation with a mistake, a proof by induction, and revealing a solution.

## License

[MIT](LICENSE)
