# Anki - English Grammar (Advanced)

Anki deck for learning English grammar, from English Grammar in Use (Advanced) – Activities.

500 cards in 23 decks. Live quiz: https://waldmann-dev.github.io/Anki-English-Grammar/

Structure mirrors Anki: each subdeck is a numbered folder, like in the Anki deck overview.

```
English Grammar/
  01. Tenses/
    00. What can I practise here/
      cards.tsv
    01. Present continuous and present simple 1/
      cards.tsv
    ...
  02. The future/
    ...
  03. Modals and semi-modals/
    ...
```

In Anki the decks are named:
- `English Grammar::01. Tenses::01. Present continuous and present simple 1`
- ...

## Card format

Fill-in-the-blank grammar exercises.

`cards.tsv` columns: `Question | Answer | Choices | Rubric | Audio | Image`

- Question: sentence with `{{c1::...}}` cloze + HTML. Front shows `___` for the cloze.
- Answer: the correct form(s). ` / ` = alternative correct forms.
- Choices: options (`;`-separated, two boxes separated by ` | `). `–` = no choice list.
- Rubric: exercise instruction.
- Audio: MP3 filename in `audio/` (correct sentence). `–` = no audio.
- Image: JPG filename in `images/` (exercise illustration). `–` = no image.

Import in Anki: File > Import, choose the .tsv, set separator to Tab, map fields to a Cloze note type with fields Question / Answer / Choices / Rubric / Audio / Image. Copy `audio/` + `images/` files into Anki's `collection.media` folder.

## How to add a lesson

1. Create folder `English Grammar/NN. Category/NN. Title/` (NN = 00, 01, 02, ...)
2. Add `cards.tsv` in the same format
3. Keep numbering, always `NN. Title`

## Source

Converted from the three .apkg decks (01. Tenses, 02. The future, 03. Modals and semi-modals). Media (480 MP3 + 40 JPG) preserved 1:1, no filename collisions.
