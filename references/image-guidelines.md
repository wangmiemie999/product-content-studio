# Product Showcase Image Guidelines

## Plan Each Image

Specify purpose, subject, immutable product details, composition, camera angle, setting, lighting, props, people, displayed selling point, text treatment, aspect ratio, resolution, and output format.

## Common Image Types

- Clean-background hero image
- Front, side, rear, and three-quarter views
- Material or construction detail
- Feature demonstration
- Scale or dimension explanation
- In-use lifestyle scene
- Package contents layout
- Variant comparison
- Social-media editorial image

## Fidelity Rules

List immutable visual details directly in each prompt. Add an explicit negative constraint covering incorrect logos, altered geometry, extra ports, missing controls, duplicated parts, invented accessories, distorted text, wrong colors, and misleading scale.

When reference coverage is incomplete, avoid inventing unseen sides. Choose a supported angle or mark the result as conceptual.

## Prompt Pattern

```text
Create/edit a [image type] for [product and variant]. Preserve exactly: [immutable details]. Show [composition and use]. Use [background, lighting, lens, mood]. Communicate [supported selling point] without adding text unless requested. Output [ratio and size]. Do not change [negative constraints].
```

## Review

Compare the result against every reference image. Check geometry, component count, branding, color, surface, variant, accessories, interaction, scale, shadows, reflections, anatomy, and legibility. Reject materially inaccurate results.
