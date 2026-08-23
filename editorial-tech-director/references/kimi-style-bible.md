# Kimi K3 Reference Style Bible

This is the modular style system extracted from the supplied reference video. Read it before writing prompts. Keep a small fixed DNA across the film, then choose composition and motion modules according to the beat's narrative function. Do not use the entire library as a fixed prefix on every shot.

## Style identity

Use a minimal multimodal product-demonstration montage: a clean pale gallery or studio canvas presents one concrete artifact at a time. The artifact can switch medium from screen recording to hand drawing, game footage, hardware, data dashboard, editorial poster, or physical desk object. A consistent presentation frame, spacing, UI chrome, and typography make the sequence feel like one product showcase.

## Locked visual grammar

- Horizontal 16:9 composition with a pale gray, white, or very light warm-gray presentation canvas.
- One dominant concrete demo artifact per shot, usually a rounded-rectangle screen/card/window with generous margins; do not fill the whole frame with abstract graphics.
- Rounded corners, soft cast shadow, thin clean edges, restrained physical depth; presentation-board / floating-window feeling.
- Sparse black or charcoal sans-serif typography, large isolated headings or short labels, generous tracking and clear hierarchy.
- Kimi-blue interaction accent: vivid electric/cobalt blue used for a small arc, progress ring, cursor trace, button halo, status pulse, or one key highlight. Use it sparingly, not as a full blue wash.
- Minimal product UI chrome when appropriate: a white rounded input/search bar near the lower area, a black circular action button, and a small blue arc or ring around that button. Keep chrome sparse and functional.
- Real artifact first, annotation second: the viewer should recognize the object or screen before seeing labels, tags, or diagram overlays.
- Editorial juxtaposition: a physical sheet, tool, screenshot, card, or interface can sit inside the same clean canvas; use controlled layering, slight tilt, crop, and depth.
- Preserve deliberate media switching: sketch, photographic/game image, hardware, data visualization, typewriter/editorial layout, and dark UI can each appear as the content artifact while the surrounding presentation grammar stays consistent.
- Motion is smooth and purposeful: slow reveal, clean slide-in, cursor/scan, card lift, subtle zoom, screen swap, blue pulse, and precise settle. This is a polished product demo, not a holographic sci-fi trailer.

## Fixed DNA (use in every prompt)

```text
Minimal multimodal product-demonstration montage derived from the supplied reference video, horizontal 16:9, pale gray or white presentation canvas, real artifact first, sparse black or charcoal sans-serif information layer, generous breathing room, restrained physical depth, polished product-showcase finish.
```

## Composition modules

Choose one primary module per shot and optionally one secondary module:

### Hero window

```text
One concrete hero artifact inside a clean rounded-rectangle floating window, large margins, thin precise edge, soft cast shadow, one isolated cobalt-blue interaction accent, clear focal hierarchy.
```

### Floating artifact

```text
Present the artifact as a slightly tilted floating card on the pale canvas, with visible surrounding space and one or two clipped supporting materials; let the artifact's medium remain recognizable.
```

### Interface chrome

```text
Add sparse functional UI chrome only: a white rounded input or search bar near the lower edge, a black circular action button, and a small cobalt-blue arc, cursor trace, or status halo; keep the controls secondary to the main artifact.
```

### Split comparison

```text
Use two balanced rounded windows with a clean vertical separation, one concrete subject on each side, sparse black comparison labels, and one thin cobalt-blue linking line; keep the difference readable before adding annotations.
```

### Process sequence

```text
Arrange three concrete rounded cards or windows in a left-to-right sequence, each showing a real document, screen, or object; use a single thin connector path and one cobalt-blue pulse that travels through the sequence.
```

### Scale expansion

```text
Show a small concrete card or window expanding into a larger set of repeated but meaningful windows or physical modules, with increasing scale expressed through spacing and count rather than icon repetition; reserve clear margins around the growth.
```

### Dark inset

```text
Place one dark charcoal content window inside the pale presentation canvas, with sparse white or gray information marks and one cobalt-blue status trace; keep the dark area contained and the surrounding canvas visible.
```

### Panorama system

```text
Use a wider pale presentation canvas with several rounded content windows at different depths, connected by one restrained cobalt-blue path; reveal the whole system only after the viewer recognizes the individual components.
```

## Motion modules

Choose one motion module matching the shot's role:

```text
4-second hook: reveal the hero window or floating artifact with a slow controlled push-in or clean slide, trigger one precise cobalt-blue pulse, then hold briefly for the hook to register.
```

```text
6-second comparison: reveal the two sides in sequence, let the comparison line or shared data path appear, then settle on the contrast; keep movement lateral and precise.
```

```text
6-second process: move three concrete cards one at a time through the connector path, let the cobalt-blue pulse travel with the active step, and finish with all stages visible.
```

```text
Scale beat: expand meaningful physical modules in controlled stages, increase density once, then pause on the new scale; avoid infinite cloning.
```

```text
Dark computation: use a restrained scan, cursor pass, or parameter refresh inside the dark window, with one cobalt-blue status response and no camera shake.
```

```text
Final payoff: begin close on the decisive artifact, pull back smoothly to reveal its supporting system, let one cobalt-blue path connect the real components, and hold the final composition for the last second.
```

## Prompt assembly rule

Every standalone prompt embeds the fixed DNA, the selected composition module, the content layer, and the negative constraints. Video prompts additionally embed the selected motion module. Adjacent beats should vary their primary module unless continuity is the intended effect.

## Mandatory image prompt block

Use this older full block only when the selected shot genuinely needs a full floating-window treatment; otherwise use Fixed DNA plus the selected module:

```text
Minimal multimodal product-demonstration montage derived from the supplied reference video, horizontal 16:9, pale gray or white presentation canvas, one concrete hero artifact presented inside a clean rounded-rectangle window or floating card, generous margins, soft cast shadow, thin precise edges, sparse black charcoal sans-serif typography, minimal functional UI chrome, a white rounded input/search bar and a black circular action button with a small vivid cobalt-blue arc or halo when UI chrome is present, real artifact first and annotations second, editorial media juxtaposition, restrained physical depth, smooth premium product-showcase composition.
```

## Mandatory video motion block

Use the following as a baseline only; replace the generic motion phrase with the selected motion module when the beat calls for comparison, process, scale, dark inset, or payoff motion:

```text
Smooth reference-derived product-demo motion: clean card/window reveal, controlled slide or subtle push-in, precise cursor/scan or object action, one restrained cobalt-blue pulse, gentle parallax, and a clean settle. Preserve the hero artifact and the presentation frame; do not turn it into a holographic sci-fi scene.
```

## Mandatory negative block

```text
Avoid generic cyberpunk, neon-blue full-frame lighting, holograms, floating icon grids, particle clouds, lens flares, excessive HUD overlays, dense dashboard clutter, arbitrary gradients, glossy sci-fi 3D, chaotic camera shake, liquid morphing, and large blocks of generated Chinese text. Do not force every artifact into the same navy-blue palette. Do not copy source-brand logos, product names, or exact UI text unless the user supplies them.
```

## Quality gate

A prompt fails if it has no concrete hero artifact, no pale presentation canvas, no sparse black information layer, or no meaningful relationship between the selected module and the narration. It also fails if adjacent shots mechanically repeat the same composition or if it reads like a generic server-room or cyberpunk poster.
