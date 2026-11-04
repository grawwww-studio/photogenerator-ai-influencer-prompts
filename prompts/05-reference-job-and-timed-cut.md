# 05 · Two reusable prompt shapes: the reference job and the timed cut

Two short-film tests ("The Bulb", 5 s, one take; and a 12 s micro-film in four shots) used the same recipe with Seedance 2.0 in PhotoGenerator.ai. A keyframe made first is `@image1`; the character sheet from file 01 is `@image2`. The prompts below are the ones we ran, word for word, apart from the character's surname.

## The recipe in six lines

1. **Make the opening frame first.** An Image Generator still (8 credits), with the character sheet as `@image1` and a **reference job** sentence: *"It controls her identity only: her face, ... It does not control the light, the white wall, the pose or the framing."* Without that sentence the sheet's white wall and pose tend to come back in every picture.
2. **Judge the still against a written pass list** before spending video credits (identity side, one light source, no text on any object, nobody else in frame).
3. **Start the video from that still.** Text With Reference opens on `@image1`: the still is the first frame, the sheet is `@image2`. Give each reference one job in the prompt ("sets the room, the light, her clothes and her start position" / "controls her face ... not the light, background, pose or framing").
4. **Write the video prompt in labelled blocks:** SCENE CONTEXT, OUTPUT (for a multi-shot cut), REFERENCES, LOCKS (capital letters), COMPOSITION or GEOMETRY, CAMERA, ACTION or the shot list, ACTING (goal, obstacle, tactic), LIGHT, FILM, AUDIO, NEGATIVE.
5. **Time the action in seconds** inside each shot ("0.0-1.0 s: ... 2.5-3.0 s: ...") and name the cuts ("hard cuts at 3.0, 6.0 and 8.5 s") for a multi-shot clip. Our cuts landed about 1 to 1.3 s early (planned 3.0 / 6.0 / 8.5 s, got 2.0 / 4.7 / 7.4 s): plan for that.
6. **Judge the clip at the frame numbers you wrote down** and keep the misses in a log.

Both video prompts were about 3,500 characters long and were accepted by the prompt box.

## Test 1 · "The Bulb": one 5 s take

### S4-01 · Opening frame, 16:9, 2K, `@image1` = the character sheet (8 credits)
Pass list we used: the character reads at once (her hair, her face mark and her jewellery read at once); one bulb, the only light; bulb in the left third, her on the right third, waist-up; no text on boxes or tins; no second person. Fail on any of those -> one retry (8) with the failure as a lock line.
```
Reference 1 is @image1, her character sheet. It controls her identity only: her face, [your character's identity words: hair, face, marks, make-up, jewellery]. It does not control the light, the white wall, the pose or the framing.
A 16:9 film frame from a quiet thriller, shot on a 50 mm lens at eye height. An old basement storeroom at night: rough whitewashed brick walls with damp stains, bare wooden joists and floorboards for a ceiling, a metal shelf of plain unmarked cardboard boxes and paint tins at the back left, a closed plank door in the dark background. A single bare clear incandescent bulb with a glowing filament hangs on a black cord from a joist; it is caught at the far left of a swing, slightly motion-blurred, in the left third of the frame. The woman stands on the right third, seen from the waist up, three-quarter towards the bulb, chin level, eyes following the bulb, mouth closed, arms relaxed at her sides. The bulb is the only light: warm, hard, raking in from frame left, so the red side of her hair and her face is lit and the black side falls into deep shadow; the long tilted shadow of the shelf lies across the brick; fine dust hangs in the air near the bulb. Nobody else is in the room. Kodak Vision3 500T, fine grain in the shadows, soft halation around the filament, shallow depth of field with the focus on her eyes, real skin texture with visible pores, no clean digital look. She is a woman in her late twenties. No text, labels, logos or signs anywhere.
```

Result: identity and the single light passed, but two paint tins carried pseudo-text labels (a failed lock). We went on to the clip anyway.

