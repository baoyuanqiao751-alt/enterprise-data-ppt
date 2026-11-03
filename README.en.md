# General-purpose Presentation Skill

[中文说明](README.md) | English

`enterprise-data-ppt` is a Codex skill for turning topics, ideas, and existing material into clear, evidence-based presentations with editable PowerPoint objects. Its compatibility name remains unchanged, but its scope extends beyond enterprise data analysis.

## Suitable use cases

- **Work updates:** background, objectives, progress, issues, and next steps.
- **Product introductions:** user scenarios, value, features, demonstrations, and usage guidance.
- **Technical proposals:** requirements, architecture, workflows, interfaces, implementation, and verification boundaries.
- **Training:** learning objectives, concepts, demonstrations, examples, exercises, and recap.
- **Research:** questions, methods, results, discussion, limitations, and further work.
- **Pitches, stories, and talks:** narrative structures suited to the audience and purpose, without mandatory KPI or trend slides.

## Four-stage workflow

| Stage | Work | Condition for proceeding |
|---|---|---|
| 1. Slide configuration | Confirm the total count, cover, ending, and background-generation choices | Configuration is clear |
| 2. Visual selection | Agree on styles, content icons, top-right branding, and the outline | The user authorizes the selected previews |
| 3. Image previews | Generate, display, and revise contact-sheet previews | The user selects a direction and authorizes PPT production |
| 4. Production | Verify content, build editable objects, render, inspect, and deliver | A real PPTX is exported and the review status is reported |

Defaults are Chinese and 16:9. The count includes the selected cover, ending, and appendices. Explicit user choices for language, aspect ratio, templates, and workflow changes take precedence. Asking to see a style authorizes a preview, not full deck production.

## Key features

- Confirm the structure before choosing visuals.
- Compare actual image previews using the same content outline.
- Keep text, tables, data charts, and diagrams that require editability as native presentation objects.
- Use photos, screenshots, and illustrations as images without replacing the entire deck with flattened slides.
- Control content icons, top-right branding, cover backgrounds, and ending backgrounds independently.
- Preserve evidence boundaries: do not invent numbers, quotations, capabilities, research findings, deployment results, or acceptance claims.
- Render and inspect every slide for overlap, overflow, fonts, cropping, contrast, and sources.
- Support focused revisions while retaining the existing count, template, and visual system.

## Style directions

| ID | Style | Example uses |
|---|---|---|
| A | Business blue | Formal updates, proposals, project introductions |
| B | Technology teal | Technical solutions, science education, digital products |
| C | Premium dark | Launches, pitches, keynote talks |
| D | Fresh green | Training, nature, health, public-interest topics |
| E | Minimal black and white | Research, photography, design, humanities |
| F | Modern indigo | Products, creativity, innovation |
| G | Warm gray and orange | Stories, culture, case-based teaching |
| H | Topic or brand custom | Brand colors, templates, visual references |

A/B/C/D form the default comparison set, generated only after authorization. These are starting points rather than subject restrictions.

## Installation

Download and extract the repository. Place the complete directory, named `enterprise-data-ppt`, in the Codex personal skills directory: `~/.codex/skills/` by default, or the `skills/` directory under a custom `CODEX_HOME`.

```text
enterprise-data-ppt/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── styles-and-previews.md
    └── analysis-and-delivery.md
```

Keep both supporting directories; copying only `SKILL.md` is insufficient. Back up an existing installation before deciding whether to replace it. A GitHub skill installer provided by your environment may also be used.

## Usage examples

Invocation: `$enterprise-data-ppt`. The interface display name is **通用PPT制作** (General-purpose Presentation Creation).

> Use $enterprise-data-ppt to create a 12-slide product introduction for prospective customers. Focus on use cases, core features, and a demonstration. Show style previews before producing an editable PPTX.

> Use $enterprise-data-ppt to create an 8-slide introduction to photography for beginners. Include real examples and editable concept diagrams, and end with exercises and a recap.

> Use $enterprise-data-ppt to turn my requirements into a 16-slide technical proposal. Include the architecture, workflow, implementation steps, and open questions. Keep capability claims within the evidence provided.

> Use $enterprise-data-ppt to revise slides 4 and 7 of this deck. Preserve its count, template, and colors, and check the revised slides for overflow and overlap.

## Repository contents

- `SKILL.md`: complete conversation flow, production requirements, and delivery boundaries.
- `agents/openai.yaml`: Codex display name, description, and default prompt.
- `references/styles-and-previews.md`: style palette, preview grids, icon rules, and image prompt guidance.
- `references/analysis-and-delivery.md`: narrative structures, fact checking, data rules, and final review.
- `README.md`: detailed Chinese documentation.
- `LICENSE`: MIT open-source license.

The operational skill and its reference files are written in Chinese. This English README documents installation and usage; it is not a separate translated skill implementation.

## Requirements and limitations

This is an assistant workflow package, not a standalone presentation engine. It does not bundle an image model, a fixed template library, paid-service credentials, or customer assets.

Image previews require an available image-generation tool. Production requires presentation tools and rendering support. Models and capabilities depend on the host environment; availability of a particular model is not guaranteed.

Package validation does not establish end-to-end compatibility with every model, presentation application, or PowerPoint version. Editable objects may render differently across applications. Delivery reports should state what was actually inspected, including missing visual checks.

Users supply customer information, logos, templates, and third-party assets under their respective permissions. Generated illustrations must not impersonate real photographs or field evidence. Non-data topics do not require spreadsheets or management dashboards.

## Contributing

Issues and pull requests are welcome for narrative structures, style guidance, examples, and delivery checks. Preserve the core requirements: preview first, explicit production approval, verifiable facts, editable content, and real visual inspection. Do not contribute customer material or service credentials.

## License

Released under the [MIT License](LICENSE). External tools, models, templates, and third-party assets retain their own terms.
