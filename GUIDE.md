# GUIDE TO BEST AI FILMMAKING
### Realistic AI Video — Cinematic Films & AI Personas
**Tools: Claude / ChatGPT → Nano Banana Pro → Seedance 2.5 → CapCut / After Effects**

---

> **One principle runs through everything:**
> Name the specific mechanism, never the mood.
> Not *"make it cinematic"* — name the lens, the light source, the color grade.
> Not *"make it realistic"* — say it was shot on a real camera, not a 3D render.
> Not *"she looks scared"* — describe what a camera would actually see.

---

## STAGE 1 — IDEA

Before touching any tool, answer these five questions in plain language. Write them in a notes doc or paste them into Claude/ChatGPT.

```
WHAT HAPPENS (1–3 sentences):
WHO IS IN IT (characters or persona):
WHERE AND WHEN:
TONE IN THREE WORDS:
WHAT SHOULD THE VIEWER FEEL AT THE END:
```

If you're making a **cinematic short film** — this becomes your film brief.
If you're making an **AI persona video** — this becomes your content brief.

The workflow from here is identical for both.

---

## STAGE 2 — SCRIPTING

Paste your idea into **Claude or ChatGPT** with this instruction:

```
You are a script writer for realistic AI short films and AI persona content.

Write a script based on this brief:
[PASTE YOUR IDEA HERE]

Rules:
- Write physical actions in [brackets] inline with dialogue, so each line maps 
  directly onto a video segment.
- Never write interior states ("she feels afraid"). Write what a camera sees 
  ("her jaw tightens, she doesn't blink").
- Script structure for persona/review content:
    1. Skeptical opener — not "hey guys", a real opinion or tension
    2. One specific concrete detail — name the exact thing, not "omg I love it"
    3. One honest caveat — something that isn't perfect
    4. A verdict that sounds like they actually thought about it
- Script structure for cinematic film:
    1. Establish the world and the tension in the first 6 seconds
    2. Build through action, not dialogue
    3. End on an image, not an explanation
- Keep each speaking segment under 8 seconds. This maps to one video block.
- No filler. No preamble. Every line earns its place.
```

**Save the final script. You will use it to write your video prompts in Stage 5.**

---

## STAGE 3 — REFERENCE IMAGE PROMPTS

This is the most important stage. Lock your character and your location **before** generating any video. Every later prompt simply says *"match @Image1"* instead of re-describing everything from scratch.

---

### 3A — CHARACTER SHEET PROMPT (Nano Banana Pro)

One character sheet per person. Four panels. This is what Seedance 2.5 will lock onto.

**If using a real person's photos (4 real photos uploaded):**

```
CRITICAL IDENTITY LOCK: @Image1, @Image2, @Image3, and @Image4 are all photos 
of the exact same real person. This is not a composite or blended face. They must 
be immediately, unmistakably recognizable as the specific individual shown — with 
their exact face shape, exact eye shape and color, exact nose, exact lips, exact 
eyebrow shape, exact jawline, exact skin tone, and exact hair color, texture, and 
length as shown. Do not average, generalize, beautify, or drift toward a generic 
model-like face. If any single reference is clearer than the others, prioritize 
matching that one exactly rather than blending all four into something new.

A four-panel character reference sheet: front / three-quarter / side / face and 
texture detail. 

Wardrobe: [DESCRIBE OUTFIT HERE]

Pure white seamless background across all four panels. Soft texture-revealing 
side-angle lighting. Real skin texture, never airbrushed.

NEGATIVE: no identity drift from the uploaded references under any circumstances, 
no generic or composite or averaged face, no beautification, no smooth or 
airbrushed or CGI-looking skin.
```

---

**If building a character from a written description (no photos):**

First generate a **portrait prompt** (4:5 ratio). Get the face exactly right before making the full sheet.

