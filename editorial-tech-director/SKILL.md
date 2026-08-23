---
name: editorial-tech-director
description: Create manual-production packs for Chinese editorial technology explainers and hot-topic analysis videos, including narration, beat sheets, bilingual labels, image prompts, video prompts, subtitles, and editing notes.
---

# Editorial Tech Director

Turn a user-selected topic into a complete, file-based production pack. This skill plans the film; it does not call image, video, voice, music, or editing APIs.

## Defaults

- Horizontal 16:9 unless the user specifies another aspect ratio.
- No talking-head footage. Use concrete objects, screenshots, documents, interfaces, data, diagrams, and motion graphics.
- Each beat is about 10 seconds and is always split into two independently generated shots: `0-4s` introduction and `4-10s` depth.
- Provide two or three narrative directions first. Do not expand the full pack until the user selects one, unless they explicitly ask for a direct draft.
- Chinese creative explanations and narration; English image/video prompts.
- Use short English and Chinese in-frame labels when useful. Long Chinese narration subtitles are a post-production layer.
- Voice-over and music are completed later. Recommend only necessary sound effects.

## Workflow

1. Collect the topic, audience, target platform, approximate duration, factual constraints, and whether the user wants a neutral explanation or an opinion.
2. Offer 2-3 materially different narrative directions. Typical choices are object-decomposition, evidence-tracking, and judgment/impact analysis.
3. After selection, write a concise thesis and narration. Keep each 4-second segment near 12-18 Chinese characters and each 6-second segment near 24-32 characters, adjusting for natural pauses rather than forcing a count.
4. Build the beat sheet. Each beat must contain two independent shots, separate narration, subtitle timing, visual purpose, concrete visual elements, labels, transition, and sound effects.
5. Before writing any prompt, read [references/kimi-style-bible.md](references/kimi-style-bible.md). Treat it as a modular style system. Assign each beat a narrative job, choose one primary composition module, optionally one secondary module, and one motion module appropriate to the 4-second or 6-second role. Embed only the fixed DNA and selected modules into each standalone prompt; do not mechanically paste the same full composition into every shot. Do not put the source brand or reference creator name into generated prompts. Prompts must describe one concrete hero artifact and one narrative action, not a collection of generic icons. Preserve intentional subtitle-safe negative space while allowing meaningful secondary content.
6. Run a consistency pass: every visual element must explain, prove, or advance the narration; labels must be short; subtitles must fit the segment; no shot may rely on a generated long Chinese sentence.
7. Write the files described in [references/output-schema.md](references/output-schema.md) under the requested project directory. If no directory is provided, use `work/editorial-tech-director/<slug>/` and state the path. Every prompt section and every standalone file in `prompts/` must already contain the fixed DNA, selected composition/motion modules, content layer, and negative constraints; the user must be able to copy one prompt file without consulting another file or manually concatenating a prefix.

## Style grammar

Use the modular reference-derived grammar in [references/kimi-style-bible.md](references/kimi-style-bible.md). Keep the fixed DNA stable, but vary composition modules, hero media, window count, contrast, and motion according to the beat. Do not substitute a generic navy/blue server-room look or repeat one layout for every shot.

Keep the style layer separate from the content layer. The style layer supplies composition, palette, material, typography role, motion grammar, and negative constraints. The content layer supplies the topic-specific objects, facts, labels, and causal actions.

## Output behavior

Show a compact summary in chat, then create the complete file pack. Do not hide prompts or subtitle timings only in prose. Use UTF-8 text and stable filenames. The `.srt` file must use the full project timeline and include each subtitle cue's absolute time.
