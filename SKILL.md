---
name: kling-prompts
description: Draft and refine Kling AI video prompts from creative briefs, images, storyboards, or reference clips. Use for Kling shot planning, reference mapping, keyframes, video edits, and prompt troubleshooting; not for unrelated video tools or API integration.
---

# Kling Prompts

Turn a creative brief into a clear, paste-ready Kling prompt and only the settings needed to use it. Preserve the user's concept, requested duration, dialogue, and creative constraints. Writing a prompt does not authorize uploading assets or spending credits.

## Start with the brief

Inspect supplied images or clips when possible. Distinguish what is visible from what the user wants to happen. For an image-to-video request, use the image's existing composition and details as the starting point unless the user asks to change them; describe the action that unfolds from that state. Don't invent unseen details as if they were observed.

Ask a question only when missing information prevents a useful draft. Otherwise make restrained choices; note consequential assumptions outside the prompt. Don't claim an asset was uploaded or a video was generated. Reference IDs are an upload-order plan, not actual upload IDs.

## Write the prompt

Write the ready-to-paste prompt in English by default, even if the brief is in another language. If the user explicitly requests another prompt language, use it. Keep dialogue and on-screen wording in their intended language, exactly as supplied. Use the user's language for explanations and settings unless requested otherwise.

Lead with the subject, setting, and visible action. Describe the starting state, what changes, and the ending state in an understandable sequence. Make details concrete: specify lighting, materials, framing, movement, and emotion through visible behavior rather than relying on abstract labels such as “premium” or a stack of adjectives. Describe how a transformation happens and what remains recognizable.

Match the detail to the idea. A simple action can be a short paragraph; use timed beats, asset roles, or separate audio instructions when they genuinely help control a more complex shot. Keep timing within the requested duration and allow actions and speech enough time. Avoid redundant instructions, overly precise invented timing, and competing camera or character directions. Add no unrequested plot, dialogue, music, characters, or elaborate effects.

Specify framing and camera behavior when relevant. For a static-camera request, keep the viewpoint and framing fixed throughout; subject or environmental movement can still occur. For a continuous take, state that explicitly and maintain spatial continuity. For multiple shots, identify the cuts or transitions and preserve screen direction and character positions where needed.

Favor positive descriptions of the desired result over long negative lists. Include “no subtitles” or “no background music” when the user doesn't want them. Use other exclusions sparingly when essential to the requested result. Do not assume silence or add sound solely because the guide supports audio. When audio is requested, describe relevant dialogue, ambience, effects, music, and timing; identify the speaker and quote dialogue verbatim. For on-screen text, give exact wording and useful placement or timing only when requested.

## Choose the workflow

Use the user's requested model or entry point when specified. Otherwise recommend only what fits the supplied assets and intended control:

- **Omni Reference:** Use for a concept or combined image, video, element, and voice references. State the role of each asset: what to borrow, what to preserve, and what to replace. Number references by their intended upload order, e.g. `@Image1` for scene composition and `@Video1` for motion and pacing. Do not imply a reference controls everything unless intended.
- **Keyframes:** Use for images that anchor the start, end, or specific moments. Map each image to its intended timestamp and describe the action and camera transition between anchors. The first keyframe determines the aspect ratio. Don't claim exact matching is guaranteed.
- **Video editing:** Clearly distinguish an edit from generation based on a reference. For an edit, use `Edit @Video1`, describe the precise change, and identify what should stay unchanged. For creative recreation, identify which qualities of the source to borrow and which subjects or settings to replace.

Omni Reference and the separate Keyframes entry point cannot be combined in a single task. If the request needs both, explain the tradeoff and propose a feasible arrangement without silently discarding an asset. The guide also describes keyframe-style generation through Omni; don't conflate that with using the separate Keyframes entry point alongside Omni references.

## Kling 4.0 reference

The [Kling 4.0 User Guide](https://kling.ai/quickstart/kling-4-model-user-guide), dated October 26, 2026, is the baseline, not a guarantee of current availability. Consult the guide and actual interface when exact limits or availability matter.

- Standard Kling 4.0: 3–30 seconds in one-second increments; up to 8,000 prompt tokens. The Keyframes entry supports up to 10 images.
- Omni: up to 15 total reference assets, including up to 10 images, 5 videos, 7 elements, and 3 voice profiles; at most 3 elements may be video elements. Reference videos, video edits, and video elements share a limit of 5 clips and 30 seconds total.
- Voice profiles are supported as audio references; describe desired music and sound effects in text rather than suggesting they can be uploaded as audio references.
- Flash has different limits and feature support. HDR and video extension were marked forthcoming in the guide. Verify current availability before recommending these capabilities or quoting precise limits.

## Refine and deliver

For troubleshooting, inspect the failed result or ask what went wrong. Identify the likely conflict—such as ambiguous asset roles, contradictory camera directions, or an unclear action—and revise the smallest useful portion. Treat the revision as a hypothesis until tested.

Deliver one prompt in a copyable block. Follow it with concise settings and reference mapping only when useful; label assumptions outside the prompt. Offer variants only when requested or a real creative choice requires comparison. Check asset numbering, timing, dialogue, camera continuity, and workflow compatibility before delivery. Never promise exact rendering.
