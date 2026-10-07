---
name: music-player-photo-weave
description: Transform a supplied full-body fashion or lifestyle photograph into a music-player collage with a clear square portrait window, frosted controls and selective person/hand/bag occlusion. Use for music UI photo compositions with customizable song and artist text.
---

# Music Player Photo Weave

Make the supplied photograph interact with an enlarged iPhone-like music panel. The defining feature is selective front/back weaving, not a complete person cutout pasted over a rectangle. Read [references/composition.md](references/composition.md) before production.

## Fresh-chat reference loading

Before production, read [fresh-chat visual contract](references/fresh-chat-visual-contract.md), inspect the bundled visual reference. For a generative preview, pass it together with the new user source to the image-generation call; for deterministic production, follow the bundled composition/script route and preserve source pixels. Do not assume earlier chat images are visible to the generator. Use this package as the style source; treat custom fields and occlusion choices as per-photo inputs.

## Inputs and source selection
Use the user's raw photo as the identity and scene source. Treat any finished reference only as composition guidance, not a source for its person, props, words or background. Prefer a full-body image with an unobstructed head, naturally separated arm or hand-held bag, visible shoes and enough scene around the subject. Explain an unsuitable photo rather than inventing a pose, limb or bag. If asked to find a test source, record its URL and photographer when known; label external images as test material rather than cleared publication assets.

Before generating a preview, collect the song title and artist from the user. If either is missing, ask only for the missing fields and wait for the answer; for example: “播放器里要放哪首歌？请告诉我歌名和歌手。” Do not generate with placeholder labels, invent an artist, or silently choose music. If both are already supplied in the conversation, use them directly without asking again. Placeholder text or an agent-selected song is allowed only when the user explicitly requests it. Preserve the supplied title and artist exactly and place them on separate lines. These are per-image inputs, not fixed Skill defaults.

User may also set playback state, progress, panel scale and output ratio. Defaults: portrait source ratio, pause icon, restrained native white controls. Avoid extra notices, chat bubbles, captions, AirDrop panels, decorative objects or phone hardware.

## Workflow
1. After song and artist are supplied, write a source-specific layer plan identifying the window, frosted area and which source parts will be in front. Choose panel dimensions so the clear window contains the upper body and the controls overlap hips/thighs, leaving lower legs visible.
2. Produce one preview using available image generation or compositing. Use supplied raw photo and composition reference in separately stated roles. Keep face, clothes, pose, bag and scene. The clear rounded square reveals sharp original imagery; lower controls obscure original detail with scene-derived blur and translucency.
3. Inspect the actual output against the checks below. Distinguish visual identity resemblance from verified unchanged source pixels. A generated edit is an aesthetic preview unless source fidelity is separately verified.
4. When user requests staged review, deliver this one image and stop. Do not expand variants, other styles, video or distribution package until this checkpoint passes. Apply feedback narrowly, then retest on another photo when authorized.

For source-locked production, preserve original background and person pixels through masking/compositing; render editable UI and exact text separately. Blur a duplicate of the underlying photo for the frosted region. Restore only designated foreground head/arm/hand/bag areas. Do not restore the entire person's legs over the controls. If masks or tooling are unavailable, state that the result remains a preview.

## Review checklist
- Original photo remains full bleed and recognizable; no fabricated pose or props.
- Panel reads as one integrated music player: outer rounded frame, near-square clear window, continuous lower frosted area.
- Head or a suitable arm crosses the window frame; another suitable hand/bag crosses onto lower controls.
- Body behind the lower panel is softly visible as color, not sharp trousers on top of buttons.
- Legs below the panel remain photographic and sharp.
- Frost tint derives from the photo, with subtle edges; no opaque plastic plate or uniformly transparent empty box.
- Song and artist are separately customizable, text legible; any occlusion comes from foreground masking, not deleted characters.
- Playback/progress/volume controls have consistent weight, spacing and native proportions.
- No unrelated UI, fake phone shell, huge title, sticker border or added glass-refraction effects.

Deliver source, preview and brief review findings. Do not call the Skill aesthetically approved merely because structural validation passes.

## Author and public reference

Created and maintained by **理智画** (GitHub: [liuzihe849-png](https://github.com/liuzihe849-png)). Inspect [the original sample](assets/reference-original.png) and read [sample scope and limitations](references/public-sample.md). The sample is a visual aid, not a user identity or proof of exact fidelity. Do not copy sample-specific defects into new outputs.