### S4-02 · Text With Reference, Seedance 2.0, 5 s, 16:9, 720p, voice on; `@image1` = the S4-01 result, `@image2` = the sheet (40 credits)
Voice was on because with voice off the app had returned silent clips in earlier tests, and this shot needs its diegetic sound. Shown here with its line breaks; we typed it as one line.
```
SCENE CONTEXT: One 5-second shot from a quiet thriller. Night, an old basement storeroom. Steps on the floor above have set the only bulb swinging. CHARACTER is alone down here and must stop the light before its moving shadows give her away through the floorboards.

REFERENCES: @image1 is the opening frame: it sets the room, the bulb, the light, her clothes and the starting positions; the shot begins on it. @image2 is CHARACTER's character sheet: it controls her face, [your character's identity words: hair, face, marks, make-up, jewellery]. @image2 does not control the light, the background, the pose or the framing.

LOCKS:
ONE PERSON ONLY: CHARACTER, NEVER DUPLICATED. NOBODY ELSE IN FRAME; THE STEPS ABOVE ARE ONLY HEARD.
ONE BULB ONLY, AND IT IS THE ONLY LIGHT.
NO ON-SCREEN TEXT, NO SUBTITLES, NO LABELS OR LOGOS.
NOBODY SPEAKS. HER MOUTH STAYS CLOSED.
IDENTITY LOCK: RED ON HER RIGHT SIDE, BLACK ON HER LEFT, THE MARK ABOVE HER LIP ON HER RIGHT. FACE, HAIR AND TOP NEVER CHANGE.
ONE CONTINUOUS TAKE, NO CUTS.

COMPOSITION: 16:9, protected for a 2.39:1 crop. the character holds the right third. The bulb swings in the midground, parallel to the lens, from the left third to just short of her face.

CAMERA: 50 mm lens held for the whole shot, eye height, on a dolly. Already moving on the first frame: one slow continuous push-in from waist-up to a medium close-up, drifting slightly right to keep her on the right third, still moving on the last frame. Focus on her eyes.

ACTION:
0.0-1.0 s: the bulb swings from frame left towards her; its light rakes across her face; her eyes track it, head still. Dust sifts down from the floorboards.
1.0-2.0 s: it swings back to the left; she sinks into shadow, only the red side catching light. The steps above cross from left to right.
2.0-2.5 s: anticipation: she shifts her weight forward and her right hand rises.
2.5-3.0 s: as the bulb swings back to her she takes half a step and catches the black cord just above the socket with her right hand.
3.0-3.5 s: follow-through: the cord jerks, the bulb bobs twice and stops, held a hand's width from her right cheek. The shadows on the walls stop.
3.5-4.0 s: the steps above stop. She holds completely still, eyes lifting to the ceiling.
4.0-5.0 s: her eyes come down to the lens and hold. Dust drifts through the light.

ACTING: Goal: stop the light without a sound. Obstacle: the bulb is hot and the cord creaks. Fear held under control, then a cold calm as she looks at us.

LIGHT: The single bare clear incandescent bulb, warm and hard, is the only source. Its brightness never changes; only its position moves, so the shadows sweep across the brick, then stop when she catches it. At the end it lights the red side of her face from cheek height; the black side falls to near black. No fill, no beauty light, no light from nowhere.

LOOK AND FILM: Kodak Vision3 500T, 24 fps, 180 degree shutter: natural motion blur on the swinging bulb, halation around the filament, fine grain thickening in the shadows, real skin texture, no clean digital look.

AUDIO: NO MUSIC. Diegetic only: the cord creaking on its hook with each swing; the faint hum of the filament; slow heavy footsteps on the floorboards overhead that stop at 3.5 s; the cord snapping tight in her fist at 2.8 s; one slow exhale through her nose at 4.5 s. Nobody speaks.

NEGATIVE: music, speech, text, a second person, a second lamp, a window, flicker, sparks, a changing face, swapped hair colours, a cut, a zoom.
```

## Test 2 · A 12 s micro-film with four hard cuts

