# Seedance 2.5 Block Prompt Template
### OpenArt · omni_reference mode · one block per 12–20 seconds of footage

---

## Seedance 2.5 Settings — Use These Every Time

| Setting | Value |
|---|---|
| Model | Seedance 2.5 |
| Mode | omni_reference |
| Aspect ratio | 9:16 (vertical) or 16:9 (cinematic) |
| Resolution | 1080p |
| Duration | 30 seconds max per block |
| Bitrate | Standard |
| Native audio | ON |

---

## @Image Upload Order — Never Change This

| Slot | Image |
|---|---|
| @Image1 | Character 1 — three-panel character sheet |
| @Image2 | Character 2 — three-panel sheet (if present) |
| @Image3 | Location / environment plate |
| @Image4 | Final frame of the previous block (blocks 2+ only) |

> The prompt binds to slots, not to filenames. If the order changes, the wrong
> reference gets the wrong character. Keep it identical across every generation.

---

## Shot Duration Rules

| Shot type | Duration |
|---|---|
| Standard beat | 3–4 seconds |
| Travel, reveal, collapse | 5–6 seconds |
| Fast cut | 2 seconds |
| Minimum | 2 seconds (under 2 rarely renders cleanly) |
| Block maximum | 30 seconds |

> Shot durations must total the block length exactly.
> Split blocks at story beats — never mid-moment.
> Timestamps restart at 0 inside each block.

---

## Block Prompt — Full Template

```
BLOCK [N] — [START TIME]–[END TIME] — [BEAT NAME]

@Image1 = [Character 1 — one-line description: name, key physical detail, wardrobe]
@Image2 = [Character 2 — one-line description, if present]
@Image3 = [Location — one-line description: space, time of day, key lighting]
@Image4 = [Final frame of Block [N-1] — BLOCKS 2+ ONLY. Omit for Block 1.]

In each character sheet, take the face from the [LEFT / chest-up portrait] panel.
The centre panel omits the head deliberately.
[CHARACTER NAME(S)] [has / have] a head and face in every shot of this film.

Continuous scene. [No dialogue / Voiceover only / Dialogue on camera].
[Weather condition]. [Time of day].
[LEFT/RIGHT physical facts for this block:
"The wound is on the LEFT arm. The gun is in the RIGHT hand.
The tattoo is on the inside of the LEFT wrist."]

0–[X]s: [Camera position and movement — be specific: "Handheld wide shot, 32mm
anamorphic, camera low at ankle height, pushing in very slowly."]
[@Image number] [exact physical action — what a camera would see, never interior states].
[Atmosphere detail — rain on leaf litter / chalk dust hanging in the light / etc.]
Audio: [Specific sounds — not "ambient sound" but named real sounds with timing:
"rain on foliage, a low roll of thunder at 4s, boots dragging through wet mud"]

[X]–[Y]s: Cut. [Camera]. [@Image subject]. [Action]. [Atmosphere].
Audio: [Specific sounds]

[Y]–[Z]s: Cut. [Camera]. [@Image subject]. [Action]. [Atmosphere].
Audio: [Specific sounds]

[Continue for all shots. Durations must total the block length exactly.]

[STYLE DNA — paste byte-identical from your project's master Style DNA below]
```

---

## Style DNA Templates

Write your Style DNA once per project. Paste it byte-identical at the end of every block — never reword it.

### Cinematic Film — Dark / Atmospheric
```
Style DNA:
Shot on ARRI Alexa 35 with anamorphic prime lenses. Handheld with subtle
micro-shake. Photoreal live-action cinematography, no stylisation.
Flat overcast key light, cold blue-grey ambience, deep crushed blacks,
desaturated teal-green palette. Heavy continuous rain, volumetric mist between
trunks, water beading on the lens. 24fps, 180-degree shutter, fine 35mm grain,
shallow depth of field. Bleak, hopeless, oppressive.
```

### AI Persona / UGC — Phone-shot Realism
```
Style DNA:
Shot on a recent smartphone. HDR, mild digital over-sharpening on edges,
visible luminance noise in dim areas, slight rolling shutter on pans,
clipped highlights near windows. Flat and ungraded. Genuine handheld feel
throughout — natural human hand tremor, small organic drifts and micro-adjustments,
slightly crooked horizons. Never a tripod, never a gimbal, never slow motion.
Real room tone. No music. No film grain, no halation, no cinematic grade.
```

### Cinematic Car / Product — Clean Industrial
```
Style DNA:
Shot on ARRI Alexa 35 with spherical prime lenses. Smooth controlled dolly
movement. Photoreal live-action cinematography, no stylisation.
Hard directional key light from camera-right, cool blue-grey fill,
deep blacks, desaturated steel and graphite palette. 24fps, 180-degree shutter,
fine 35mm grain, shallow depth of field on inserts, deep focus on wides. Cold, precise, controlled.
```

---

## Craft Rules — Apply to Every Block

**Camera first in every shot description.**
Then subject. Then action. Then atmosphere. Early tokens carry more weight.

**Physical actions only. Never interior states.**
❌ `she is nervous`
✅ `her jaw tightens, she doesn't blink, her hand is still`

**Sustained poses need a duration.**
❌ `he aims the gun`
✅ `he holds the aim for the full three seconds and does not lower the arm`

**Involuntary motion needs a mechanism.**
❌ `he drops it`
✅ `his hand goes limp, the fingers uncurl, it slips from a slack grip`

**Name the wrong version inline when a mistake is likely.**
`the weapon slips free — he does not open his hand, does not throw it`

**State left/right as hard facts. Capitalise the side.**
`the wound is on the LEFT arm` — models mirror reference images constantly.

**Dialogue and physical action never overlap.**
She speaks, or she moves. Never both at the same time.

**Refer to characters by @image number inside block prompts.**
`@Image1 sits slumped against the boulder` — not the character's name.
Character names are for the shot list, where you are reading, not the model.

---

## Common Mistakes and Fixes

| Mistake | Fix |
|---|---|
| Face changes between blocks | Never change @image upload order. Add @Image4 (last frame of previous block) from block 2 onward. |
| Video looks like a 3D render | Add: "this must read as actual footage shot on a real camera, NOT a digital render, NOT a 3D visualisation, NOT a video-game environment" |
| Character doing two things at once | Separate into two shots. Dialogue and action never overlap. |
| Skin looks plastic | Run the skin realism pass on the character sheet before generating |
| Shot durations don't add up | Count every shot's seconds. They must total the block length exactly. |
| Location looks different between blocks | Always attach the same @Image3 location plate to every block |
| Block too long | Target 12–20 seconds. Hard ceiling is 30 seconds. Split at a story beat. |
| Shot under 2 seconds | Combine with adjacent shot or extend to 3 seconds minimum |

---

> **See a completed example with all prompts:**
> [`/examples/tess-lode-ugc/prompts-seedance.md`](../examples/tess-lode-ugc/prompts-seedance.md)
