# Product Information Schema

## Status Labels

- `confirmed`: Explicitly supported by a readable source.
- `inferred`: Plausible from context or appearance but not explicitly confirmed.
- `conflicting`: Two or more sources disagree.
- `missing`: Required or useful information is unavailable.

For every important field, retain `value`, `status`, `source`, and optional `note`.

## Core Fields

- identity: product_name, brand, model, sku, category, variant
- physical: color, material, finish, dimensions, weight, capacity
- functional: functions, features, controls, compatibility, performance
- commercial: package_contents, quantity, warranty, country_of_origin
- regulated: ingredients, allergens, certifications, warnings, expiry, age_limit
- usage: intended_use, target_users, use_cases, instructions, care, storage
- visual: shape, visible_components, logo_location, label_text, packaging, reference_images
- positioning: audience, primary_benefit, supported_selling_points, differentiators

## JSON Shape

```json
{
  "identity": {
    "product_name": {
      "value": "",
      "status": "confirmed",
      "source": "",
      "note": ""
    }
  },
  "physical": {},
  "functional": {},
  "commercial": {},
  "regulated": {},
  "usage": {},
  "visual": {},
  "positioning": {},
  "conflicts": [],
  "missing_information": []
}
```

Include only relevant fields, but never remove source and status from consequential facts.
