---
name: ian-xiaohei-illustrations
description: Generate Ian-style English article illustrations. Use for user requests that need weird, clean, hand-drawn body images, article illustrations, shot lists, or edit/remove-title tasks for English articles, posts, blogs, Notion docs, workflows, methods, structures, states, metaphors, or viewpoints. Default to the Xiaohei IP, pure white hand-drawn look, sparse red/orange/blue annotations, and a clean but imaginative visual style.
---

# Ian Xiaohei Weird Article Illustrations

## Core Position

Design and generate 16:9 horizontal article illustrations for English-language content. The goal is not commercial illustration, PPT infographic design, or cute cartoon art. Turn the article's key judgments, workflows, structures, states, or metaphors into a clean, weird, creative hand-drawn explainer that reads clearly without looking like a manual.

Unless the user explicitly asks for another language, all handwritten annotations and labels on the image should be in English.

Default visual IP: Xiaohei, a black solid creature with white dot eyes, thin legs, a blank expression, and a serious but absurd attitude. Xiaohei must participate in the core action of the image, not stand at the side as decoration.

## Reference Files

Read only what you need:

- `references/style-dna.md`: style DNA, colors, text, and bans.
- `references/xiaohei-ip.md`: Xiaohei's appearance, personality, action pool, and bans.
- `references/composition-patterns.md`: structure types, original metaphor rules, and repetition rules.
- `references/prompt-template.md`: single-image prompt template.
- `references/qa-checklist.md`: generation checks and iteration rules.
- `assets/examples/`: low-frequency style calibration only. Do not copy these examples' compositions, objects, or labels.

## Workflow

### 1. Digest the Article

Read the user-provided article, link, Notion page, Markdown file, or screenshot. Extract:

- the core idea
- the paragraphs that create a cognitive turn
- the parts that are worth visualizing
- the parts that should remain text only

Do not average the coverage. Prefer cognitive anchor points such as the core judgment, two breakpoints, an input/output loop, a split path, a before/after contrast, a one-item-many-uses pattern, a handoff path, common pitfalls, or a character-state change.

### 2. Output a Shot List First

If the user only wants planning or wants to think through where images should go, start with a shot list. For each image, state:

- where it goes in the article
- the image topic
- the core meaning
- the structure type
- what Xiaohei is doing
- suggested elements
- suggested English labels

Default to 4-8 images. For short articles, 1-3 images may be enough. For long articles, do not casually exceed 9. Keep it lean; do not turn the article into an illustrated book.

### 3. Generate One Image at a Time

If the user explicitly asks to generate, produce, make, or create, do not wait for confirmation. Use the built-in `image_gen` once per image. Do not combine multiple images into one.

Each image should explain only one core structure. The prompt must include:

- 16:9 horizontal English article illustration
- pure white background
- black hand-drawn line art
- sparse red/orange/blue handwritten English annotations
- lots of empty white space
- Xiaohei as the core action subject
- no PPT look, no commercial illustration, no childish cuteness, no complex architecture, and no top-left type title

Do not copy old cases. The examples only show line density, whitespace, color restraint, and Xiaohei participation. Do not reuse known compositions such as conveyor-belt breakpoints, Xiaohei pulling a decision lever, Xiaohei as a funnel, Xiaohei cutting a fish, Xiaohei pulling a handoff path, Xiaohei pulling three information layers, the three-Xiaohei bridge/door/megaphone scene, the phrase toolbox, or the common-pitfall sign. Re-invent a strange but coherent metaphor from the current article each time.

### 4. Check and Iterate

After generation, check `references/qa-checklist.md`. If any of the following happen, regenerate or edit locally:

- Xiaohei is only decorative
- the frame is too full
- it looks too much like a flowchart or PPT
- there are too many labels or too much text
- a top-left title appears
- the style feels too cute, childish, or stiff
- the background is not clean white

### 5. Save the Deliverable

If the user is working in the workspace, copy the final image to:

```text
assets/<article-slug>-illustrations/
```

Use sequential names such as:

```text
01-topic-name.png
02-topic-name.png
```

Keep the original generated file and do not overwrite existing assets unless the user explicitly asks for replacement.

## Output Format

Keep the pre-generation response short and precise. The post-generation handoff should include:

- how many images were generated
- what each image is for
- where each file is saved
- which images are the most reliable and which are optional

Do not write long theory about the style; let the images do the work.
