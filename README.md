<!-- DRAFT v6 (2026-11-03, no presenter identity), local only, not published. Proposed repo name: grawwww-studio/ep06-presenter-prompts (short, says what it is). Slots in {braces} are filled at publish time; the repo goes up (private at go-live, then public) only with the episode's «publica». -->
# How we made our new AI presenter: all the prompts, tests that didn't make the cut included

All people in these images are AI-generated and fictional.

Mae is our channel's character: her prompt and sheets are not shared; please don't use her likeness to pose as us.

The method, the prompts, the room pictures, the workflow and the credit ledger behind our video about making the channel's new AI presenter: her face and her room in Nano Banana Pro through PhotoGenerator.ai, what PhotoGenerator's Lip-Sync taught us, and how she talks every week with MiniMax H3 and the Pika H3 Flex adapter on our own computer.

- Video: https://youtu.be/5HPXjKsawMc

**Ad:** PhotoGenerator.ai gave us a free month of its Pro plan for this video, and more free months once it is published.
**Affiliate link:** if you subscribe through it, Grawwww earns a commission at no extra cost to you: https://www.photogenerator.ai/?ref=grawwww

## What is here
| Path | What it is |
|---|---|
| `presenter/` | How a face and its character sheets are built, with a demo person: a face prompt of the same structure and length as ours (`FACE_PROMPT.md`) and the sheet layout, prompt shape and outfit-sheet steps (`SHEET_TEMPLATE.md`). Our presenter's own prompt and sheets are not shared. |
| `room/` | The two room pictures (the streamer-webcam view and its edit without books) and the prompts that made them. |
| `h3/` | The ComfyUI graph we use for her weekly takes, as a JSON file only (`minimax-h3-pika-flex-api.json`), and `RECIPE.md`: three cameras, the short-outfit-text lesson and the numbers we measured. No model weights and no frames from H3. |
| `ledger.md` | Every PhotoGenerator.ai credit we spent for this episode, one line per try, failed ones included. The total in the video, {N} credits, is read in the app on {date}; `ledger.md` explains why it is a slot. |
| `prompts/` | The earlier tests that did not make the cut: a fictional influencer, phone-style photos, a podcast with lip-sync, a product ad, dance-trend tests and two short-film tests. |
| `NOTICE.md` | Licences, and what is not in this repository. |

Every picture carries a small AI tag in a margin strip, so it stays labelled if you share or download it.

## How to read it
- Prompts are in code blocks, exactly as typed before the click, except that the words that describe our presenter are replaced by the slot `[your character's identity words: hair, face, marks, make-up, jewellery]`. Where we only kept a summary of a prompt, the note says so. A short note under each says what went wrong, what we changed and what came out.
- Credit prices are what the app showed on the days we spent them; they may change.
- A prompt is a starting point. These tools change often, and we ran most shots once or twice.

## Using the pictures
Made with Nano Banana Pro via PhotoGenerator.ai; check Google's and PhotoGenerator's terms before using these images to train a model. Do not use them to imitate a real person.

## Credits
Powered by MiniMax H3 (the presenter's takes, made on our own computer under the MiniMax H3 Community License Agreement). Pika H3 Flex adapter by Pika, a Model Derivative of MiniMax H3, used under the MiniMax H3 Community License Agreement. Voice: a licensed library voice (AI-generated). Music: MiniMax-Music3 (AI-generated).

## Licences
Our text here is MIT (see `LICENSE`; `NOTICE.md` says exactly what that covers). No model weights and no logo files are in this repository. Not affiliated with Google, ByteDance, Kuaishou, Pika or MiniMax. Nano Banana Pro and Lip-Sync are used through PhotoGenerator.ai; MiniMax H3 and the Pika adapter run on our own computer. Independent affiliate of PhotoGenerator.ai, not an official representative.