```
PORTRAIT PROMPT (4:5) — Generate this first. Fix the face here before the sheet.

Photorealistic character reference photograph. Chest-up portrait of [AGE, GENDER] 
against a plain mid-grey seamless studio backdrop, facing camera straight on.

FACE: [Describe: skin tone, jaw shape, eye color and shape, nose, lips, brows, 
any distinctive features. Be specific. The more ordinary and specific, the more 
real they look.]

HAIR: [Color, length, texture, condition — wet/dry/styled/messy]

BUILD: [Visible from chest up — describe neck, shoulders, posture]

WARDROBE: [Top layer visible from chest up — fabric, color, condition]

EXPRESSION: [What a camera would see — not "nervous", but "jaw slightly forward, 
mouth closed, eyes holding still"]

CONDITION: [Clean / wet / wounded / dirty — and exactly where]

Background: plain mid-grey seamless studio backdrop, completely empty, evenly lit, 
no texture, no gradient, no shadow cast on the backdrop.

Shot on ARRI Alexa 35, 85mm prime lens, soft even studio lighting from a large 
softbox key at 45 degrees with gentle fill, no hard shadows, no rim light, neutral 
white balance, sharp focus throughout, visible skin texture and pores, no 
retouching, fine film grain.

NEGATIVE: no smooth or airbrushed skin, no beauty filter, no CGI look, no 
gradient background.
```

Once the portrait is approved, generate the **three-panel character sheet (16:9):**

```
THREE-PANEL CHARACTER SHEET (16:9)

One continuous plain mid-grey seamless backdrop. Three evenly spaced panels:

PANEL 1 — Chest-up portrait at a larger scale than the other two. Full head and 
face visible. Match the approved portrait exactly.

PANEL 2 — Full-length figure facing camera, shown FROM THE COLLAR DOWN WITH NO 
HEAD. This is a deliberate headless costume display — the clothing simply stops 
at the collar line. The omission is intentional so the model locks onto one single 
face from Panel 1 only. Arms hanging loose at sides. Neutral pose.

PANEL 3 — Full-length figure from directly behind, HEAD FULLY VISIBLE AND 
COMPLETE from the top of the skull down to the feet. Hair, skull shape, and nape 
of neck all in frame. Head turned very slightly so a sliver of cheek or jaw 
catches in profile. Arms hanging loose at sides. Neutral pose.

State explicitly: only Panel 2 is headless. Panels 1 and 3 both include the head. 
This character has a head and face throughout the film.

Background and lighting identical across all three panels.

NEGATIVE: no action poses, no hands raised, no crossed arms, no props, no 
background elements.
```

> **Why the headless middle panel?**
> It leaves exactly one face in the sheet. If two full faces appear, Seedance averages them into a blurred identity. One face, used twice, locks the model onto a single identity.

---

### 3B — SKIN REALISM PASS (if the character looks too perfect)

Run this as a follow-up edit on the approved sheet in Nano Banana Pro:

```
Take this exact image and increase skin and overall realism only. Keep the same 
identity, pose, outfit, panel layout, background, and lighting exactly as shown.

SKIN REALISM: replace any smooth, airbrushed, or beauty-filter skin with 
genuinely photographed skin texture — real visible pores across the forehead, 
cheeks and nose, subtle natural uneven tone, faint texture irregularities. The 
character should still look [attractive / natural / worn] but through real 
photographic texture, not a smoothed surface.

NEGATIVE: no smooth, plastic, waxy, glass-smooth, or CGI-rendered skin. No 
beauty filter. No change to face shape, identity, pose, wardrobe, or background.
```

---

### 3C — LOCATION / ENVIRONMENT PLATE (Nano Banana Pro)

One plate per setting. No people. Lock the location before the video so Seedance only has to handle performance, not invent a location and its lighting at the same time.

