# Multi-Domain Expert Research Skill for Claude Code

A standalone Claude Code skill that runs any research topic through a panel of up to 42 domain experts in parallel, then synthesises their findings into a cross-domain report — all saved as local markdown files.

No server. No database. No API keys beyond your Claude subscription.

---

## What It Does

You give it a topic. It deploys up to 42 domain experts simultaneously — each one analyses the topic from their unique perspective across human sciences, design, philosophy, systems thinking, business, and specialised lenses. When all experts finish, a synthesis agent cross-references their findings and extracts the most important insights, contradictions, and blind spots.

Everything is written to a folder of plain markdown files you can read, share, or import into Notion or Obsidian.

### Example

```
/research "How might a mobile game built around koi ponds create restorative experiences for burnout recovery?"
```

Produces a folder like:

```
research-output/
  koi-pond-mobile-game-burnout-recovery/
    README.md
    00-synthesis.md          ← Start here
    01-ux-researcher.md
    02-behavioral-psychologist.md
    03-cultural-anthropologist.md
    04-game-designer.md
    05-environmental-psychologist.md
    06-metaphysics-spiritual-scholar.md
    07-cognitive-scientist.md
    08-sound-music-expert.md
    09-market-analyst.md
    10-philosopher-ethicist.md
```

---

## Expert Panel (42 domains)

The skill auto-selects the most relevant experts for your topic. You can control exactly how many to use with `--experts N`.

### Human Sciences
| Expert | What they bring |
|--------|----------------|
| Behavioral Psychologist | Decision-making, motivation, emotion, habit formation |
| Cognitive Scientist | Attention, memory, cognitive load, perception, mental models |
| Neuroscientist | Brain mechanisms, neural reward systems, embodied cognition |
| Clinical Psychologist | Mental health, wellbeing, coping, therapeutic value, harm potential |
| Depth Psychologist (Jungian) | Archetypes, shadow, individuation, collective unconscious |
| Sports & Performance Psychologist | Flow states, peak performance, resilience, pressure |
| Child Development Specialist | Developmental stages, play, learning, age-appropriateness |
| Gerontologist | Aging, cognitive changes, elder experience, accessibility over time |
| Cultural Anthropologist | Cultural context, rituals, values, cross-cultural meaning |
| Anthropologist of Religion | Sacred/profane, ritual structure, myth, spiritual meaning-making |
| Sociologist | Social dynamics, community, identity, power structures |
| Historian | Historical context, precedent, long-term patterns |
| Linguist | Language, framing, discourse, semiotics of text, naming |

### Experience & Design
| Expert | What they bring |
|--------|----------------|
| UX Researcher | Usability, user journeys, friction, mental models |
| Interaction Designer | Input/output loops, affordances, feedback, moment-to-moment feel |
| Game Designer | Mechanics, loops, progression, challenge curves, player agency |
| Narrative Designer | Storytelling, world-building, character, emergent narrative |
| Visual Arts Critic | Aesthetics, composition, art direction, visual language |
| Motion Designer / Animator | Time, rhythm, easing, emotional motion language |
| Sound & Music Expert | Sonic identity, emotional resonance, sound design |
| Music Therapist | Healing properties of music, therapeutic applications |
| Accessibility Specialist | Inclusive design, disability considerations, universal access |
| Urban Designer / Architect | Space, flow, scale, designed environments |
| Environmental Psychologist | Place, nature, restorative environments, attention restoration |

### Philosophy & Meaning
| Expert | What they bring |
|--------|----------------|
| Philosopher / Ethicist | Meaning, ethics, assumptions, value tensions |
| Phenomenologist | Lived experience, embodiment, presence, consciousness |
| Semiotician | Signs, symbols, codes, representation, signifier/signified |
| Metaphysics / Spiritual Scholar | Archetypes, consciousness, non-dual traditions, transcendence |
| Art Historian | Art movements, influence, canon, context, iconography |
| Play Researcher / Ludologist | Nature of play, game theory, ludic experience |

### Systems & Science
| Expert | What they bring |
|--------|----------------|
| Systems Thinker | Feedback loops, emergence, leverage points, unintended consequences |
| Complexity Scientist | Self-organisation, non-linearity, adaptive systems |
| Ecological Designer / Biomimicry Expert | Nature as model, sustainability, regenerative design |
| Technology Architect | Technical feasibility, platforms, scalability, implementation risks |

