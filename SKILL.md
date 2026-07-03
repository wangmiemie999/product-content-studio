---
name: product-content-studio
description: Extract reliable product facts from product copy, specification sheets, PDFs, documents, packaging photos, labels, and product images; normalize the information into a structured product record; write channel-appropriate listing copy; and plan or generate faithful product showcase images. Use when Codex needs to turn incomplete or mixed product source material into product information, e-commerce listings, selling points, image briefs, image-generation prompts, or finished showcase visuals while preserving factual and visual accuracy.
---

# Product Content Studio

Turn mixed product source material into a traceable product record, usable sales copy, and visually faithful showcase-image deliverables.

## Workflow

1. Inspect every supplied text, file, and image before drafting.
2. Determine whether the material covers one product, multiple variants, or multiple products. Keep variants separate.
3. Extract facts into the schema in `references/product-schema.md`.
4. Label each value as `confirmed`, `inferred`, `conflicting`, or `missing`. Record its source. Never present an inference as a fact.
5. Normalize units, terminology, variants, repeated fields, and packaging information. Preserve original values when conversion could be ambiguous.
6. Resolve duplicates. Surface conflicting values and request clarification only when the conflict materially affects the deliverable.
7. Derive positioning, audience, use cases, benefits, and selling points only from supported facts.
8. Write the requested listing content for the target language and channel. If the channel is unspecified, create neutral marketplace copy.
9. Plan the image set before generating or editing images. Read `references/image-guidelines.md` for any visual work.
10. Use the available image-generation or image-editing capability when the user requests finished visuals. Use supplied product images as references whenever available.
11. Run the final consistency check and deliver the structured record, copy, image plan, prompts, generated files, and unresolved questions as applicable.

## Source Handling

- Treat printed labels, specification sheets, and explicit user statements as evidence, not automatically as mutually consistent truth.
- Use OCR or visual inspection for labels and packaging. Preserve uncertain characters with an uncertainty marker.
- Do not infer hidden dimensions, materials, certifications, ingredients, compatibility, performance, or package contents from appearance alone.
- Separate the product from props, background objects, reflections, and optional accessories.
- Prefer omission over invention. Ask a concise question when a missing value is essential.
- Keep claims traceable to a source location such as filename, page, table, image, label region, or user statement.

## Copy Requirements

Read `references/copy-and-compliance.md` before producing regulated, health-related, beauty, food, children's, electrical, or safety claims.

- Separate factual features from customer benefits and promotional language.
- Use concrete, scannable language and preserve important limitations.
- Do not invent awards, rankings, sales volume, endorsements, patents, certifications, guarantees, comparisons, or test results.
- Do not use absolute claims unless the source explicitly supports them and the target channel permits them.
- Do not convert an observed visual characteristic into an unsupported material or performance claim.
- Adapt title length, tone, keywords, and field order when the user names a platform. State assumptions when exact platform rules are unavailable.

## Visual Requirements

- Preserve product geometry, proportions, color, texture, controls, ports, labels, logos, package count, and included accessories.
- Do not add functions, components, variants, claims, or packaging contents that are not supported by the source material.
- Prefer image editing or reference-conditioned generation when an original product image is available.
- Generate environments, lighting, props, and people only when they do not misrepresent scale, use, safety, or included items.
- Keep critical text, prices, dimensions, and specifications out of generative image pixels when accurate typography matters; supply them as a layout layer or image brief instead.
- Inspect every generated image for deformations, duplicated or missing parts, incorrect branding, inconsistent variants, implausible use, and misleading scale. Regenerate or disclose limitations when defects remain.

## Output

Follow `assets/output-template.md` unless the user requests another format. Return only sections relevant to the request.

Include, when applicable:

- Structured product record with source and confidence status
- One-sentence positioning statement
- Target audience and use cases
- Three to six supported selling points
- Listing title, subtitle, description, specifications, package contents, instructions, cautions, and keywords
- Image-set plan with purpose, composition, displayed claim, aspect ratio, and generation/editing method
- Production-ready image prompts that identify immutable product details and prohibited changes
- Finished visual files when requested and supported by available tools
- Conflicts, missing information, assumptions, and compliance risks

For machine-readable output, use the same field names from `references/product-schema.md` and valid JSON. Do not place commentary inside JSON.

## Final Quality Check

Before delivery, verify that:

1. Every factual claim is supported by source material.
2. Facts, inferences, conflicts, and missing values are clearly separated.
3. Product variants and package contents have not been mixed.
4. Units and values are internally consistent.
5. Copy, specifications, image text, and visuals agree.
6. Generated visuals preserve the real product and do not imply unsupported features or scale.
7. Regulated or sensitive claims are either supported and appropriately qualified or omitted.
8. The output matches the requested language, channel, dimensions, file format, and image count.

## References

- Read `references/product-schema.md` for extraction fields and confidence labels.
- Read `references/image-guidelines.md` whenever planning, generating, or editing visuals.
- Read `references/copy-and-compliance.md` for claim writing and sensitive categories.
- Use `assets/output-template.md` as the default human-readable deliverable structure.