### S6-01 · Opening frame, 21:9, 2K, `@image1` = the sheet (8 credits)
Pass list we used: (1) the character reads at once: red side on frame left (her right), the mark above her lip on frame left, chains and ear cuffs; (2) her eyes look straight into the lens; (3) no mirror frame, no reflection, no second person or face anywhere; (4) the light is cold grey daylight with slat shadows, no warm sun; (5) the dome is small, out of focus, wordless; (6) no text, labels, logos or screens on any surface; (7) her hand and hair are plausible. Fail on any -> S6-01r. A second fail -> stop and review.
```
Reference 1 is @image1, her character sheet. It controls her identity only: her face, [your character's identity words: hair, face, marks, make-up, jewellery]. It does not control the light, the white wall, the pose or the framing. A 21:9 widescreen film frame from a Spanish black comedy set five years from now, 50 mm lens at her eye height. The camera stands exactly where her bathroom mirror is, so she looks straight into the lens as if into the mirror; the picture holds only her and the room behind her. A close-up from the chest up, her face just left of centre, the red side of her hair on frame left. A small, sterile, too-clean bathroom: seamless pale grey microcement walls, the white edge of a basin at the bottom of the frame, bare shelves, no towels, no personal objects. Behind her the open door shows a slice of a bare grey hallway, out of focus, and high on its ceiling a small black camera dome with one dim steady green dot. Cold, flat, overcast daylight through closed horizontal blinds on frame left is the only light: grey-blue, soft parallel slat shadows across the wall and the red side of her face, no warm tones anywhere. She studies her own face with cool attention, mouth closed, chin slightly lowered, her left hand tucking the black side of her hair behind her ear. She is alone. Kodak Vision3 250D, cool and desaturated, the red of her hair the only strong colour, fine grain thickening in the shadows, real skin texture with visible pores and freckles, unretouched, no clean digital look. She is a woman in her late twenties. No text, labels, logos, screens or signs anywhere.
```

Result: the whole face came back mirror-flipped (the red side on the wrong side). One retry (8 credits) with this line appended at the end:
```
Her red side is on frame left and her black side on frame right.
```

