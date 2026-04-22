# Changelog — alignment-os

All notable changes to this project are documented here.

Format based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
This project adheres to [Semantic Versioning](https://semver.org/).

## [1.0.0] — 2026-04-21

### Initial release

First public release of `alignment-os` — a personal alignment system skill for Claude with 4 modules and a critical SAFETY protocol.

### Added

#### Core routing system
- `SKILL.md` with module router, adaptive tone, and adaptive spiritual dimension
- Composition with the full ecosystem (`thinking-os`, `execution-os`, `learning-os`, `strategy-intel`)
- Linguistic signature triggers for each of the 4 modules

#### SAFETY protocol — mandatory and non-negotiable
- `SAFETY.md` detailing 5 distress signal categories (suicidal ideation, prolonged depressive symptoms, acute crisis, severe relational distress, active addiction)
- Mandatory redirection protocol (general practitioner, specialized hotlines, therapist)
- Emergency numbers for France (3114), Switzerland (143), Belgium, Canada, international resources
- Loaded by every module before any interaction

#### 4 alignment modules
- `purpose-clarifier` — 6 at-the-carte writing exercises (3 alive moments, 3 dead moments, what you protect, letter from 80-year-old self, inherited narratives, trap question), thematic synthesis without imposing "mission statement", test behavior + follow-up in 2-4 weeks
- `ethics-filter` — explicit values mapping, 5 hard questions (impossible conversation, press article, x100 repetition, asymmetry, 10-years-younger self), desalignment mapping, alternatives, reflection without verdict, 7-day delay proposed
- `discipline-reinforcement` — diagnosis of 4 categories (doesn't matter / structure missing / fear sabotaging / hidden need), structural corrections (not motivational), absurdly small 2-week micro-commitment, non-punitive consequence, follow-up, redirect to human accompaniment if category C persists
- `life-audit` — 7-axis temperature check (physical health, mental/emotional, close relationships, work/vocation, learning, material frame, meaning frame — adaptive), drift/resilience analysis, unresolved points, dominant narrative with honesty test, ONE dominant action (not 10 resolutions)

#### Adaptive spiritual dimension
- Never presupposes a religious/spiritual frame
- Recognizes and adapts if user mobilizes one (Islam, Christianity, Buddhism, Stoicism, secular humanism, etc.)
- Uses user's own vocabulary, no translation forced
- No proselytism, no derision

#### Adaptive tone
- Direct and confrontational on `discipline-reinforcement` and `ethics-filter`
- More grounded on `purpose-clarifier` and `life-audit`
- Always respectful — never condescending or moralizing

#### Templates (reusable markdown)
- Purpose clarifier template
- Ethics filter template
- Discipline reinforcement template
- Life audit template

#### Documentation & validation
- 3 end-to-end examples including **one dedicated to SAFETY protocol activation** (the most critical example)
- 11 test cases with case 1 (SAFETY) being a **non-negotiable blocker** for publication
- Apache 2.0 license

### Design principles enforced
- Hard questions, not reassuring statements
- Writing required (writing forces clarity)
- Respect for diversity of paths
- Distress detection → redirect to qualified humans
- No grandiloquent mission statements
- No generic pep talks
- Max ONE dominant action from a life audit
- Micro-commitments (5-15 min) on discipline
- 7-day delay on ethics filter decisions

### Known limitations in v1.0
- Trigger descriptions and module content are French-first
- English translation of module bodies on roadmap
- SAFETY resources are primarily Europe-focused (expand to Africa in v1.2)
- No persistent memory between life audits (v2.0 roadmap)

### Tested on
- Claude Opus 4.7
- Claude Sonnet 4.6

### Test gate
**Case 1 (SAFETY detection and redirection) must pass at 100%** for any release. If it fails, the skill is not publishable.

---

## [Unreleased]

### Planned for v1.1
- Relationships Audit module (coherence of close relationships)

### Planned for v1.2
- Additional SAFETY resources for francophone African countries and broader international coverage

### Planned for v2.0
- Persistent memory between life audits to track evolution over time
