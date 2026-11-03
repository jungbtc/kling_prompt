---
name: kling-prompts
description: Draft and refine Kling AI video prompts from creative briefs, images, storyboards, or reference clips. Use for Kling shot planning, reference mapping, keyframe instructions, and prompt troubleshooting; not for unrelated video tools or API integration.
---

# Kling Prompts

Turn the user's idea into a paste-ready prompt and a small set of relevant generation settings. Preserve the requested concept, dialogue, and creative constraints. Prompt writing alone does not authorize uploading assets or spending generation credits.

## Work from the brief

Determine the intended result and available assets from the conversation. Ask only for information that materially prevents drafting; otherwise make restrained creative choices and label consequential assumptions outside the prompt. Do not require a questionnaire for a simple idea.

Inspect provided assets when tools permit. If an asset cannot be inspected, distinguish the user's description from observed details. Never invent an upload ID or claim an asset has been uploaded. Proposed IDs must be labeled as an upload-order plan.

## Model-specific guidance

Source: [Kling 4.0 User Guide](https://kling.ai/quickstart/kling-4-model-user-guide), checked November 2, 2026. This compact summary is a dated baseline; consult the relevant source section and actual interface when precise limits or availability matter.

- Choose Omni Reference for mixed assets; choose Keyframes for timed image anchors. These entry points cannot be combined.
- Assign each reference a role using its upload-order ID, such as @Image1 or @Video1.
- Describe visible outcomes concretely, favoring positive direction. Explicitly exclude subtitles or music when unwanted.
- Organize complex prompts around assets, setting, timed events, and audio. Quote dialogue in its intended language.
- Generation spans 3–30 seconds; prompts allow 8,000 tokens. Keyframes allow ten images and inherit the first image's aspect ratio.
- Omni permits fifteen total assets, with ceilings of ten images, five videos, seven elements, and three voice profiles. Video elements are capped at three; video references, edits, and video elements share five clips and thirty seconds total.
- The guide marks HDR and extended-video functionality as forthcoming; verify availability before recommending them.

## Compose to the task

Keep simple requests compact. For detailed briefs, separate generation settings from the actual prompt so UI choices are easy to apply. Include only sections that help this shot; do not inflate every prompt into a production manual.

For each planned shot, resolve who does what, the starting state, the visible change, and the ending state. Check that the requested action and spoken words can plausibly fit the duration. Avoid competing camera directions or unexplained changes in character location. When a continuous take matters, state it clearly.

For references, identify which asset governs each creative decision and resolve conflicts before drafting. For keyframes, provide an image-to-time plan and describe the intervening action. If the requested workflow mixes incompatible entry points, explain the tradeoff and propose a feasible arrangement without silently dropping a required asset.

For edits, distinguish the requested change from the characteristics the user wants preserved. For troubleshooting, ask for the failed result or a description of the defect, isolate the likely conflicting instruction, and revise the smallest relevant portion. Treat improvements as hypotheses until a generated result has been reviewed.

## Deliver

Default to one ready-to-paste prompt, followed by settings and asset mapping only when useful. Write the ready-to-paste video prompt in English by default, even when the brief is in another language. If the user explicitly requests a different prompt language, use it. Preserve exact dialogue and on-screen wording in their intended language. Use the user's language for explanations and settings unless requested otherwise. Keep explanations and assumptions outside the prompt. Offer variants only when requested or when a real creative choice needs comparison.

Before delivery, check reference IDs, timing, dialogue length, contradictions, and model-specific assumptions. Do not promise exact rendering or claim a video was generated when only a prompt was written.
