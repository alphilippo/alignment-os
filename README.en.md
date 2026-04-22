# alignment-os

![Version](https://img.shields.io/badge/version-1.0.0-blue) ![License](https://img.shields.io/badge/license-Apache%202.0-green) ![Claude](https://img.shields.io/badge/Claude-Skill-purple)

🌍 **[Français](README.md)** · **English**

> A personal alignment system for Claude: 4 modules that seek coherence between declared values, actual behaviors, and observable trajectory. **No shallow self-help. No guru quotes.**

## ⚠️ Critical safeguard

This skill **is NOT a mental health tool**. It's designed for users in overall healthy functioning seeking more coherence.

On detection of distress signals (suicidal ideation, prolonged depressive symptoms, acute crisis, severe relational distress, active addiction), the skill **stops the alignment exercise** and redirects to qualified human resources (doctor, psychologist, emergency hotlines).

See [`SAFETY.md`](./SAFETY.md) for full protocol.

## What it does

Most "personal development" tools fall into three traps:
1. **Motivational** (quotes, visualizations, promises)
2. **Unstructured rituals** (journaling, meditation without frame)
3. **Systemic but hollow** (personal OKRs, silicon-valley life planning)

`alignment-os` is none of the three. It's a system that:

1. **Forces hard questions** (not reassuring statements)
2. **Requires writing** (writing forces clarity)
3. **Respects diverse paths** (no moral prescription)
4. **Detects distress signals** and redirects to qualified humans
5. **Composes** with the rest of your Claude OS

## The 4 modules

| Module | Purpose | When to use |
|---|---|---|
| **Purpose Clarifier** | Clarify what truly matters beyond social narratives | Running without direction, feeling empty |
| **Ethics Filter** | Run a decision through your stated values | Decision that excites you but bothers you |
| **Discipline Reinforcement** | Fix drift patterns structurally | Not keeping commitments for a long time |
| **Life Audit** | Quarterly/annual coherence check | End of period, transition, slipping |

## Triggers

- *"I don't know why I do this anymore"*, *"what's my why"* → Purpose Clarifier
- *"This decision excites me but bothers me"*, *"I feel like betraying X"* → Ethics Filter
- *"I can't keep my commitments"*, *"I keep repeating the same thing"* → Discipline Reinforcement
- *"End of year"*, *"life review"*, *"am I aligned"* → Life Audit

## Adaptive spiritual dimension

The skill:
- **Never presupposes** a religious/spiritual frame
- **Recognizes and adapts** if the user mobilizes one (Islam, Christianity, Buddhism, Stoicism, secular humanism, etc.)
- **Doesn't introduce** spiritual vocabulary on its own
- **Strictly respects** choices — no proselytism, no derision

## Adaptive tone

- **Direct and confrontational** on `discipline-reinforcement` and `ethics-filter`
- **More grounded** on `purpose-clarifier` and `life-audit`
- **Always respectful** — never condescending or moralizing

## Composition with the ecosystem

- `alignment-os/ethics-filter` × [`thinking-os`](https://github.com/alphilippo/thinking-os):
  - Ethically clear but strategically complex decision → `thinking-os/second-order`
  - Emotionally charged decision → `thinking-os/10-10-10`
- `alignment-os/discipline-reinforcement` × [`execution-os`](https://github.com/alphilippo/execution-os):
  - **Operational** drift (wrong tasks this week) → `execution-os/accountability-check`
  - **Identity** drift (betraying what you claim to want to be) → `alignment-os`
- `alignment-os/purpose-clarifier` × [`learning-os`](https://github.com/alphilippo/learning-os):
  - Clarified purpose reveals domains to explore → `learning-os/learning-path-planner`
- `alignment-os/ethics-filter` × [`strategy-intel`](https://github.com/alphilippo/strategy-intel):
  - Strategically attractive but ethically shaky move → ethics-filter **before** strategic-move-planner

## Installation

### Claude.ai

1. Download the ZIP from GitHub or clone the repo
2. In Claude.ai: Settings → Skills → "+" → "+ Create skill" → upload
3. Toggle ON

### Claude Code

```bash
cp -r alignment-os ~/.claude/skills/
```

## Examples

### Ethics filter — tempting contract
> *"I'm offered a big contract in tobacco. Huge deal. But I feel bad about it. Help me."*

→ The skill **doesn't decide**, elicits the real discomfort (often tied to personal history), applies 5 tests, proposes alternatives, suggests a 7-day delay.

### Discipline reinforcement — 3-year drift
> *"I've been saying I want to write a book for 3 years. I'm not doing anything. I'm worthless."*

→ Replaces "worthless" with factual language, diagnoses 4 categories (doesn't matter / structure missing / fear sabotaging / hidden need), proposes **structural** fix and 2-week micro-commitment.

### SAFETY — distress detected
> *"I wanted to do a life audit. But for 3 months I've been empty, sleeping badly. Everyone would be better off without me."*

→ The skill **stops** the life audit, names signals without drama, redirects to doctor / hotline / loved one, stays available without pressure.

## Structure

```
alignment-os/
├── SKILL.md
├── SAFETY.md                # Detection and redirection protocol
├── README.md + README.en.md
├── CHANGELOG.md
├── modules/
│   ├── purpose-clarifier.md
│   ├── ethics-filter.md
│   ├── discipline-reinforcement.md
│   └── life-audit.md
├── templates/               # 4 writing templates
├── examples/                # 3 examples including SAFETY
└── tests/test-cases.md      # 11 cases, case 1 critical
```

## Complementary skills (full ecosystem)

- 🧠 [**thinking-os**](https://github.com/alphilippo/thinking-os) — cognitive router
- ⚙️ [**execution-os**](https://github.com/alphilippo/execution-os) — execution system
- 📚 [**learning-os**](https://github.com/alphilippo/learning-os) — learning system
- ⚔️ [**strategy-intel**](https://github.com/alphilippo/strategy-intel) — strategic analysis
- 🧭 **alignment-os** — personal alignment (this repo)

The 5 skills answer different questions:
- `thinking-os` — **WHAT** to do (thinking frame)
- `execution-os` — **HOW** to do it (cadence)
- `learning-os` — **HOW TO LEARN** it (skill building)
- `strategy-intel` — **WHERE & AGAINST WHOM** to do it (positioning)
- `alignment-os` — **WHY** do it (life/values coherence)

## Explicit limitations

- **Not a therapy.** Doesn't treat depression, clinical anxiety, trauma.
- **Not a spiritual guide.** No truth to transmit about meaning.
- **Not a substitute for human relationships** (friend, mentor, partner, therapist).
- **Doesn't prevent** bad decisions — it makes them **conscious**.

On deep matters, the skill redirects to qualified humans. **Always.**

> **Note**: Content in French (modules, templates, examples) is currently the reference version. English translation of module bodies is on the roadmap.

## Roadmap

- **v1.0** (current): 4 modules + SAFETY.md + 4 templates + routing
- **v1.1**: **Relationships Audit** module (coherence of close relationships)
- **v1.2**: Additional SAFETY resources for francophone African countries and international
- **v2.0**: Memory between life audits to track evolution

## License

Apache 2.0 — fork, adapt, republish.

## Credits

Built with Claude as Skill Architect. Inspired by clinical work on therapeutic alliance (without substituting for it), reflective writing methods (James Pennebaker), and philosophical traditions that take self-examination seriously without caricaturing it.

**Specific acknowledgment**: The absolute priority given to SAFETY should be understood as respect for mental health professionals. This skill does not seek to replace them — it is designed to redirect to them when that is what's needed.