### Business & Society
| Expert | What they bring |
|--------|----------------|
| Market Analyst | Market size, competition, positioning, monetisation |
| Economist | Incentive structures, resource allocation, value creation |
| Political Scientist | Power, governance, policy, civic implications |
| Journalist / Media Critic | Narrative framing, public discourse, media representation |
| Legal / Ethics & Compliance Expert | Regulation, liability, data, IP, compliance risk |

### Specialised Lenses
| Expert | What they bring |
|--------|----------------|
| Educator / Learning Designer | Pedagogy, scaffolding, knowledge transfer, skill development |
| Community Organiser / Social Designer | Participation, belonging, co-creation, grassroots dynamics |
| Futurist / Trend Analyst | Emerging patterns, weak signals, long-term trajectories |

---

## Install

**Step 1:** Find your Claude skills folder:

| OS | Path |
|----|------|
| Mac / Linux | `~/.claude/skills/` |
| Windows | `C:\Users\<your-username>\.claude\skills\` |

If the folder doesn't exist, create it.

**Step 2:** Copy `SKILL.md` from this folder into a subfolder called `research`:

```bash
# Mac / Linux
mkdir -p ~/.claude/skills/research
cp SKILL.md ~/.claude/skills/research/SKILL.md

# Windows (PowerShell)
New-Item -ItemType Directory -Force "$env:USERPROFILE\.claude\skills\research"
Copy-Item SKILL.md "$env:USERPROFILE\.claude\skills\research\SKILL.md"
```

**Step 3:** That's it. Open any Claude Code session and type `/research`.

---

## Usage

### Basic

```
/research <your topic>
```

### Options

```
/research <topic> --mode sequential     Run experts one at a time (shows progress as it goes)
/research <topic> --experts 5           Use only 5 experts (faster, lower API cost)
/research <topic> --depth quick         Briefer analysis per expert (~300 words each)
/research <topic> --depth deep          Thorough analysis per expert (~700 words each) [default]
/research <topic> --output ./my-folder  Save results to a custom folder
/research <topic> --no-web              Use model knowledge only, no web searches
```

### Modes

**Parallel (default):** All experts run at the same time. Fastest. Best for deep topics where you want maximum coverage.

**Sequential (`--mode sequential`):** Experts run one by one. You see each finding as it arrives. Good for watching the analysis unfold, or if you're hitting API rate limits.

---

## Reading the Output

Start with `00-synthesis.md`. It contains:

- **Convergence** — themes multiple experts agreed on
- **Divergence** — where experts disagreed (often the most interesting part)
- **Blind Spots** — what no expert covered
- **Priority Insights** — top 5 findings ranked by cross-domain confidence
- **Open Questions** — best follow-up questions
- **One-Sentence Takeaway** — the single most important finding

Then read individual expert files for depth on angles that interest you most.

---

## Tips

**Be specific with your topic.** The more concrete your question, the richer the insights.

- Too vague: *"tell me about meditation apps"*
- Better: *"What psychological and cultural barriers prevent Western millennials from sustaining daily meditation practice, and how might a game mechanic address them?"*

**Use `--experts 5` for a quick scan.** Five well-chosen experts in 3 minutes beats ten shallow ones. Use `--experts 42` for full coverage on important questions.

**The Divergence section is gold.** When experts disagree, it usually points to a genuine tension worth exploring.

**Re-run with a follow-up question.** Use insights from the synthesis to ask a more targeted second question.

---

## Requirements

- Claude Code CLI installed (`npm install -g @anthropic-ai/claude-code`)
- An active Anthropic API subscription or Claude.ai Pro/Team plan
- Nothing else

---

## Origin & Credits

Created by **Baki Bektas** as part of the [Between Ponds](https://github.com/Threchette/BetweenPonds) project — a fictional game concept designed to stress-test how conflicting domain expert opinions surface when multiple specialists review the same brief.

This skill was extracted from that larger multi-agent research infrastructure and stripped down to be fully self-contained. The Between Ponds game concept deliberately creates tension between fields (child safety vs. anonymity, monetization vs. accessibility, cultural authenticity vs. global scale), and this research skill is the engine that surfaces those conflicts by deploying domain experts in parallel.

The same underlying pattern — deploying multiple expert personas in parallel and synthesising across their findings — is what makes multi-domain research qualitatively different from asking a single AI the same question.

The key insight: experts don't just bring different answers. They bring different *questions*. A philosopher asks "what does this assume?" A behavioral psychologist asks "what behaviour does this reinforce?" An anthropologist asks "what does this mean to someone from a different culture?" The synthesis is where those different questions collide and produce something none of them would find alone.

Open source — free to use and share. as long as you keep it that way.
