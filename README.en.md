# Miniature Landscape · 方寸山河

**Let a city rise from a map.**

[简体中文](README.md) · [MIT License](LICENSE) · [Examples & prompts](examples/README.md)

An Agent Skill for generating and editing miniature landscape images. Turn cities, mountains and landmarks into tactile little worlds: finely textured trees, miniature buildings, gentle water and printed roads connect naturally, as if photographed up close as a handcrafted model.

![Rio de Janeiro](examples/images/rio-de-janeiro.png)

## Selected examples

Nine creator-selected AI-generated examples. Click an image for the original PNG, or open its actual generation prompt. Hangzhou and Shenzhen use individually selected versions; the other seven were generated with a New York image as a style reference. See the [example notes](examples/README.md).

| | | |
| --- | --- | --- |
| [![阿勒泰 · Altay](examples/images/altay.png)](examples/images/altay.png) | [![旧金山 · San Francisco](examples/images/san-francisco.png)](examples/images/san-francisco.png) | [![悉尼 · Sydney](examples/images/sydney.png)](examples/images/sydney.png) |
| **阿勒泰 · Altay** · [Prompt](examples/prompts/altay.txt) | **旧金山 · San Francisco** · [Prompt](examples/prompts/san-francisco.txt) | **悉尼 · Sydney** · [Prompt](examples/prompts/sydney.txt) |
| [![里约热内卢 · Rio de Janeiro](examples/images/rio-de-janeiro.png)](examples/images/rio-de-janeiro.png) | [![上海 · Shanghai](examples/images/shanghai.png)](examples/images/shanghai.png) | [![巴黎 · Paris](examples/images/paris.png)](examples/images/paris.png) |
| **里约热内卢 · Rio de Janeiro** · [Prompt](examples/prompts/rio-de-janeiro.txt) | **上海 · Shanghai** · [Prompt](examples/prompts/shanghai.txt) | **巴黎 · Paris** · [Prompt](examples/prompts/paris.txt) |
| [![伦敦 · London](examples/images/london.png)](examples/images/london.png) | [![杭州 · Hangzhou](examples/images/hangzhou.png)](examples/images/hangzhou.png) | [![深圳 · Shenzhen](examples/images/shenzhen.png)](examples/images/shenzhen.png) |
| **伦敦 · London** · [Prompt](examples/prompts/london.txt) | **杭州 · Hangzhou** · [Prompt](examples/prompts/hangzhou.txt) | **深圳 · Shenzhen** · [Prompt](examples/prompts/shenzhen.txt) |

## What it does

- **A place becomes a miniature world.** Create cities, lakes, mountains, villages, gardens or imaginary landscapes.
- **Maps transition naturally into relief.** Printed roads become streets and coastlines become water edges, without a thick display base by default.
- **Materials and photography establish scale.** Flocked trees, painted buildings, carved rocks and macro depth of field give the scene a physical-model feel.
- **Follow a reference without copying its city.** Keep the chosen density, lighting and materials while preserving each place's spatial character.
- **Create a series or revise an existing image.** Request prompt-only output, change the aspect ratio, season, time of day or labels, or preserve a composition during an edit.

Defaults: a square image, vintage map paper, warm side lighting and one short place label. Explicit user instructions take priority. Dense city references do not have to become sparse toy scenes.

## Install in Codex

Use a Codex environment that supports Agent Skills. Actual rendering also requires an available image-generation/editing tool in that environment. This repository provides instructions and examples, not a standalone renderer, API key or dedicated model.

For a fresh installation:

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/carpediem67/miniature-landscape.git ~/.agents/skills/miniature-landscape
```

Start a new session and invoke `$miniature-landscape`. If the destination already exists, inspect that installation first; do not overwrite custom changes or install a duplicate. Alternatively, download the ZIP from [Releases](https://github.com/carpediem67/miniature-landscape/releases) and place the extracted skill folder in the same directory.

Other assistants supporting `SKILL.md` may load it according to their own conventions. Creative use has been tested in Codex; other hosts have not been individually tested. The skill prefers the host's built-in image tools, does not pin an image-model version and does not silently switch to a paid API.

## Start creating

```text
Use $miniature-landscape to create a miniature landscape of Paris.
```

```text
Use $miniature-landscape for autumn in Altay: lakes, conifers, golden birches and wooden houses, with visible map paper and no text.
```

```text
Use $miniature-landscape to create Shanghai, London and Sydney, one image each. Match the attached reference's materials, building density and depth of field.
```

```text
Use $miniature-landscape to edit this image: keep the landmarks and composition, change the light to early morning and add no buildings.
```

Requests can be in English or Chinese. Specify the label language, aspect ratio or style when desired. For text-only output, explicitly request “the prompt only; do not generate an image.”

## What makes it feel miniature

The effect goes beyond blurring an aerial photograph. Paper fibers, textured model trees, engraved building details, tiny boats and contact shadows create visible scale cues. Key landmarks remain readable while foreground and background soften naturally. Both dense cityscapes and open terrain can work; the place and the chosen reference guide the composition.

The concise skill instructions cover user-priority handling, reference-image roles, targeted geography checks, actual generation and visual review. Examples are optional references, not a mandatory image bundle to load on every invocation.

## Repository contents

| File | Purpose |
| --- | --- |
| [SKILL.md](SKILL.md) | Execution instructions and discovery metadata |
| [agents/openai.yaml](agents/openai.yaml) | Display name, summary and default invocation |
| [examples/](examples/README.md) | Nine selected images, actual prompts and style reference |
| [README.md](README.md) | Full Chinese documentation |
| [LICENSE](LICENSE) | MIT license |

## Scope and license

These are artistic miniatures with compressed distances and simplified architecture, not surveyed maps or editable 3D assets. Image generation is stochastic; examples illustrate a style, not a promise of pixel-identical reproduction.

The skill, documentation, prompts and bundled examples are released under the [MIT License](LICENSE). Retain the license and copyright notice when using, modifying or redistributing the material. Images are AI-generated; this license does not transfer third-party trademarks or other rights.

Created and maintained by [carpediem67](https://github.com/carpediem67). An independent community project, not an official OpenAI product.