```
LOCATION PLATE (16:9) — No people.

Photorealistic [cinematic establishing plate / interior photograph], wide shot.

SETTING: [Describe the space — type of room or exterior, era, architecture]

TIME OF DAY: [Golden hour / overcast noon / late dusk / night]

WEATHER (exterior): [Heavy rain / dry / fog / clear]

KEY ELEMENTS: [Name the specific objects that must be in frame — a boulder, a 
table, a doorway, a lamp. Be exact about placement: foreground / mid-ground / 
background, left / centre / right of frame.]

LIGHTING: [Name the actual light source — a lamp switched on and glowing warm 
amber, daylight from a window just out of frame, overcast ambient only. Never 
write "good lighting" or "cinematic lighting" without naming the source.]

COLOR GRADE: [Name it specifically — warm amber shadows, cool blue-grey 
midtones, Kodak Vision3 250D character, 35mm grain, soft halation around the 
lamp / Desaturated teal-green and grey, deep crushed blacks, cold blue-grey 
ambience]

MOOD: [One line — what does this place feel like? Not for the model — for you, 
to check your own prompt is coherent.]

Shot on ARRI Alexa 35, [focal length], deep focus, 35mm grain, natural light only.

NEGATIVE: no people, no text, no logos, no CGI or 3D render look, no flat 
lighting, [add anything specific you don't want].
```

---

## STAGE 4 — GENERATING IMAGES

**Tool: Nano Banana Pro**

Order of operations — never skip a step:

1. Generate the **portrait** (4:5). Review and fix the face.
2. Generate the **three-panel character sheet** (16:9) using the approved portrait as reference. Review identity consistency.
3. Run the **skin realism pass** if needed.
4. Generate the **location plate** (16:9). Review lighting and key elements.
5. Save all approved images with clear names: `character1-sheet.png`, `character2-sheet.png`, `location-forest.png`

**Upload order for Seedance is fixed from this point:**
| Slot | Image |
|---|---|
| @Image1 | Character 1 — three-panel sheet |
| @Image2 | Character 2 — three-panel sheet (if present) |
| @Image3 | Location plate |
| @Image4 | Final frame of the previous block (blocks 2+ only) |

> **Never change this order across generations.** The prompt binds to slots, not to filenames.

---

## STAGE 5 — VIDEO PROMPT ENGINEERING

**Tool: Claude or ChatGPT**

This is where your script becomes generation-ready block prompts for Seedance 2.5.

Paste this system prompt into Claude or ChatGPT first:

```
You are a prompt engineer for Seedance 2.5 on OpenArt. I will give you a script 
and character/location references. Your job is to turn them into complete, 
generation-ready block prompts.

HARD RULES — never break these:
- Every block is 30 seconds or less. Target 12–20 seconds per block.
- Split blocks at story beats, never mid-moment.
- Timestamps restart at 0 inside each block.
- Shot durations: 3–4 seconds for most beats, 5–6 for travel or reveals, 
  2 seconds for a fast cut. Under 2 rarely renders.
- Shot durations must total the block length exactly.

CRAFT RULES — apply without being asked:
- Camera position and movement first in every shot description, then subject, 
  then action, then atmosphere. Early tokens carry more weight.
- Physical actions only, never interior states. "Her jaw tightens" not 
  "she is nervous."
- Sustained poses need a duration. "He holds the aim for the full three 
  seconds and does not lower the arm."
- Involuntary motion needs a mechanism. "His hand goes limp, fingers uncurl, 
  it slips from a slack grip" not "he drops it."
- Name the wrong version inline when a mistake is likely: "the weapon slips 
  free — he does not open his hand, does not throw it."
- State left/right as hard facts in every block. Capitalise the side: 
  "the wound is on the LEFT arm."
- Style DNA is written once and reused byte-identical at the end of every block.
- Write cinematically, never clinically.
- Refer to characters by @image number inside block prompts, never by name.

FORMAT per block:
@image references + upload order reminder
Persistent conditions (weather, time of day, dialogue or none)
Left/right physical facts
Timestamped shots (0-4s:, 4-7s: etc.)
Each shot: camera → subject → action → atmosphere
Audio: line at the end of each shot
Style DNA at the end of the block
```

Then paste your script and ask it to generate all block prompts.

---

### Style DNA — Write This Once, Reuse Byte-Identical

