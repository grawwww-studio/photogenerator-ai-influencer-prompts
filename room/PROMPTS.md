# The room

Both pictures are Image Generator, `nano-banana-pro`, 16:9, 2K, JPEG, one image, 8 credits. We kept a written summary of each prompt, not its full text, so these are what each prompt asked for, in the order of the prompt.

## BG1 (failed) and BG2: a streamer's webcam view of an empty room
The first prompt (about 2,150 characters) asked for a real unretouched photo from a streamer's webcam, with no one in it:
- an empty black office chair about 90 cm from the lens, a little left of centre;
- the desk edge along the bottom, a mic arm with a broadcast mic in the right foreground;
- a dark teal-black wall, a walnut bookshelf with worn books and a pothos, a peach and teal abstract print, a pleated floor lamp lit;
- a soft LED panel as key light from the left, a wide-angle webcam look at f/2, lived-in;
- no people, no text, no logos, no RGB lights, no laptop.

It named a video platform and a camera brand. The generation failed on the provider's side after 8-13 minutes and the credits came back. We took the three brand names out (about 2,130 characters) and it worked: that is BG2, `BG2_room.jpg`.

What BG2 got wrong: the LED panel was in the frame and blown out, and a cyan glow sat on the wall behind the chair.

## BG3: the edit without books
Image Generator, BG2 as the reference image, about 1,040 characters. Books were a problem for us because their spines turn into fake lettering in video. The prompt asked to keep the room, camera, chair, desk, mic, lamp, print, pothos, light and grain exactly, and to change only:
- shelves holding objects without text (ceramics, plants, a basket, plain boxes, folded linen) instead of books;
- the desk notes become one closed plain notebook;
- no cyan glow; the LED panel out of frame;
- no text anywhere.

Result: `BG3_room_no_books.jpg`. The room, framing and objects held; the shelves hold vases, bowls, a plant, a basket and boxes.

## A second camera angle (BG4): a miss
We asked the same model for the same room from 1.5 m to the left, about 35 degrees off the chair's front. The camera did not move: the model kept the composition and changed objects instead (a second desk appeared). We did not keep the picture. The 8 credits are in `ledger.md`.
