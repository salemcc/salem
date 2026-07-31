---
name: decode-visual-aesthetics
description: Analyze film, animation, photography, painting, illustration, advertising, or other visual references to extract transferable aesthetic logic and convert it into an original visual DNA, style bible, reference pack, keyframe brief, or AI-video prompt system. Use when the user asks to reverse-engineer a masterwork or admired visual style; study color, tonal range, lighting, composition, lens and perspective, depth, texture, blocking, camera movement, motion design, or editing rhythm; compare multiple references; reduce an AI-generated look; create an account-wide visual language; or translate references into prompts for Seedance, Kling, Veo, Runway, image generators, or a downstream storyboard workflow. Learn mechanisms without reproducing protected characters, signature scenes, or exact shot sequences.
---

# Decode Visual Aesthetics

Turn admired references into a reusable visual system. Treat aesthetic similarity as a hypothesis to test, not as permission to duplicate a finished work.

## Route the task

Choose only the modes the user needs:

1. **Reference analysis** — inspect one or more images, clips, films, animations, photographs, or artworks.
2. **Visual DNA extraction** — identify recurring rules rather than isolated decorative details.
3. **Style comparison** — distinguish shared mechanisms and meaningful differences across references.
4. **Style bible creation** — define fixed rules, controlled variables, and prohibited drift.
5. **Production translation** — map the visual DNA to reference assets, keyframes, prompts, camera directions, and post-production notes.
6. **Evaluation** — score whether generated work preserves the logic while remaining original.

Read the relevant references before working:

- Read [visual-dna-framework.md](references/visual-dna-framework.md) for every reference-analysis or visual-DNA task.
- Read [source-specific-analysis.md](references/source-specific-analysis.md) when the source includes live-action film, animation, photography, painting, illustration, or mixed media.
- Read [production-translation.md](references/production-translation.md) when the user wants prompts, a style bible, a reference pack, keyframes, model-specific guidance, or video production output.
- Read [originality-and-evaluation.md](references/originality-and-evaluation.md) when the user asks to replicate, emulate, reproduce, borrow, or closely match a work, or when scoring generated results.

## Gather evidence

Use the user's supplied files and descriptions first.

- For a single image, analyze only visible spatial and surface evidence. Label motion, editing, lens, and production-process claims as hypotheses.
- For an image set, compare at least three distinct compositions before declaring a recurring rule.
- For a video, inspect representative frames at shot boundaries and moments of meaningful camera, blocking, lighting, or palette change. Prefer 8–16 useful frames over uniform oversampling.
- For a named public work or URL requiring current evidence, retrieve accessible public sources. Separate observed facts, informed estimates, and unavailable information.
- If the source cannot be inspected, ask for 3–8 representative frames or one short clip when exact analysis matters. Do not fabricate visual evidence from memory.

Record uncertainty explicitly. Never present an estimated focal length, lighting ratio, film stock, color pipeline, frame rate, or production method as confirmed unless supported by reliable evidence.

## Derive the visual logic

Analyze the source across these layers:

1. color system;
2. tonal structure;
3. lighting geometry;
4. composition and negative space;
5. lens, perspective, and camera height;
6. depth and focus hierarchy;
7. texture, edge behavior, and material response;
8. subject blocking and scale relationships;
9. camera-motion grammar;
10. subject and environmental motion;
11. editing rhythm and transition logic;
12. emotional or narrative function.

Distinguish:

- **surface traits** — immediately visible colors, grain, props, or decorative motifs;
- **structural rules** — repeated relationships between light, space, subject, movement, and emotion;
- **production mechanisms** — choices that could plausibly create those relationships;
- **uncertain inferences** — claims requiring more evidence.

Promote a feature to visual DNA only when it repeats across independent examples or clearly organizes the whole image. Treat a one-off feature as a local choice.

## Explain why the style works

Do not stop at labels. For every major rule, connect:

> observable choice → perceptual effect → emotional function → transferable production instruction

Example:

> Large cool negative space around a small warm subject → immediate figure-ground separation → vulnerability and isolation → preserve a 3:1 empty-to-subject area and keep the subject as the only warm accent.

Avoid vague conclusions such as “cinematic,” “premium,” “dreamy,” or “masterful” unless converted into observable instructions.

## Build an original system

Separate the output into:

- **fixed grammar** — rules that should remain stable across the user's project;
- **controlled variables** — elements that may change by scene or episode;
- **forbidden drift** — combinations that would break the intended identity;
- **originality changes** — subject, setting, narrative function, visual motif, or staging changes that create independent expression.

Do not use an artist or title name as the final prompt. Translate the reference into attributes and relationships. Preserve the mechanism, not the protected expression.

## Translate to production

When generation output is requested, deliver only what is needed from the following:

1. reference-asset map with one responsibility per asset;
2. still-keyframe prompt;
3. image-to-video motion prompt;
4. model-specific master prompt;
5. continuity header reused across shots;
6. color-grading and finishing notes;
7. A/B test changing one aesthetic variable at a time.

Keep identity references, style references, composition references, and motion references separate. State what each reference may influence and what it must not copy.

If the user requests a complete 8–12 shot production plan and `direct-ai-video-shots` is available, finish the aesthetic brief first, then pass the fixed grammar, reference map, continuity rules, and forbidden drift into that skill. Do not duplicate its shot-planning workflow here.

For model-specific limits or syntax that may change, verify current official documentation before stating exact capabilities. Do not invent parameter syntax.

## Default deliverable

Use the user's language and content maturity. Unless a narrower format is requested, provide:

1. **One-sentence aesthetic engine**
2. **Evidence and confidence**
3. **Visual DNA table** — observed pattern, effect, function, production instruction, confidence
4. **Hidden organizing logic**
5. **Fixed grammar / controlled variables / forbidden drift**
6. **Originality distance** — what to retain and what to redesign
7. **Production translation** — reference roles and prompt architecture
8. **Evaluation plan**

Use approximate palette swatches or hex values only as practical guides; note that display transforms, compression, and source grading can change sampled values.

## Quality gate

Before delivering, verify:

- evidence is separated from inference;
- recurring rules are not confused with one-off details;
- every aesthetic label becomes an observable production instruction;
- color, light, composition, optics, texture, and motion form one coherent system;
- static sources do not generate unsupported motion claims;
- the output preserves originality distance from recognizable expression;
- model-specific prompts assign one clear role to each reference;
- the result gives the user a direct next production step.
