# 04 · "Can she do a dance trend?": the motion tests

What we tried to make the fictional character move like a viral dance. We never show the original creator's video or audio. The first tests turned a public trend clip into a grayscale depth video; the later ones used a dancer we generated ourselves. **The depth video is not in this repo** (it is derived from someone else's clip); the prompts are ours.

Short version of the results (the video has them): Motion Sync copied the motion well and leaked the reference's clothes and room into her; the depth-video route in Seedance kept her face but did not follow the body.

## Round 1: a depth video made from a public clip (not shared)

### M1 · Motion Sync, Kling 3.0 Omni (48 credits, 10 s, 9:16)
Character image = the main image of the character, reference video = the depth render (10 s maximum). Motion description:
```
The woman from the character image performs the same movement as the figure in the reference video, in a simple bright room, natural phone video look.
```

### V-R1 · Seedance 2.5, Text With Reference (280 credits at 10 s, then 140 at 5 s); references: the character's character, the sheet as `@image1`, the depth video as `@video1`
```
Reference 1 is the character and reference 2 is her character sheet: keep exactly her face, [your character's identity words: hair, face, marks, make-up, jewellery]. Reference 3 is a grayscale depth video used ONLY for the body movement and timing: copy how the figure sways, turns, raises both arms and then leans in close to the camera. Ignore the clothing, hairstyle and body shape of the figure in the depth video; never give her a skirt, a dress or a bun. A vertical TikTok filmed on a phone propped on a shelf in her bedroom in the evening, warm lamp light, unmade bed and clothes rail behind her, natural phone video quality, realistic motion, no motion blur on her face. She is a woman in her late twenties. No text, no logos.
```

### V-R2 · Same references, with a dress in the trend's colours (Seedance 2.5, 5 s, 140 credits)
```
[@Character] is the woman in this video and [@image1] is her character sheet: keep exactly her face, [your character's identity words: hair, face, marks, make-up, jewellery]. She wears a short black fitted dress with a full red tulle skirt, in a bold colour. [@video1] is a grayscale depth video used only for the body movement and timing: copy how the figure sways the skirt, turns, raises both arms and then leans in close to the camera. Her hair stays loose in the bob, never tied up. A vertical TikTok filmed on a phone propped on a shelf in her bedroom in the evening, warm lamp light, an unmade bed and a clothes rail behind her, natural phone video quality, realistic motion, no motion blur on her face. She is a woman in her late twenties. No text, no logos.
```

### V-R3 · The same references and text on Seedance 2.0, to see whether the model was the problem
No new text.

## Round 2: a reference dancer we generated ourselves (a fictional person)

### D0 · The reference dancer, 9:16, no reference (8 credits)
The first version, below, came back with a phone camera interface baked into the picture. The retry opened with "A vertical 9:16 photograph" and added a no-camera-interface line.
```
Vertical phone photo, full body, of a woman in her mid twenties with dark brown shoulder-length straight hair, wearing a plain heather-grey cotton tracksuit (a zip jacket zipped halfway over a white T-shirt, matching joggers) and plain white sneakers. She stands relaxed in the centre of the frame facing the camera, feet hip-width apart, arms loose at her sides and clear of her body, a small smile, ready to dance. The phone sits on a small tripod at waist height about three metres away, so her whole body fits from the top of her head to her shoes, with a little space above her head and below her feet. Behind her, a plain off-white wall and a light wooden floor in a small bedroom; soft daylight from a window off frame left, a faint shadow on the wall. Everyday phone-camera look, slight grain. She is a fictional woman in her mid twenties. No text, logos or brand marks anywhere.
```

### P0 · The dance on the spot, Frame to Video, Seedance 2.0, start frame = D0, 480p, voice off
We ran it at 5 s (20 credits) with the four steps stretched over 5 s. The written steps:
```
Locked-off phone shot on a tripod, full body, one continuous shot, the camera stays still. The woman dances on the spot at a moderate tempo, one move per second:
0-1 s: she steps her right foot out to the side and points her right index finger straight at the camera, left hand on her hip.
1-2 s: she bounces her knees and rolls both shoulders back twice.
2-3 s: she sweeps both arms up over her head and claps once above her head.
3-4 s: she drops both hands to her hips, pushes her right hip out, tilts her head and holds the pose with a small laugh.
Same outfit and hair throughout. No text, no music.
```

### D1 · the character full body with the same framing as D0, 9:16, sheet as `@image1` (8 credits)
```
Reference 1 is @image1, her character sheet: keep her face, [your character's identity words: hair, face, marks, make-up, jewellery] exactly as shown. A 9:16 vertical full-body phone photo: the phone sits on a small tripod at waist height about three metres away, so she fits from the top of her head to her white sneakers, with a little space above her head and below her feet. She stands in the centre of the frame facing the camera, feet hip-width apart, arms loose at her sides and clear of her body, a small smile, about to start a dance. She wears a fitted black long-sleeve top, black straight-leg joggers and plain white sneakers. Behind her, a plain off-white wall in her small bedroom and a light wooden floor, the corner of an unmade bed at the right edge and a clothes rail at the left edge, both cut by the frame. Soft daylight from a window off frame left, a faint shadow on the wall. An everyday phone photo, slight grain. She is a woman in her late twenties. No text, logos or brand marks anywhere.
```

### MS1 · Motion Sync, Kling 3.0 Omni, Standard, 9:16, 5 s (24 credits): character = D1, reference = the P0 clip
Motion Sync refused the 480p clip ("reference video resolution is too low"); we upscaled our own clip locally to 720p and ran it again (the first, refused job was refunded). Scene description:
```
A woman in her late twenties dances on the spot in her small bedroom, filmed on a phone on a tripod, full body, one continuous shot, the camera stays still. Soft daylight from a window on the left. Same outfit and hair throughout.
```