### S6-02 · Text With Reference, Seedance 2.0, 12 s, 21:9, 720p, voice on; `@image1` = the passing keyframe, `@image2` = the sheet (96 credits)
We changed one lock before clicking, because of the flipped keyframe: "RED ON HER RIGHT (FRAME LEFT IN SHOTS 1, 2, 4)". The text below went in as one line (the labels carry the structure):
```
SCENE CONTEXT: A 12-second black comedy in four shots, five years from now, in a sterile, too-clean flat. CHARACTER, alone, rehearses in her bathroom mirror, like an actress, a widow's face. The turn: the police arrive, and we see who she rehearses for, while the flat's ceiling camera watches her. OUTPUT: 4 shots, 12.0 s, hard cuts at 3.0, 6.0 and 8.5 s. 21:9 widescreen, 24 fps. REFERENCES: @image1 is the opening frame of SHOT 1: it sets the bathroom, the cold light, her clothes and her start position. @image2 is CHARACTER's character sheet: it controls her face, [your character's identity words: hair, face, marks, make-up, jewellery]; not the light, background, pose or framing. GEOMETRY: in SHOTS 1, 2 and 4 the camera is the mirror: she looks straight into the lens and the frame holds only her and the room behind her. SHOT 1, 0.0-3.0 s, CLOSE-UP, 50 mm, locked-off at eye height: she finishes tucking her hair; at 1.0 s she rehearses a shocked gasp, hand flat over her mouth, eyes far too wide, hammy; at 2.3 s she drops the hand, frowns at herself and resets. SHOT 2, 3.0-6.0 s, TIGHT CLOSE-UP, 85 mm, locked-off, same mirror: she leans closer and tries again: her eyes fill, her chin trembles, a breath catches. Better. At 5.3 s a tiny approving nod. SHOT 3, 6.0-8.5 s, WIDE, 24 mm, high in the hallway ceiling corner beside the small black camera dome, out of focus in the top-left foreground with its dim steady green dot; one slow push-in on a slider. Bare grey hallway, plain front door at the far end, CHARACTER small in the bathroom doorway on frame right. She freezes and turns her head to the front door to the sounds outside. SHOT 4, 8.5-12.0 s, CLOSE-UP, 85 mm, locked-off, the mirror again. 8.8 s: the doorbell. 8.8-9.6 s: one slow breath, eyes on herself. 9.6-10.4 s: her face drops into real grief, tears well. 10.4-11.2 s: CHARACTER says quietly, voice breaking, in the Spanish of Spain: «¿Cómo que muerto?» 11.2-11.8 s: the grief switches off into a tiny satisfied smile, lips closed. 11.8-12.0 s: she starts to turn away. LOCKS: ONE PERSON ONLY: CHARACTER, NEVER DUPLICATED; NO MIRROR FRAME, NO REFLECTION. DIALOGUE LOCK: THE ONLY WORDS ARE «¿Cómo que muerto?», ONCE, AT 10.4-11.2 s; HER GASP AND BREATHS ARE WORDLESS; NOBODY ELSE SPEAKS. IDENTITY LOCK: RED ON HER RIGHT (FRAME LEFT IN SHOTS 1, 2, 4), BLACK ON HER LEFT; FACE, HAIR AND TOP NEVER CHANGE ACROSS THE CUTS. NO TEXT, SCREENS, SIGNS OR LOGOS ANYWHERE. ACTING: Goal: a grief that will convince whoever is at the door. Obstacle: her real face is calm and they are already here. Tactic: an actor's small corrections, then a real memory for the tears. The comedy is the switch: grief on, grief off. LIGHT: cold flat overcast daylight through closed horizontal blinds is the only light, grey-blue, soft slat shadows, constant. The dome's green dot is tiny and steady. No fill, no beauty light. FILM: Kodak Vision3 250D, cool, desaturated, her red hair the only strong colour, 180 degree shutter, grain in the shadows, real skin with pores and tears. AUDIO: NO MUSIC. Diegetic only: faint ventilation hum; her breath and wordless gasp; from 6.3 s, outside, the soft electric whine of a vehicle gliding to a stop and a drone's thin whine descending to hover by the window; at 7.6 s a short synthetic three-note chirp; at 8.8 s a soft two-tone electronic doorbell; her line; then only the drone. NEGATIVE: music, other speech, radio voices, text, a second person, police, vehicles or drones in frame, warm sunlight.
```

Result in short: a usable rough cut (four shots, the Spanish line in sync, no music), cuts early, the tear close-ups not good enough to call it a finished piece. A test to learn from, not a result to copy.

## A template to start from (ours, generalised from the two above)

```
SCENE CONTEXT: <one or two sentences: where, when, who is alone, what must happen>
OUTPUT: <N> shots, <total> s, hard cuts at <t1>, <t2> s. <aspect>, 24 fps.
REFERENCES: @image1 is the opening frame of SHOT 1: it sets <room, light, clothes, start position>. @image2 is <NAME>'s character sheet: it controls <face, hair, marks, jewellery>; not the light, background, pose or framing.
LOCKS: ONE PERSON ONLY: <NAME>, NEVER DUPLICATED. ONE LIGHT SOURCE. NO TEXT, SIGNS OR LOGOS. IDENTITY LOCK: <which side is which, written both as "her right" and as "frame left">.
SHOT 1, 0.0-3.0 s, <WIDE|CLOSE-UP>, <lens> mm, <camera>: <what happens, with a time for each beat>.
SHOT 2, ...
ACTING: Goal / Obstacle / Tactic.
LIGHT: <the one source and what it does to each side of the face>.
FILM: <stock or look, shutter, grain>.
AUDIO: NO MUSIC. Diegetic only: <sounds with timestamps>. <The only words, in quotes, with their time.>
NEGATIVE: <what must not appear>.
```
