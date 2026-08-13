---
name: video-production-router
description: Classify and lock a video request as AI generation, designed composition, supplied-footage editing, or a mixed end-to-end workflow before production begins.
---

# Video Production Router

Read the brief before any production work. Capture its audience, platform, duration, language, aspect ratio, supplied media, visible copy, and export target.

## Choose the dominant line

- **Generate** for new model-generated footage or imagery.
- **Compose** for explainers, designed HTML/SVG scenes, kinetic type, charts, captions, title cards, overlays, or motion graphics. Prefer this for explainer and animation work.
- **Edit** for supplied footage that must be selected, cut, cleaned, reframed, captioned, mixed, localized, or changed. A bounded semantic pixel edit remains an Edit job.
- **AUTO** only when multiple lines must be woven into one deliverable.

Classify supplied references as `reproduce`, `edit`, or `guide`. State one primary line and any supporting lines. Do not silently change the primary line after locking it.

Use 1920×1080 for 16:9, 1080×1920 for 9:16, and 1080×1080 for 1:1 unless the brief requires another canvas.

## Produce the routing result

Return the chosen line, reason, reference relationship, target format, timed outline, supplied and missing assets, optional provider-backed operations, review gates, and final playback checks.

Confirm before overwriting source media, destructive edits, paid provider calls, or publishing. If the runtime is unavailable, return a complete unexecuted production package and label it planned rather than rendered.

## Example

For “Turn this interview into a 45-second vertical clip, remove pauses, add captions and an animated title,” lock **Edit** as primary and **Compose** as supporting on a 1080×1920 canvas.

**Source and inspiration:** [OrkasVideoStudio `video-router`](https://github.com/Orkas-AI/Orkas-VideoStudio/blob/7387d99d468e0cce22508854ba8bca04e79657e1/packages/skills/video-router/SKILL.md), adapted under MIT.
