# Pipeline

```
 idea  ->  Claude  ->  ChatGPT  ->  Higgsfield  ->  post
         (scene +    (still in     (motion)
          prompts)    the scene)
```

## 1. Reference sheet (once)

Generate the 6-panel character sheet in ChatGPT: front, side and back full body, plus front, three-quarter and profile headshots on a plain gray backdrop. This sheet is attached to every future image request. See `prompts/01-image-chatgpt.md`.

## 2. Scene (per video)

Claude gets the character bible and returns one scene: setting, action, camera, caption. See `prompts/02-scenes-claude.md`.

## 3. Still (per video)

ChatGPT gets the reference sheet plus the scene, and renders the first frame. Check it against the consistency checklist in `CHARACTER.md`. Regenerate until it passes.

## 4. Motion (per video)

The approved still goes into Higgsfield with the motion prompt from step 2. Keep clips short; long clips are where the face starts to drift. See `prompts/03-video-higgsfield.md`.

## 5. Post

Caption from Claude, lowercase, one line. Post, then rotate to a completely different setting for the next clip.

## Lessons

- Face drift is the biggest risk. Always attach the reference sheet, never describe her from memory.
- Settings should change more than you think is necessary. Novelty drives views, recognition drives follows.
- Action beats posing. The clips that moved (sparring, parkour, flexing) outperformed the static ones by a wide margin.
