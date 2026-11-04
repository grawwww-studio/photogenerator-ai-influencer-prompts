# Character sheet template and the outfit sheets

This is the method we used for our presenter. Her sheets and prompts are not shared; see the note in `FACE_PROMPT.md`. The sheet names below are our working names.

## Layout we settled on
One 16:9 picture on flat mid-grey, three photographs of the same person side by side, white gutters between them:
1. full body, front, neutral stance (attitude only in this panel);
2. exact side profile of head and shoulders;
3. a large frontal face close-up, the right-most panel at full height.

We first tried four panels and a different layout for every sheet. A fixed three-panel layout held the face much better, so after the third sheet every prompt said: `same 3-panel layout, light and face`, and the previous sheet went in as the one reference image.

## Prompt shape for an outfit sheet
```
Same three photographs, same layout, light, face, poses and flat mid-grey background as the reference image. Change only the clothes: [garments]. [Accessories]. No glasses, no hat, no bag, no logos, text, numbers or prints.
```
Image Generator, `nano-banana-pro`, 16:9, 2K, 1 image, previous sheet as `@image1`, 8 credits each.

## The sheets, in order (what we typed, as we logged it)
We kept a summary of each prompt, not the full text, so these are descriptions of what each prompt asked for.

| sheet | the ask | outcome |
|---|---|---|
| S1 | four panels, oversized washed-black cropped tee, very baggy charcoal cargo, striped tie as belt, headphones round the neck | failed on the provider's side, refunded |
| S1b | the same prompt again | face held; stiff stance, tie read as school uniform, headphones removed after |
| S2 | natural everyday slouch, cropped charcoal tee, extremely wide black cargo, thin chains, small bag | closer; no bags after this |
| S3 | the fixed three-panel layout, thin glasses | format held; flat look |
| S4 | white ribbed crop tank, open oversized black track jacket, very baggy light-wash jeans, chunky mesh runners, chains, hoops, thin oval glasses | style landed; a facial mark rendered like a stud |
| S5 | oversized off-white hoodie, black cargo with tight ankle cuffs, no glasses | not what we wanted |
| S6 | all black: cropped hoodie, hood down, wide balloon cargo, elastic ankle cuffs, chunky trainers, layered silver chains | the one we liked |
| S7 | the S6 sheet as reference; trousers cream and lower on the hips with a plain black band showing; hoodie a little shorter, raw hem, thick drawstrings, long bunched sleeves | the one we use |

## How the working sheet was derived, with no AI
The S7 sheet from the app had her profile face smaller than the sheet we had tested the video model on (25.2 % of the sheet height against 38.3 %). We **re-cropped** the original picture: the profile panel became a window of the original, magnified about 1.13x with Lanczos resampling and placed where the earlier sheet had it. No generation, no face fix, no retouching. The face close-up panel was already within 10 % and stayed as it was.

Our first grey sheet was also made without AI from the app's 4K output: an area downscale to 2304x1152 and replicated grey columns at the sides, white gutters kept.

## Character text next to the sheet
The video model also gets a three-line text (who is on the sheet, what stays fixed, what the skin and fabric look like). The identity words (as in the demo `FACE_PROMPT.md`) go in it unchanged; only the garment nouns change per sheet.
