# Guide to Best AI Filmmaking
### Realistic AI Video — Cinematic Films & AI Personas

> The seven-stage workflow behind the BMW M350 concept film and the Tess / LODE UGC ad.
> Claude / ChatGPT writes the prompts, Nano Banana Pro locks the character and the location, Seedance 2.5 generates the video in 12–20 second blocks, and CapCut or After Effects finishes it.

---

## What This Is

Realistic AI video usually breaks in three places, and this workflow is built to stop each one:

- **The face changes between shots.** A three-panel character sheet with a deliberately headless centre panel leaves Seedance exactly one face to lock onto.
- **The location changes between shots.** An empty location plate is generated before any video, so the model only has to handle the performance.
- **It looks like a 3D render.** Every prompt names a real camera, lens, light source and colour grade instead of words like "cinematic", and one Style DNA paragraph is pasted byte-identical into every block.

The same pipeline covers two kinds of video:
- **Cinematic short films**: narrative, atmospheric, character-driven
- **AI persona / UGC ads**: a realistic creator reviewing a product to camera

---

## Launch Film

30 seconds: the wall of prompts and failed renders most people start with, the seven stages, the three tools, frames from the BMW and Tess films, and the Character Sheet Builder in use.

▶️ [Watch the launch film](https://minhawork123-afk.github.io/guide-to-best-ai-filmmaking/tools/launch-film/)

Source: [`/tools/launch-film/`](./tools/launch-film/) — a single HTML file with no dependencies. The animation, particles and Web Audio soundtrack are all generated in your browser. If your browser blocks autoplay audio, tap once for sound.

---

## Proof of Concept

These were made entirely with this workflow.

### AI Persona / UGC Ad — LODE Protein (Tess)
Full pipeline: character sheet → product reference → location plates → Seedance 2.5 block prompts → CapCut edit

▶️ [Watch the finished video](https://lnkd.in/p/dXEZhci9)

The seven reference images and both Seedance block prompts for this film are in [`/examples/tess-lode-ugc/`](./examples/tess-lode-ugc/)

---

### Cinematic Concept Film — BMW M350 xDrive
Full pipeline: brief → script → character sheets → location plates → Seedance 2.5 → After Effects

▶️ [Watch on YouTube](https://www.youtube.com/watch?v=84tbDvXKknw)

---

### Live Workflow Breakdown
Watch the full production process explained step by step.

▶️ [Watch on YouTube](https://www.youtube.com/watch?v=bJXobsqN85w)

---

## The Tools

| Stage | Tool |
|---|---|
| Idea + Scripting | Claude / ChatGPT |
| Prompt Engineering | Claude / ChatGPT |
| Image Generation | Nano Banana Pro |
| Video Generation | Seedance 2.5 on OpenArt |
| Editing | CapCut / After Effects |

---

## The Workflow — 7 Stages

```
STAGE 1   IDEA
          Answer 5 brief questions in plain language

STAGE 2   SCRIPT
          Claude / ChatGPT — physical actions in [brackets] inline with dialogue

STAGE 3   REFERENCE IMAGE PROMPTS
          Portrait → Character Sheet → Skin Realism Pass → Location Plate

STAGE 4   IMAGE GENERATION
          Nano Banana Pro — in fixed order, saved with clear names

STAGE 5   VIDEO PROMPT ENGINEERING
          Claude / ChatGPT — block prompts with Style DNA, timestamps, @image refs

STAGE 6   VIDEO GENERATION
          Seedance 2.5, omni_reference, 1080p, native audio ON, block by block

STAGE 7   EDITING
          CapCut (fast/persona) or After Effects (cinematic)
```

Full documentation → [`GUIDE.md`](./GUIDE.md)

---

## Tools

### Character Sheet Builder
Describe your character in a simple form and get the two Stage 3 prompts for Nano Banana Pro, ready to copy-paste:
- **Portrait prompt (4:5)** — generate this first and get the face right
- **Three-panel character sheet prompt (16:9)** — chest-up portrait, deliberately headless full-length front view, full-length rear view with head visible

▶️ [Open the Character Sheet Builder](https://minhawork123-afk.github.io/guide-to-best-ai-filmmaking/tools/character-sheet-builder/)

Source: [`/tools/character-sheet-builder/`](./tools/character-sheet-builder/) — a single HTML file, nothing to install, runs entirely in your browser.

---

## Repo Structure

```
guide-to-best-ai-filmmaking/
│
├── README.md                        ← you are here
├── GUIDE.md                         ← full workflow documentation
├── index.html                       ← Faizan Film Labs website (GitHub Pages)
│
├── examples/
│   └── tess-lode-ugc/
│       ├── README.md                ← breakdown of this specific film
│       ├── prompts-seedance.md      ← full Seedance 2.5 block prompts A + B
│       └── assets/                  ← character sheet, product reference, location plates
│
├── tools/
│   ├── character-sheet-builder/
│   │   └── index.html               ← Character Sheet Builder web app
│   └── launch-film/
│       └── index.html               ← 30-second launch film
│
└── templates/
    ├── film-brief-template.md       ← blank brief for cinematic films
    ├── persona-brief-template.md    ← blank brief for UGC / persona content
    ├── character-sheet-prompt.md    ← fill-in character sheet prompt
    ├── location-plate-prompt.md     ← fill-in location plate prompt
    └── seedance-block-template.md   ← fill-in block prompt for Seedance 2.5
```

---

## Core Principles

**Name the mechanism, never the mood.**
Not *"make it cinematic"* — name the lens, the light source, the color grade.
Not *"make it realistic"* — say it was shot on a real camera, not a 3D render.
Not *"she looks scared"* — describe what a camera would actually see.

**Lock character first, location second.**
Every later prompt says *"match @Image1"* instead of re-describing from scratch.
A model inventing a location and lighting at the same time as a performance will fail both.

**Physical actions only. Never interior states.**
*"Her jaw tightens, she doesn't blink"* — not *"she is nervous."*
A video model renders what a camera sees. Give it something to see.

**Style DNA is written once, pasted byte-identical.**
Never reword it between blocks. One project, one signature.

**Dialogue and physical action never overlap.**
She speaks, or she moves. Never both at the same time.

---

## Quick Start

1. Read [`GUIDE.md`](./GUIDE.md) — the full workflow
2. Open [`/templates/film-brief-template.md`](./templates/film-brief-template.md) or [`/templates/persona-brief-template.md`](./templates/persona-brief-template.md)
3. Fill in your brief and paste it into Claude or ChatGPT
4. Follow the workflow through all 7 stages
5. See [`/examples/tess-lode-ugc/`](./examples/tess-lode-ugc/) for a real completed example

---

## Contributing

If you use this workflow and make something you're proud of, open a pull request and add your example to `/examples/`. Include:
- The finished video link
- Your reference image prompts
- Your Seedance block prompts
- A one-line description of what you made
- Optional, and the most useful part: a block that failed and the prompt change that fixed it

---

## License

MIT — use freely, credit appreciated.

---

*Made by Fazi, AI filmmaker and multi-language YouTube creator, at [Faizan Film Labs](https://www.faizanfilmlabs.online/).*
*[Watch the live workflow breakdown on YouTube](https://www.youtube.com/watch?v=bJXobsqN85w)*
