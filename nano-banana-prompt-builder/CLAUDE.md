# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Claude Code skill** (not a runnable codebase) for building professional image generation prompts for Nano Banana (Google Gemini 2.5 Flash Image). The skill guides users through an interactive Q&A to craft prompts using photography and cinematography terminology.

## Repository Structure

```
nano-banana-prompt-builder/
├── SKILL.md              # Main skill definition (entry point)
├── INSTALL.md            # Installation instructions
└── library/              # Pattern library referenced by the skill
    ├── styles/           # Style templates with examples
    │   ├── _index.md     # Style catalog for keyword matching
    │   └── *.md          # Individual style definitions
    ├── ingredients/      # Building blocks
    │   ├── cameras.md    # Lens & angle guide
    │   ├── lighting.md   # Lighting moods
    │   └── negatives.md  # What to avoid
    └── examples/
        └── user-favorites.md  # Curated successful prompts
```

## Key Concepts

- **SKILL.md** is the main entry point that Claude reads when the skill is invoked
- **library/** contains reference material that the skill reads when building prompts
- **Fast Mode**: Auto-matches style from keywords, generates prompt instantly
- **Pro Mode**: Step-by-step Q&A guiding user through style, lighting, camera, and special elements

## Available Styles

Seven style templates: Cinematic Drama (default), Soft & Dreamy, Editorial Fashion, Macro Miniature, Fine Art Conceptual, Street Art Mural, Fantasy Crossover.

Each style in `library/styles/` includes: prompt template, default camera/lighting, keyword triggers, and example prompts.

## Modifying the Skill

When editing:
- Update `SKILL.md` for workflow/behavior changes
- Update `library/styles/*.md` for style-specific template changes
- Update `library/styles/_index.md` when adding/modifying style keywords
- Update `library/ingredients/*.md` for camera/lighting/negative reference changes

## No Build System

This is a documentation-only project. No commands to run - changes take effect immediately when the skill is loaded.
