# AIGC Film Studio

A standalone Codex skill for developing an idea into an actionable, reviewable AI-generated film.

It connects story development, screenwriting, directing, performance design, visual assets, shot planning, generation tasks, and finishing. It supports episodic shorts, narrative short videos, and standalone short films in photoreal, 2D anime, stylized 3D, limited-animation, hand-drawn, and mixed-media forms.

[中文](README.md) · [Skill instructions](SKILL.md) · [Worked example](examples/returning-the-key.md) · [Sources](SOURCES.md) · [MIT](LICENSE)

## Approach

Start with what the character wants, what prevents it, what they try, and what changes. Carry that event through performance, staging, camera placement, sound, and editing. Adapt the design to the visual form and the tools actually available. Judge the resulting media rather than treating a well-written prompt as a finished performance.

Enter at the stage the user needs. Existing footage can be reviewed directly; an existing script need not be rewritten before shot planning. The skill does not force every project through a fixed package of documents or a prescribed number of acts, twists, or shots.

The skill instructions and detailed references are currently written in Chinese. The agent should follow the user's chosen language for deliverables.

## Execution requirements

This repository contains instructions, references, reusable templates, and an original worked example. It does not include generation engines, models, API credentials, credits, or an editing application.

With text-only capabilities, it produces creative work and production handoffs. With suitable host tools and user authorization, it can coordinate image, video, audio, and finishing tasks. Installation alone does not provide these tool capabilities.

Prompt-only requests remain prompt-only. Existing generation authorization is respected without repeatedly asking the same question; substantial scope or cost changes are handled explicitly. Task success, inspected media, edit usability, and final review are reported separately.

## Install in Codex

The repository root is the skill folder. Download or clone the repository, or extract its release archive, and place the complete `aigc-film-studio` directory under your Codex skills directory:

```text
~/.codex/skills/aigc-film-studio/SKILL.md
```

The default Windows location is `%USERPROFILE%\.codex\skills\aigc-film-studio`. Use your configured skills location if you customized the Codex home directory. Reload skills through your host and invoke `$aigc-film-studio`. Back up local edits before replacing an existing installation.

No other skill or media provider is required. `agents/openai.yaml` supplies Codex UI metadata. Other agents supporting `SKILL.md` may use the instructions, but their compatibility must be tested separately.

## Example requests

```text
Use $aigc-film-studio to develop my idea into an approximately 60-second
photoreal AI short. Deliver the story and script first. Do not generate media.
```

```text
Use $aigc-film-studio to turn this accepted script into 2D anime shots.
Preserve the plot and dialogue; specify staging, shot purpose, and continuity.
```

```text
Use $aigc-film-studio to review these three clips for edit continuity.
Only evaluate what you can actually inspect. Do not modify or regenerate them.
```

## Sources and contributions

The repository uses original wording to connect general dramatic craft with selected ideas discussed in Sidney Lumet's Making Movies, Steven D. Katz's Film Directing Shot by Shot, and Judith Weston's Directing Actors. Its AIGC workflow is a contemporary adaptation, not a method jointly authored or endorsed by those writers. See [SOURCES.md](SOURCES.md).

Contribute realistic requests, observed failures, and focused improvements. Keep private materials and credentials out of contributions. Behavioral scenarios in `evaluations/scenarios.md` are intended for fresh-context checks, not exact wording tests.

Original repository content is available under the [MIT License](LICENSE). No book files, book illustrations, tutorial transcripts, or models are distributed here. Third-party materials and services retain their own terms.
