# Character Sheet Prompt Template
### For Nano Banana Pro — generates the @Image1 reference for Seedance 2.5

---

## STEP 1 — Portrait First (4:5 ratio)

Generate this before the full sheet. Get the face exactly right here.
Use this as the reference image when generating the three-panel sheet.

```
Photorealistic character reference photograph. Chest-up portrait of a [AGE, GENDER]
against a plain mid-grey seamless studio backdrop, facing camera straight on.

FACE: [Skin tone and undertone. Jaw shape. Eye color and shape. Nose. Lips. Brows.
Any distinctive features. Be specific — the more ordinary and precise, the more real.]

HAIR: [Color. Length. Texture. Condition — wet / dry / tied up / messy loose]

WARDROBE: [Top layer visible from chest up — fabric, color, condition]

EXPRESSION: [What a camera would see — not "nervous" but "jaw slightly forward,
mouth closed, eyes holding still"]

CONDITION: [Clean / wet / wounded / dirty — and exactly where on the body]

DISTINGUISHING FEATURE: [Tattoo location and description / scar / glasses / earrings]

Background: plain mid-grey seamless studio backdrop, completely empty, evenly lit,
no texture, no gradient, no shadow cast on the backdrop.

Shot on ARRI Alexa 35, 85mm prime lens, soft even studio lighting from a large
softbox key at 45 degrees with gentle fill, no hard shadows, no rim light, neutral
white balance, sharp focus throughout, visible skin texture and pores, no retouching,
fine film grain. Original character, not resembling any existing person or public figure.

NEGATIVE: no smooth or airbrushed skin, no beauty filter, no CGI look,
no gradient background, no heavy makeup, no resemblance to any real person.
```

---

## STEP 2 — Three-Panel Character Sheet (16:9 ratio)
### Attach the approved portrait as a reference image before generating

```
Photorealistic character reference sheet. Three panels side by side against a plain
mid-grey seamless studio backdrop. One continuous background across all three panels.

LEFT PANEL — chest-up portrait of a [AGE, GENDER], facing camera straight on,
level chin, calm neutral expression, eyes into the lens.
[PASTE FULL FACE AND HAIR DESCRIPTION FROM PORTRAIT]
[PASTE WARDROBE DESCRIPTION — top layer only]

CENTRE PANEL — full-length front view of the same [GENDER], framed from the
shoulders down so the head is DELIBERATELY CROPPED OUT OF FRAME.
This is an intentional headless costume display — the clothing simply stops at the
collar line. The omission is deliberate so the model locks onto one single face
from the LEFT panel only.
Standing upright and square to camera, weight evenly on both feet, arms hanging
relaxed and straight at the sides, nothing crossing the body, hands open and visible.
[PASTE FULL BUILD AND WARDROBE DESCRIPTION — head to toe]
[INCLUDE DISTINGUISHING FEATURES — tattoo location, etc.]

RIGHT PANEL — full-length rear three-quarter view of the same [GENDER],
HEAD FULLY VISIBLE AND COMPLETE from the top of the skull down to the feet.
[PASTE HAIR DESCRIPTION — from behind]
[PASTE WARDROBE DESCRIPTION — rear view]
Same neutral upright posture, arms at sides.

CRITICAL: Only the CENTRE panel is headless. LEFT and RIGHT panels both include
the head. This character has a head and face in every shot of the film.

All three panels identically lit and identically scaled. Plain mid-grey seamless
studio backdrop, completely empty, evenly lit, no texture, no gradient.

Shot on ARRI Alexa 35, 85mm prime lens, soft even studio lighting from a large
softbox key at 45 degrees with gentle fill, no hard shadows, no rim light,
neutral white balance, sharp focus throughout, visible skin texture and pores,
no retouching, fine film grain.
Original character, not resembling any existing person or public figure.

NEGATIVE: no resemblance to any real person or influencer, no identity drift
between panels, no smooth or airbrushed or waxy or CGI-looking skin, no beauty
filter, no heavy makeup, no arched back or posed stance, no props, no text,
no watermark, no branding.
```

---

## STEP 3 — Skin Realism Pass (if skin looks too perfect)
### Run this as a follow-up edit on the approved sheet

```
Take this exact image and increase skin and overall realism only.
Keep the same identity, pose, outfit, panel layout, background,
and lighting exactly as shown.

SKIN REALISM: replace any smooth, airbrushed, or beauty-filter skin with
genuinely photographed skin texture — real visible pores across the forehead,
cheeks and nose, subtle natural uneven tone, faint texture irregularities.
The character should still look [attractive / natural / weathered] but through
real photographic texture, not a smoothed surface.

NEGATIVE: no smooth, plastic, waxy, glass-smooth, or CGI-rendered skin.
No beauty filter. No change to face shape, identity, pose, wardrobe, or background.
```

---

## If Using Real Photos (4 photos uploaded)

Replace the description-based prompt above with this identity lock:

```
CRITICAL IDENTITY LOCK: @Image1, @Image2, @Image3, and @Image4 are all photos
of the exact same real person. This is not a composite or blended face.
They must be immediately and unmistakably recognizable as the specific individual
shown — with their exact face shape, exact eye shape and color, exact nose,
exact lips, exact eyebrow shape, exact jawline, exact skin tone, and exact hair
color, texture, and length as shown.
Do not average, generalize, beautify, or drift toward a generic model-like face.
If any single reference is clearer than the others, prioritize matching that one
exactly rather than blending all four into something new.

A four-panel character reference sheet: front / three-quarter / side / face and
texture detail.

Wardrobe: [DESCRIBE OUTFIT]

Pure white seamless background across all four panels. Soft texture-revealing
side-angle lighting. Real skin texture, never airbrushed.

NEGATIVE: no identity drift from the uploaded references under any circumstances,
no generic or composite or averaged face, no beautification, no smooth or
airbrushed or CGI-looking skin.
```

---

> **Why the headless centre panel?**
> It leaves exactly one face in the sheet. If two full faces appear at different
> scales, Seedance averages them into a blurred, unstable identity. One face,
> used twice, locks the model onto a single identity that holds across blocks.
>
> **Upload order for Seedance (never change this):**
> @Image1 = Character 1 sheet · @Image2 = Character 2 sheet · @Image3 = Location · @Image4 = Last frame of previous block
