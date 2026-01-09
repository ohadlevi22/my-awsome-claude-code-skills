# Style Index

Master catalog for Nano Banana prompt styles. Used for automatic style matching in Fast Mode.

## Quick Reference

| ID | Name | Keywords | Default Camera | Default Lighting | Best For |
|----|------|----------|----------------|------------------|----------|
| cinematic-drama | Cinematic Drama | hero, epic, powerful, movie, superhero, astronaut, action, poster, dramatic | 85mm low-angle | dramatic-shadows | Heroes, powerful moments, movie posters |
| soft-dreamy | Soft & Dreamy | family, kids, baby, warm, gentle, romantic, love, tender, sweet | 50mm eye-level | golden-hour | Family portraits, kids, romantic scenes |
| editorial-fashion | Editorial Fashion | fashion, magazine, professional, elegant, model, vogue, editorial, cover | 85mm f/1.4 | studio-clean | Professional shots, magazine quality |
| macro-miniature | Macro Miniature | tiny, miniature, giant, small, big world, scale, honey shrunk, ant | macro worm-eye | dramatic-cinematic | Creative scale play, surreal fun |
| fine-art-conceptual | Fine Art Conceptual | art, symbolic, gallery, conceptual, artistic, museum, meaning, abstract | 50mm neutral | studio-controlled | Artistic statements, symbolic imagery |
| street-art-mural | Street Art Mural | street, mural, graffiti, painted, urban, wall, banksy, texture | medium straight-on | golden-warm | Urban art, textured creative |
| fantasy-crossover | Fantasy Crossover | disney, pixar, animated, magical, cartoon, whimsical, fairy, enchanted | wide environmental | soft-magical | Real people in animated worlds |

## Matching Rules

### Priority Order
1. **Exact keyword match** - scene contains exact keyword from list
2. **Semantic match** - related concepts (e.g., "space" → astronaut → cinematic-drama)
3. **Subject type** - kids default to soft-dreamy, adults to cinematic-drama
4. **Fallback** - cinematic-drama (most versatile)

### Confidence Levels
- **High** (3+ keyword matches): "I'm thinking **{style}** style"
- **Medium** (1-2 matches): "This could work as **{style}**"
- **Low** (no matches): "I'll start with **Cinematic Drama** - want something different?"

## Style Files

Each style has a dedicated file with:
- Plain English description
- Key ingredients (camera, lighting, textures)
- Prompt template
- Full example prompts
- Default negative prompts

Files: `{style-id}.md` in this directory
