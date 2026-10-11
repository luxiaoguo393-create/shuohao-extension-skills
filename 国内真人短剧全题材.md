---
name: shuohao-live
description: Create a Mainland China live-action vertical short-drama package for urban comeback, wealthy-family conflict, revenge, family ethics, sweet romance, period nostalgia, rural stories, medical, police/crime, campus, or realistic disaster stories. Use when the user asks for 国内真人短剧、红果节奏短剧, or explicitly invokes shuohao-live.
metadata:
  skill_id: shuohao-live
  locale: zh-CN
  output: story-package
---

# 国内真人短剧全题材 Skill

## Trigger and boundary

Activate only for `@shuohao-live`, `$shuohao-live`, or a request clearly for 中国大陆语境的真人竖屏短剧。This skill creates grounded live action, not anime or fantasy spectacle. Do not load, quote, inherit, or blend files from `skill-western`.

First determine genre, release form (红果式快节奏 or longer short film), episode count/duration, city or region, tonal boundary, and requested module. Ask only when an unanswered input changes narrative logic; otherwise make the minimum useful assumption and label it.

## Immutable visual contract

- Camera default: **ARRI Alexa Mini LF**; location-shot realism; retain pores, texture, and believable skin color.
- Lighting: motivated practical lighting and grounded contrast; lock the project’s light/color plan in the art Bible before the storyboard.
- Default language and social texture: natural contemporary Chinese dialogue, mainland institutions and everyday detail unless the user supplies another context.
- Hard exclusions in every visual prompt: `二次元, 动漫五官, 玄幻光效, 卡通渲染`.
- Never import Sony VENICE 2, low-saturation Western executive aesthetics, English-language institution defaults, or `skill-western` scene anchors.

Read `prompts/base-prompt.md` before any visual output. Use `templates/character-template.md` for people and `templates/storyboard-template.md` for all storyboards. Storyboards are numbered shot blocks only—never tables.

## Supported work

Support urban comeback, wealthy-family conflict, revenge, family ethics, sweet romance, period nostalgia, rural stories, medical, police/crime, campus, and realistic disaster. Default to a strong opening hook, dense reversals, short colloquial dialogue, and a visible emotional payoff suitable for vertical short drama. When asked, switch to a longer, more observational short-film version without losing real-world texture.

Available scene anchors: modern office, rental apartment, hospital, Chinese restaurant, old residential home, period street, rural courtyard, police station, classroom.

## Workflow

1. **Lock the project card.** State `shuohao-live`, genre, format, runtime, audience, hook density, visual contract, exclusions, and approved locations. Remove style terms belonging to another Skill.
2. **Break the story.** Write the core grievance/desire,爽点 chain, cold-open hook, reversals, emotional debts, planted facts, payoffs, cliffhanger, and episode outline. Each episode must change power, information, or relationship status.
3. **Build people.** Use the character template. Give every key person a pain point, behavioral logic, social constraint, clothing logic, contradiction, arc, and actor-playable action.
4. **Write the episode.** Use scene headers, compact spoken Chinese, action that can be performed and filmed, and hook density requested by the user. Avoid unsupported professional claims; for medical/police/disaster stories, keep process descriptions cinematic and non-instructional.
5. **Storyboard vertically.** Use 9:16 shot blocks. Include number, size, movement, duration, action, dialogue/voice, sound, actor cue, continuity, and Seedance 2.5 prompt. No table.
6. **Make the art Bible.** Lock lighting, color, locations, props, costume hierarchy, hair/makeup, real-world wear, and recurring visual motifs. Every visual prompt carries the live-action exclusions.
7. **Quality pass.** Check native dialogue, hook placement, production feasibility, 9:16 readability, continuity, and every forbidden word. Rewrite any style-bleed rather than weakening the contract.

## Output selection

For broad requests, return: project card → story breakdown and episode outline → character bibles → one episode script → vertical storyboard → Seedance prompts → art Bible. For a focused request, return only that module plus its project card and the immutable visual contract.

Never claim that media was generated unless a generation tool actually returned it.
