# Location Plate Prompt Template
### For Nano Banana Pro — generates the @Image3 environment reference for Seedance 2.5

---

> **Why lock the location before the video?**
> If Seedance has to invent a location AND handle a performance at the same time,
> it fails both. Lock the environment as a reference plate first.
> Every block prompt then says "match @Image3" instead of re-describing the space.

---

## Location Plate Prompt (16:9 or 9:16)

```
[Photorealistic cinematic establishing plate / Photorealistic interior photograph],
[wide shot / medium / three-quarter angle]. No people. Empty of people entirely.

SETTING: [Type of space — small rented kitchen / industrial gym / dense forest /
modern apartment bedroom / car interior from driver's seat POV]

ERA / STYLE: [Contemporary / 1970s / brutalist / minimal / cluttered and lived-in]

TIME OF DAY: [Pre-dawn / golden hour / overcast noon / late dusk / night]

WEATHER (exterior only): [Heavy rain / dry / fog / overcast / clear]

KEY ELEMENTS:
[Name every specific object that must appear — and where it sits in the frame.
Foreground / mid-ground / background. Left / centre / right of frame.
Example: "A chalk bowl on a low stand with white dust around its base,
foreground left. A black power rack mid-ground centre. Tall steel-framed
windows along the right wall."]

LIGHTING:
[Name the actual physical light source — never write "good lighting" or
"cinematic lighting" without naming what is producing the light.
Example: "A single warm tungsten under-cabinet strip switched on, acting as
the real practical key with soft falloff, against cold blue pre-dawn light
coming through a window just out of frame — the two sources visibly disagree
in colour temperature."
Example: "Hard directional window daylight from camera-right as the primary key,
throwing long shadow bars across the floor. Cool LED battens overhead as a
secondary fill in the background only."]

COLOUR GRADE:
[Be specific — not "dark and moody" but named values.
Example: "Cold blue shadows, warm amber pooling only under the cabinets,
slightly crushed blacks from phone sensor limits, faint digital luminance
noise in darker areas."
Example: "Near-monochrome charcoal and graphite with cool blue-grey highlights
on the steel, one pocket of warm daylight at the far end. Rich blacks,
controlled highlights, gently desaturated."]

CAMERA POSITION: [Low at hip height / eye level / overhead / three-quarter angle
looking down the length of the floor — describe where the camera is and what
it is looking at]

MOOD: [One line — what does this place feel like. Not for the model — for you,
to check your prompt is coherent.]

This must read as an actual photograph taken [on a phone in a real space /
on a real camera] — NOT a digital render, NOT a 3D visualisation, NOT a
video-game environment, NOT an AI-generated look.

Shot on [ARRI Alexa 35 / Sony A7S III / recent smartphone], [focal length],
[deep focus / shallow], 35mm grain, [natural light only / mixed practical sources].

NEGATIVE: no people, no text, no logos, no CGI or 3D render look,
no flat or shadowless lighting, no plants (unless specified),
no clutter (unless specified), [add anything specific you don't want].
```

---

## Examples by Location Type

### Small Apartment Kitchen (pre-dawn, phone-shot feel)
```
This must read as an actual photograph taken on a phone in a real apartment.
NOT a digital render, NOT a 3D visualisation, NOT an interiors magazine shoot.

Location reference plate, completely empty of people. A small, slightly cluttered
rented apartment kitchen at 5am. Laminate countertop with real wear marks,
a stainless sink, a kettle, an open box of oats, a phone charger cable trailing
off the edge. Cheap white cabinets, one door very slightly misaligned.
A nylon gym bag sitting on the floor against the cabinets.

LIGHTING: a single warm tungsten under-cabinet strip switched on, acting as the
real practical key with soft falloff, against cold blue pre-dawn light coming
through a window just out of frame — the two sources visibly disagree in colour
temperature. The room is under-lit and a little too dim.

COLOUR: cold blue shadows, warm amber pooling only under the cabinets,
slightly crushed blacks, faint digital luminance noise in the darker areas.

NEGATIVE: no CGI, no 3D render, no styled or minimalist interior, no plants,
no people, no film grain, no halation, no cinematic colour grade,
no even or flattering lighting, no text or branding.
```

### Industrial Gym — Wide Establishing (cinematic)
```
Location reference plate, 9:16, completely empty of people.
A large modern strength gym on an industrial upper floor. Deep charcoal rubber
tile flooring, faintly reflective. Exposed dark grey concrete ceiling with black
conduit and suspended linear LED battens running in parallel into the distance.
Raw concrete columns. Matte black power racks and benches, plate trees loaded
with black bumper plates, grey and black cable machines. At the far end, tall
windows letting in soft daylight that glows against the dark interior.

CAMERA: low, hip height, three-quarter angle looking down the length of the floor.
LIGHTING: linear LED battens as the main practical, cool and directional.
Daylight from the far windows as a secondary, warmer, creating depth.
COLOUR: near-monochrome charcoal with cool blue-grey highlights on steel,
one pocket of warm daylight at the far end. Rich blacks, controlled highlights.

NEGATIVE: no CGI, no 3D render, no showroom look, no people, no flat lighting,
no fluorescent tint, no neon, no real brand logos, no text.
```

### Dense Forest — Exterior Night / Dusk (cinematic horror / drama)
```
Photorealistic cinematic establishing plate, wide shot, no people.
A dense temperate forest at late dusk in torrential rain. Tall dark pine and
silver birch trunks crowd the frame, bark blackened and slick with water.
Thick green moss climbs the lower trunks and covers exposed roots. The forest
floor is wet black earth, sodden brown leaf litter, broken branches, standing
puddles pocked by falling rain. A narrow muddy trail runs from foreground into
mid-ground, churned and waterlogged, winding between trunks and disappearing
into fog. In the mid-ground, slightly off-centre, a large granite boulder
roughly the height of a seated person, its top furred with dark green moss.
Low ground fog lies in bands between the trunks. Heavy rain falls in visible
sheets. The canopy overhead is dense and near-black.

COLOUR: desaturated teal-green and grey, deep crushed blacks, cold blue-grey.
MOOD: isolated, oppressive, hopeless, miles from anyone.

Shot on ARRI Alexa 35, 32mm anamorphic, deep focus, 35mm grain,
water droplets on the lens, natural overcast light only.

NEGATIVE: no people, no artificial light sources, no CGI, no text.
```

---

> **Upload order for Seedance (never change this):**
> @Image1 = Character 1 · @Image2 = Character 2 · @Image3 = Location plate · @Image4 = Last frame of previous block