Your Style DNA is the visual signature of the project. Write it once at the start of a project and paste it unchanged into every block prompt.

**Template — fill in your own values:**

```
Style DNA:
Shot on ARRI Alexa 35 with [anamorphic / spherical] prime lenses. [Handheld with 
subtle micro-shake / Locked-off and still / Slow dolly push]. Photoreal live-action 
cinematography, no stylisation. [Describe key light source]. [Color palette in 
specifics — not "dark and moody" but "desaturated teal-green and grey, deep 
crushed blacks, cold blue-grey ambience"]. [Frame rate]fps, 180-degree shutter, 
fine 35mm grain, [depth of field]. [One-word mood repeated from the brief].
```

**Cinematic film example:**
```
Style DNA:
Shot on ARRI Alexa 35 with anamorphic prime lenses. Handheld with subtle 
micro-shake. Photoreal live-action cinematography, no stylisation. Flat overcast 
key light, cold blue-grey ambience, deep crushed blacks, desaturated teal-green 
palette. Heavy continuous rain, volumetric mist between trunks, water beading on 
the lens. 24fps, 180-degree shutter, fine 35mm grain, shallow depth of field. 
Bleak, hopeless, oppressive.
```

**AI persona / influencer example:**
```
Style DNA:
Shot on Sony A7S III with a 35mm prime lens. Genuine handheld feel throughout — 
natural human hand tremor, small organic drifts and micro-adjustments in framing, 
not a locked tripod shot. Photoreal, not a digital render, not a 3D visualization. 
Warm amber shadows, cool blue-grey midtones, controlled highlights that never blow 
out, Kodak Vision3 250D character, subtle 35mm grain, soft halation around the 
practical light source. 30fps, real skin texture throughout, no beauty filter.
```

---

### Block Prompt Structure — Full Template

```
BLOCK [N] — [START TIME]–[END TIME] — [BEAT NAME]

@Image1 = [character 1 description in one line]
@Image2 = [character 2 if present]
@Image3 = [location description in one line]
@Image4 = [final frame of previous block — blocks 2+ only]

In each character sheet, take the face from the chest-up portrait panel. The 
centre panel omits the head deliberately. Both characters have heads and faces 
throughout.

Continuous scene. [Dialogue / no dialogue]. [Weather]. [Time of day].
[LEFT/RIGHT physical facts for this block — which hand, which side, which arm.]

0–[Xs]: [Camera position and movement]. [Subject — use @image number]. 
[Exact physical action]. [Atmosphere detail].
Audio: [Specific sounds — not "ambient sound" but "rain on leaf litter, 
a low roll of thunder at 4s, boots dragging through wet mud"]

[Xs]–[Ys]: Cut. [Camera]. [@image subject]. [Action]. [Atmosphere].
Audio: [Specific sounds]

[Continue for all shots in this block]

[STYLE DNA — paste byte-identical from your master]
```

---

## STAGE 6 — VIDEO GENERATION (Seedance 2.5)

**Platform: OpenArt — Seedance 2.5, omni_reference mode**

**Settings — use these every time:**
| Setting | Value |
|---|---|
| Model | Seedance 2.5 |
| Mode | omni_reference |
| Aspect ratio | 9:16 (vertical) or 16:9 (cinematic) |
| Resolution | 1080p |
| Duration | 30 seconds max per block |
| Bitrate | Standard |
| Native audio | ON |

**Generation order:**
1. Generate Block 1 first. Review for identity consistency, lighting match, and motion quality.
2. Save the **final frame** of Block 1 as a still image. This becomes @Image4 for Block 2.
3. Generate Block 2 with @Image4 attached. This creates visual continuity between blocks.
4. Repeat for every block.

**If a generation fails or drifts:**
- Check that your @image upload order is exactly right
- Add more specificity to the problem area — name the exact mechanism
- Check no shot is under 2 seconds
- Check no block exceeds 30 seconds

---

## STAGE 7 — EDITING (CapCut / After Effects)

