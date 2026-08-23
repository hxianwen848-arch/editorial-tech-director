# Output Schema

Create one project directory per request. Use a lowercase ASCII slug for the directory and filenames; Chinese content remains inside UTF-8 text files.

## Required files

### `00-project-overview.md`

Include topic, thesis, audience, aspect ratio, target duration, selected narrative direction, style summary, assumptions, and factual caveats.

### `01-narration.md`

Include the full Chinese narration in timeline order. Mark every beat and its `0-4s` / `4-10s` segments. Include approximate delivery duration and pause notes.

### `02-beat-sheet.md`

Use one section per beat with:

- absolute time range and beat duration;
- introduction and depth purpose;
- narration for each sub-shot;
- subtitle text and absolute subtitle timing;
- concrete visual subject and action;
- in-frame English labels and Chinese labels;
- shot transition and necessary sound effects;
- the corresponding prompt filenames.

### `03-shot-prompts.md`

Provide the prompts in execution order. For every sub-shot include a `Nano Banana image prompt` and an `Omni video prompt`. Keep the two prompts independent because the two clips are generated independently. State the intended duration (`4s` or `6s`) and the continuity cue used at the edit point.

### `04-subtitles.srt`

Use standard SRT numbering and `HH:MM:SS,mmm --> HH:MM:SS,mmm` timestamps. Keep cues within their parent shot. Prefer one or two lines; split long depth narration into sequential cues. Do not duplicate in-frame labels as narration subtitles unless they are intentionally spoken.

### `05-editing-notes.md`

Include assembly order, hard-cut or transition recommendation at each 4-second boundary, subtitle placement, safe-area guidance, label treatment, sound-effect timing, and a final QA checklist.

## Optional files

Create `prompts/` when the prompt pack is large. Store one UTF-8 `.txt` per independently generated shot using names such as `beat-01-intro-image.txt`, `beat-01-intro-video.txt`, `beat-01-depth-image.txt`, and `beat-01-depth-video.txt`. Each file must be standalone and include the fixed DNA, selected composition/motion modules, content layer, and negative constraints. Do not paste the entire module library into every file, and never make the user concatenate a style prefix manually. Keep these files identical to the corresponding complete sections in `03-shot-prompts.md`.

Create `06-facts-and-sources.md` when the topic is a current event, scientific claim, statistic, or contested issue. Separate verified facts from interpretation and flag claims that require user confirmation.

## Timing rules

- A 4-second intro subtitle normally contains 12-18 Chinese characters.
- A 6-second depth segment normally contains 24-32 Chinese characters, split into 1-3 cues when needed.
- Leave a small lead-in and tail-out inside each shot; do not place subtitle cues outside the shot boundaries.
- The two sub-shots of a beat are separate generation units and may use different compositions, but they must share one causal idea and one visual continuity cue.
