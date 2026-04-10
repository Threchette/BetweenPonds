# Between Ponds

> **This is a fictional game concept.** Between Ponds does not exist. Lanternwater Studio does not exist. The entire brief, studio backstory, team bios, seed round, cultural consultancy, is fabricated. The purpose of this repository is to stress-test how domain experts (human or AI) handle a design brief where legitimate expertise from different fields produces genuinely conflicting recommendations. Monetization vs. accessibility, child safety vs. anonymity, cultural authenticity vs. global scale, the tensions are real even if the game is not.

Created by **Baki Bektas** — open source, free to use and share.

**A made-up mobile game about tending a koi pond and writing to strangers you will never meet.**

Between Ponds is a fictional async social / cozy / collectible mobile title from the imaginary Lanternwater Studio (Berlin + Kyoto). You tend a small koi pond. Once every few days, you write a three-line message on a rice-paper scroll, attach it to a koi, and release it into "the current." The koi disappears for a day or two, then resurfaces in a stranger's pond somewhere else in the world. They read your words. They may keep the koi, or they may send it back with their own reply and a trace of their pond's genetics. There is no chat. There are no usernames. There are no profiles. Only koi, water, and short poems drifting between ponds.

## Why This Exists

This repository is a research artifact for exploring how conflicting domain expertise surfaces when multiple specialists review the same brief. The game concept is deliberately designed to create genuine tension between fields: a child-safety expert and a privacy advocate will disagree on anonymity; a monetization consultant and an accessibility specialist will disagree on pricing; a cultural consultant and a localization expert will disagree on how far Japanese aesthetics should bend for global audiences. None of them are wrong and that's the point.

## Repository Structure

### The Fictional Brief

Start here to understand the made-up game concept:

| File | What it does |
|------|-------------|
| [`docs/game-bible.md`](docs/game-bible.md) | The complete game design document, core loop, mechanics, message system, breeding, monetization, launch markets, age rating, and hard constraints. |
| [`docs/studio-fiction.md`](docs/studio-fiction.md) | The fictional Lanternwater Studio's team, origin story, cultural consultancy, seed round, and the seven questions posed to the advisory panel. |
| [`docs/open-questions.md`](docs/open-questions.md) | The eight open questions the advisory panel is asked to answer. |
| [`docs/visual-references.md`](docs/visual-references.md) | Descriptions and viewing instructions for the six concept images. |
| [`docs/cross-reference-instruction.md`](docs/cross-reference-instruction.md) | Mandatory quality requirement every expert finding must satisfy. |

### Visual Assets

| File | What it does |
|------|-------------|
| [`art/`](art/) | Six AI-generated concept images (`.png`) with accompanying description files (`.md`) — release ritual, winter hibernation, dormant shrine, pond at dawn (two variants), and message board. |

### Research Data

Results from different AI tools and methods reviewing the same brief:

| File | What it does |
|------|-------------|
| [`data/Expert-Round/`](data/Expert-Round/) | Multi-expert research round, the prompt used and the resulting report (Markdown + HTML). |
| [`data/Gemini-deep-research/`](data/Gemini-deep-research/) | Google Gemini Deep Research output, seed-round advisory review and the prompt that produced it. |
| [`data/TinyTroupe/`](data/TinyTroupe/) | Microsoft TinyTroupe simulated survey results (CSV) from AI-generated personas. |
| [`data/initial-research-via-notebookLM/`](data/initial-research-via-notebookLM/) | Early explorations via NotebookLM on agentic research architecture. |

### Research Skill

| File | What it does |
|------|-------------|
| [`research-skill/`](research-skill/) | A Claude Code skill definition for running structured multi-expert research investigations. |

### Presentation

| File | What it does |
|------|-------------|
| [`scaling-research-presentation.html`](scaling-research-presentation.html) | Standalone Reveal.js slide deck from the "Scaling Research" talk at the Employed.world meetup (10 April 2026, Berlin). Co-created with AI — some slides were deliberately left as raw AI output to show how AI-generated content can be both influential and out of touch. Open directly in any browser. |

## Disclaimer

Everything in this repository, the studio, the team, the game, the investors, the cultural consultancy, is fiction. Any resemblance to real studios, people, or products is coincidental. This is a research tool, not a pitch deck.
