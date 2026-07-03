# Product Content Studio

Product Content Studio is a Codex skill that converts product documents, specifications, packaging photos, labels, and product images into structured product information, marketplace-ready copy, and faithful showcase-image plans or visuals.

## Install

Copy the `product-content-studio` folder into your Codex skills directory:

```bash
cp -R product-content-studio "${CODEX_HOME:-$HOME/.codex}/skills/"
```

Restart or reload Codex if the skill is not discovered immediately.

## Use

Invoke the skill explicitly in your prompt:

```text
Use $product-content-studio to extract the product information from these files, write a marketplace listing, and create a six-image showcase plan.
```

Attach any available product copy, specification sheets, PDFs, packaging images, label photos, and clean product images. For better results, also provide:

- Target marketplace or sales channel
- Output language and tone
- Target audience and positioning
- Required image count, dimensions, and aspect ratios
- Brand assets and visual rules
- Any facts that must not be changed

## Example Requests

```text
Use $product-content-studio to turn these package photos into a structured product record. Mark uncertain values and do not write marketing copy yet.
```

```text
Use $product-content-studio to create an English Amazon-style listing from this specification sheet. Do not invent certifications or performance claims.
```

```text
Use $product-content-studio to plan and generate four 1:1 showcase images from these product photos. Preserve the exact shape, color, logo, controls, and included accessories.
```

## Outputs

Depending on the request, the skill can produce:

- A source-traceable product record
- Product positioning, audience, and use cases
- Supported selling points and listing copy
- Specifications, package contents, instructions, and cautions
- A showcase-image shot list and production-ready prompts
- Generated or edited showcase images when an image tool is available
- A list of conflicts, missing information, assumptions, and compliance risks

## Accuracy Model

Extracted values are labeled as `confirmed`, `inferred`, `conflicting`, or `missing`. The skill avoids presenting visual guesses as facts and requires generated images to preserve the product's real geometry, branding, color, parts, variant, and package contents.

## License

No license has been granted by default. Add the license that matches your intended distribution before accepting external contributions or reuse.
