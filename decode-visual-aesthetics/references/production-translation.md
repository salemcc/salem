# Production Translation

Convert the visual DNA into a controllable production system.

## Deliverable stack

Create only the layers the user needs:

1. visual thesis;
2. fixed grammar and controlled variables;
3. reference-asset map;
4. keyframe brief;
5. still-generation prompt;
6. motion prompt;
7. model-specific prompt;
8. finishing notes;
9. test matrix.

## Reference-asset map

Give each asset one primary responsibility:

| Asset | Primary role | Must not control |
|---|---|---|
| character reference | identity, proportions, marks, costume or fur | lighting, composition, camera path |
| environment reference | layout, materials, geography | character identity or blocking |
| palette reference | hue relationships and saturation hierarchy | exact objects or composition |
| lighting reference | direction, softness, falloff, contrast | subject identity or scene design |
| composition reference | placement, scale, depth, negative space | color, character identity, story |
| texture reference | grain, edge, surface response | layout or motion |
| motion reference | camera path, speed, easing, subject cadence | characters, costume, setting, plot |

If one asset performs multiple roles, name those roles explicitly and note the risk of contamination.

## Keyframe-first workflow

Prefer:

1. lock character and environment;
2. generate the opening or representative keyframe;
3. compare it with the visual DNA;
4. correct composition, light, and material response;
5. animate only after the frame passes;
6. describe motion rather than restating the whole image.

Use text-to-video directly when the shot does not require identity, exact spatial continuity, or precise opening composition.

## Prompt architecture

Build prompts in this order:

1. format and duration;
2. subject identity and environment;
3. one dominant action;
4. visual-DNA rules;
5. framing, camera height, and probable focal behavior;
6. camera movement with speed and easing;
7. physical and material response;
8. sound or silence;
9. concise exclusions.

Use positive, observable outcomes. Avoid adjective piles.

### Still-keyframe template

> [format and medium]. [original subject and setting]. Preserve [identity references]. Use [palette relationship], [tonal curve], and [light geometry]. Compose with [placement, scale, negative space, depth layers]. Use [perspective and focus behavior]. Render [texture and material response]. The frame should create [emotional function]. Do not copy the reference's characters, exact setting, props, or signature composition.

### Motion template

> Begin from the approved keyframe. [subject] performs [one dominant action] from [start state] to [end state]. The camera [path] at [speed], [easing or stop behavior]. Secondary motion is limited to [environmental response]. Preserve screen direction, scale, lighting direction, and material continuity. No identity change, object teleportation, contradictory movement, or unmotivated camera drift.

## Seedance translation

When Seedance is requested:

- map each uploaded reference by name or UI label;
- state exactly what to borrow from each image or video;
- state what must not be copied from style and motion references;
- keep the motion instruction chronological;
- separate natural sound effects from music instructions;
- verify current official limits and syntax before claiming exact file counts, durations, or parameters;
- avoid invented API flags.

Example role mapping:

> `@图1` locks the original character only. `@图2` controls environment geography only. `@图3` contributes palette and lighting relationships only, not people or objects. `@视频1` contributes only camera trajectory, speed, and easing, not its subjects, setting, or shot content.

## Finishing notes

Specify relationships rather than brand-name LUTs:

- exposure and white-balance target;
- contrast curve and black-point behavior;
- highlight roll-off and bloom;
- palette compression or separation;
- local protection for skin, fur, paper, paint, or product color;
- grain, halation, sharpening, and vignette restraint;
- shot-matching order.

Treat generated clips as ordinary display-referred footage unless metadata proves otherwise. Do not mislabel them as log footage.

## Handoff to shot planning

When a downstream shot skill is available, pass:

- one-sentence aesthetic engine;
- fixed grammar;
- controlled variables;
- forbidden drift;
- character and environment continuity;
- reference-asset map;
- per-beat visual function;
- approved first-frame principles;
- sound and finishing constraints.

Let the shot skill determine shot count, timing, transitions, and shot-specific prompts.
