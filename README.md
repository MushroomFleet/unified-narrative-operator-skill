# UNO: Unified Narrative Operator

A Claude Code skill that enhances narrative prose through a three-stage pipeline — expansion, repetition analysis, and precision editing. Built from the proven workflow behind the [Narrative Spittoon](https://spittoon.orangenai.com/) web application.

## What It Does

UNO takes a story page and runs it through three sequential stages in a single response:

**Stage 1 — UNO Enhancement**
Expands the page to close to 200% or above its original word count using five techniques:
- **Golden Shadow** — Develops undercurrents from characters and threads with unexplored potential
- **Environmental Expansion** — Enriches setting, sensory detail, and renders one insignificant object in exceptional detail
- **Action Scene Enhancement** — Temporal manipulation, spatial clarity, visceral impact for high-intensity sequences
- **Prose Smoothing** — Sentence rhythm, paragraph flow, transitions, stylistic consistency
- **Repetition Elimination** — Replaces unintentional repetition while preserving intentional literary devices

**Stage 2 — Semantic Echo Analysis**
Scans the enhanced text for five types of repetitive language patterns:
- Lexical Echoes (word repetition)
- Syntactic Echoes (structural patterns)
- Conceptual Echoes (recurring imagery)
- Rhythmic Echoes (cadence and pacing)
- Tonal Echoes (mood and voice)

Rates severity on a 1–5 scale and produces a structured report with specific revision recommendations.

**Stage 3 — Narrative Inpainting**
Applies precision inline edits to the sections flagged by the Echo report. Operates like image inpainting but for text — surgical modifications within defined boundaries, preserving everything outside the mask.

## Installation

### Option 1: Extract the `.skill` archive

Download `UNO.skill` from this repository and extract it to your Claude Code commands directory:

```
~/.claude/commands/UNO/
```

The extracted structure should be:

```
~/.claude/commands/UNO/
├── SKILL.md
├── README.md
├── references/
│   ├── 01-uno-enhancement.md
│   ├── 02-semantic-echo.md
│   ├── 03-narrative-inpainting.md
│   ├── nsl-context-guide.md
│   └── output-template.md
└── assets/
    └── nsl-1.1-specification.md
```

### Option 2: Clone and copy

```bash
git clone https://github.com/MushroomFleet/unified-narritive-operator-skill.git
cp -r unified-narritive-operator-skill/build/UNO ~/.claude/commands/UNO
```

## Usage

In Claude Code, say:

```
using UNO
```

or

```
use the UNO skill
```

followed by your story page text. UNO processes the page through all three stages and delivers the enhanced text with a processing summary.

### With NSL Context

For multi-page consistency, provide an NSL (Narrative Spittoon Language) file containing your project's world-building, character profiles, speech styles, and narrative frameworks:

```
using UNO

[NSL context or file path here]

[Your story page text here]
```

UNO works without NSL context — it uses the page itself and conversation context as the reference standard. NSL simply enables deeper consistency across pages in a larger project.

## Output

UNO delivers a final polished page followed by a processing summary:

| Stage | Words | % of Original |
|-------|-------|---------------|
| Original page | 500 | 100% |
| After UNO Enhancement (Stage 1) | 1,020 | 204% |
| After Narrative Inpainting (Stage 3) | 1,015 | 203% |

Plus enhancement techniques applied, echo issues identified and resolved, and a preservation verification checklist confirming all dialogue, plot points, and voice fidelity are intact.

## Core Principles

- **Dialogue is sacred** — all original dialogue is preserved word for word
- **No plot invention** — enhancement adds depth to what exists, never introduces new events
- **Voice fidelity** — the final text reads as if written by the original author in an inspired moment
- **Inpainting is surgical** — Stage 3 edits only what Stage 2 flags, preserving everything else
- **150% floor, 200%+ goal** — expansion targets are enforced with quality taking priority

## Live Web App

The full Narrative Spittoon web application (the original implementation this skill was derived from) is available at:

**[https://spittoon.orangenai.com/](https://spittoon.orangenai.com/)**

## Skill File Structure

```
UNO.skill (ZIP archive)
├── SKILL.md                    # Pipeline orchestrator with YAML frontmatter
├── README.md                   # Skill overview
├── references/
│   ├── 01-uno-enhancement.md   # Stage 1: Expansion protocol
│   ├── 02-semantic-echo.md     # Stage 2: Repetition analysis protocol
│   ├── 03-narrative-inpainting.md  # Stage 3: Precision editing protocol
│   ├── nsl-context-guide.md    # NSL bucket loading guide
│   └── output-template.md      # Final deliverable format
└── assets/
    └── nsl-1.1-specification.md  # Full NSL 1.1 specification
```

## License

See [LICENSE](LICENSE) for details.

---

## 📚 Citation

### Academic Citation

If you use this codebase in your research or project, please cite:

```bibtex
@software{unified_narrative_operator,
  title = {Unified Narrative Operator: Three-Stage Narrative Enhancement Pipeline for Claude Code},
  author = {Drift Johnson},
  year = {2025},
  url = {https://github.com/MushroomFleet/unified-narritive-operator-skill},
  version = {2.0.0}
}
```

### Donate:

[![Ko-Fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=3)](https://ko-fi.com/driftjohnson)
