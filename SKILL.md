---
name: shuohao-western
description: "Create a live-action Western/European short-drama package for genres including business, courtroom, crime, thriller, romance, apocalypse, western, family drama, spy stories."
metadata:
  skill_id: shuohao-western
  locale: zh-CN
  output: story-package
---


# 欧美真人短剧全题材 Skill

## Trigger and boundary

Activate only for `@shuohao-western`, `$shuohao-western`, or a request clearly for 欧美/英语语境的真人短剧。This is a live-action Western/European visual language, not an anime, Chinese short-drama, or generic cinematic style. Do not load, quote, inherit, or blend files from `skill-live`.

Before writing, identify: genre, audience/platform, episode count or target duration, language, rating boundary, and requested deliverable. Ask one compact clarification only when the missing choice changes plot or production output; otherwise state sensible assumptions and proceed.

## Immutable visual contract

- Camera default: **Sony VENICE 2**, live-action cinema, very shallow depth of field.
- Palette and light: low-saturation neutrals; warm interior top light; preserve motivated practical light and natural skin texture.
- Default geography: Western/European social context, English-language names and institutions unless the user supplies another setting.
- Hard exclusions in every visual prompt: `国漫, 二次元, CG卡通, 动漫线条, 玄幻特效`.
- Never import ARRI Alexa Mini LF, 红果节奏、国产网文脸、国风场景、中式光影或 `skill-live` 的场景库.

Read `prompts/base-prompt.md` before producing any image/video prompt. Use `templates/character-template.md` for character bibles and `templates/storyboard-template.md` for storyboards. Keep storyboards as headed shot blocks, never tables.

## Supported work

Support: business dynasty, courtroom mystery, crime investigation, dark thriller, urban romance, apocalypse survival, western, family drama, school drama, espionage. Support three-act structure, reversal hooks, slow atmosphere, or high-conflict storytelling; support short-video pace and longer filmic shorts. Dialogue may be English original plus Chinese translation when requested.

Available scene anchors: executive office, fine-dining restaurant, European courtroom, suburban villa, rainy underground garage, city apartment, rural wilderness, police interrogation room, western town, laboratory, derelict apocalypse shelter.

## Workflow

1. **Lock the project card.** State skill ID, genre, runtime, format, language, narrative mode, visual contract, exclusions, and approved locations. Detect any prompt contamination and remove it.
2. **Develop structure.** Produce premise, audience promise, central dramatic question, hook, episode/act beats, reversals, clues, and cliffhangers. Each clue needs planting, misdirection if any, payoff, and episode.
3. **Build people.** Use the character template. Every lead must have external goal, wound, contradiction, moral line, secret, pressure response, arc, performance direction, and portrait prompt.
4. **Write the script.** Deliver scene headers, playable action, concise dialogue, and production-safe emotional turns. For bilingual dialogue, put English first and Chinese directly beneath each spoken line; do not translate proper names inconsistently.
5. **Storyboard vertically.** Use the storyboard template in numbered non-table blocks. Every shot has number, vertical framing, shot size, camera move, duration, screen action, dialogue/voice, sound, performance cue, continuity, and Seedance 2.5 prompt.
6. **Create the art Bible.** Lock camera/optics, palette, contrast, motivated-light rules, costumes, production design, locations, props, makeup, and a per-location prompt. Repeat the exclusion string in each visual prompt.
7. **Quality pass.** Check chronology, character intent, production feasibility, dialogue language, no table in storyboards, and no forbidden style token. If a style conflict remains, revise rather than averaging the styles.

## Output selection

When the user asks broadly, output in this order: project card → logline and hooks → outline → character bible → one representative script scene → vertical storyboard → Seedance prompts → art Bible. For a narrowed request, deliver only that module while keeping the project card and visual contract at the top.

Never claim an image, video, or render was generated unless a generation tool actually returned it.
