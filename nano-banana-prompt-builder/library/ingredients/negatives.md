# Negative Prompts Guide

What to AVOID in your images - organized by style and common issues.

## Why Negative Prompts Matter

Nano Banana responds well to explicit "don't do this" instructions. Negative prompts help:
- Avoid common AI image artifacts
- Prevent style drift
- Eliminate unwanted elements
- Maintain realism where needed

---

## Universal Negatives (Use Almost Always)

### Quality Issues
```
blurry, low resolution, pixelated, grainy, noisy,
out of focus, motion blur, compression artifacts,
low quality, amateur, snapshot
```

### Anatomy Problems
```
distorted hands, extra fingers, missing fingers,
malformed limbs, unnatural pose, broken anatomy,
crossed eyes, asymmetrical face, uncanny valley
```

### Unwanted Elements
```
watermark, signature, text overlay, logo,
border, frame, vignette (unless intended),
multiple subjects (unless intended)
```

---

## Style-Specific Negatives

### Cinematic Drama
```
soft lighting, flat lighting, high angle looking down,
passport photo, ID photo, mundane, boring composition,
centered static pose, awkward pose, stiff posture,
fake looking, plastic skin, cartoon, anime, illustration
```

### Soft & Dreamy
```
harsh shadows, high contrast, dramatic lighting,
dark mood, cold blue tones, stark white light,
flash photography look, stiff posed expressions,
fake smiles, awkward positioning, sharp harsh background,
busy distracting elements, over-saturated colors,
artificial looking, plastic skin
```

### Editorial Fashion
```
harsh unflattering shadows, under-eye circles emphasized,
amateur lighting, on-camera flash, red eye,
busy distracting background, cluttered environment,
awkward pose, uncomfortable expression, stiff posture,
over-retouched plastic skin, uncanny valley
```

### Macro Miniature
```
toy, plastic, diorama, miniature model, dollhouse,
fake, cartoon, tilt-shift effect, obvious photoshop,
floating without shadows, no contact shadow,
unrealistic scale, anime, illustration,
smooth plastic texture, toy-like proportions
```

### Fine Art Conceptual
```
fantasy creatures, childish style, heavy busy textures,
cluttered background, over-saturated colors,
cartoonish elements, obvious digital effects,
stock photo feeling, generic composition,
unintentional elements, horror aesthetic,
disturbing imagery, creepy uncanny elements,
low artistic value, snapshot quality, casual composition
```

### Street Art Mural
```
photographic skin texture, smooth airbrushed finish,
glossy paint, wet looking surface, digital art style,
clean perfect wall, new construction, pristine surface,
floating elements without shadows, obvious photoshop,
unrealistic integration, paint bleeding onto real objects,
blurry textures, low resolution wall detail
```

### Fantasy Crossover
```
costume, cosplay, parody, mockery, obvious photoshop,
pasted in, floating, not integrated, harsh edges,
person looks animated/cartoonish, uncanny valley,
scary creatures, horror elements, dark disturbing mood,
cheap party decorations, fake looking props,
low quality compositing, mismatched lighting
```

---

## By Problem You Want to Avoid

### "Looks Fake / AI-Generated"
```
artificial looking, obviously AI generated,
uncanny valley, plastic skin, wax figure,
over-processed, over-smoothed, airbrushed,
digital artifacts, glitchy, morphed
```

### "Too Cartoonish"
```
cartoon, anime, illustration, drawing,
stylized, cel-shaded, comic book style,
3D render, CGI looking, video game graphics
```

### "Wrong Scale / Proportions"
```
wrong proportions, miniature looking, toy-like,
diorama, tilt-shift, unrealistic scale,
giant head, tiny body, distorted perspective
```

### "Bad Lighting"
```
flat lighting, harsh shadows, unflattering light,
overexposed, underexposed, blown highlights,
crushed blacks, on-camera flash, red eye
```

### "Cluttered / Messy"
```
busy background, cluttered, messy, chaotic,
too many elements, distracting, confusing composition,
visual noise, no focal point
```

### "Wrong Mood"
```
(for happy scenes): dark, moody, depressing, scary
(for dramatic): flat, boring, mundane, generic
(for professional): casual, amateur, snapshot
(for artistic): commercial, stock photo, generic
```

---

## Integration Negatives (Mixed Reality)

### When Combining Real + Generated Elements
```
obvious photoshop, poorly composited,
mismatched lighting, inconsistent shadows,
floating elements, no contact shadows,
edge artifacts, visible seams,
different resolution between elements,
color mismatch, perspective mismatch
```

---

## Building Your Negative Prompt

### Formula
```
[Universal quality issues] +
[Style-specific negatives] +
[Specific things to avoid for this image]
```

### Example for Superhero Scene
```
Negative prompt:
blurry, low resolution, distorted hands, watermark,
soft lighting, flat lighting, passport photo,
boring composition, stiff posture, plastic skin,
cartoon, anime, fake looking, awkward pose
```

### Example for Family Portrait
```
Negative prompt:
harsh shadows, high contrast, cold blue tones,
flash photography, stiff posed expressions,
fake smiles, busy background, over-saturated,
artificial looking, plastic skin
```

### Example for Miniature Scene
```
Negative prompt:
toy, plastic, diorama, miniature model,
no contact shadow, floating, tilt-shift effect,
cartoon, unrealistic scale, smooth plastic texture,
obviously fake, no interaction with environment
```

---

## Pro Tips

1. **Be specific** - "no harsh shadows" works better than just "bad lighting"
2. **Match style** - use negatives that address that style's common issues
3. **Don't overdo it** - too many negatives can confuse the AI
4. **Prioritize** - put the most important exclusions first
5. **Test and iterate** - see what works for your specific prompts