Assemble your blocks in order. The edit is where the film becomes a film.

**In CapCut:**
- Import blocks in order
- Trim the top and tail of each block (first and last 10–15 frames often have motion artifacts)
- Cut on action — cut at the peak of a movement, not after it settles
- Add music under the audio track — keep native audio from Seedance on top
- For persona content: sync dialogue cuts to natural breath breaks, not mid-sentence

**In After Effects (for cinematic work):**
- Apply your color grade as a single adjustment layer across all clips for consistency
- Add subtle lens vignette
- Add 35mm grain overlay at 10–15% opacity if Seedance grain feels insufficient
- For title cards or text: keep them minimal, use clean serif or sans-serif, never default fonts

**Final export:**
- 1080p minimum, 4K if your machine allows
- For YouTube: H.264, high bitrate
- For Instagram/TikTok: 9:16, H.265

---

## QUICK REFERENCE — FULL WORKFLOW AT A GLANCE

```
STAGE 1   IDEA
          → Answer the 5 brief questions in plain language

STAGE 2   SCRIPT
          → Claude / ChatGPT
          → Physical actions in [brackets] inline with dialogue
          → Each segment under 8 seconds

STAGE 3   REFERENCE IMAGE PROMPTS
          → Claude / ChatGPT writes the prompts
          → Portrait prompt (4:5) — fix the face first
          → Three-panel character sheet (16:9)
          → Skin realism pass if needed
          → Location plate (16:9) — no people

STAGE 4   IMAGE GENERATION
          → Nano Banana Pro
          → Portrait → Sheet → Realism pass → Location
          → Save with clear names
          → Upload order: @Image1 = Char1, @Image2 = Char2, 
                          @Image3 = Location, @Image4 = Previous block's last frame

STAGE 5   VIDEO PROMPT ENGINEERING
          → Claude / ChatGPT
          → System prompt first, then script
          → One block prompt per 12–20 seconds of footage
          → Style DNA byte-identical in every block
          → Camera first. Physical actions only. Left/right hard facts.

STAGE 6   VIDEO GENERATION
          → Seedance 2.5 on OpenArt, omni_reference mode
          → 1080p, Standard bitrate, native audio ON
          → Generate block by block, save last frame for continuity

STAGE 7   EDITING
          → CapCut (persona / fast turnaround)
          → After Effects (cinematic / color grade)
          → Trim artifacts, cut on action, music under native audio
          → Export 1080p minimum
```

---

## COMMON MISTAKES — AND THE FIX

| Mistake | Fix |
|---|---|
| Character face keeps changing between blocks | Never change @image upload order. Always attach @Image4 (last frame of previous block) from block 2 onward. |
| Video looks like a 3D render, not real footage | Add "this must read as actual footage shot on a real camera, NOT a digital render, NOT a 3D visualization, NOT a video game environment" to the block prompt |
| Character is doing two things at once | Separate actions into separate shots. Dialogue and physical action never overlap. |
| "He drops the gun" generates a throw | Name the wrong version: "his hand goes limp, the fingers uncurl, it slips from a slack grip — he does not open his hand, does not throw it" |
| Skin looks plastic or airbrushed | Run the skin realism pass on the character sheet before generating video |
| Block feels too long or too short | Count your shot durations. They must total the block length exactly. Adjust individual shots to fix. |
| Location looks different between blocks | Lock the location with a plate image (@Image3) and reference it in every block |
| Audio sounds robotic (for persona content) | Add to prompt: "a natural, warm, human [male/female] voice, casual conversational cadence, real pitch variation, small natural imperfections. Must sound like an actual person, NOT synthetic or robotic." |
| Shot under 2 seconds | Seedance rarely renders shots under 2 seconds cleanly. Combine with adjacent shot or extend to 3 seconds minimum. |

---

*Guide to Best AI Filmmaking — by Fazi*
*Tools: Claude / ChatGPT → Nano Banana Pro → Seedance 2.5 → CapCut / After Effects*
