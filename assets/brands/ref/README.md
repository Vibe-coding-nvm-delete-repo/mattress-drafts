# Nappedia Brand Vector Asset & Reference Registry

This directory contains verified reference records and vector design standards for all **63 mattress brands** active in Nappedia.

## Asset Directory Structure
- `assets/brands/svg/`: Standardized, production-ready vector `.svg` files for each brand.
- `assets/brands/ref/brand_reference_dossier.json`: Machine-readable master metadata for every brand (parent company, corporate HQ, founding year, website URL, brand colors).
- `assets/brands/brands_manifest.json`: Unified manifest with inline SVGs for runtime bundling.
- `preview_logos.html`: Standalone visual test harness for inspecting all 63 logos.

## Vector Standard Specifications
1. **ViewBox Aspect Ratio**: Default `viewBox="0 0 100 24"` (or `0 0 110 24` for elongated wordmarks).
2. **Typography & Geometry**: Uses system-accessible clean font stacks (`Segoe UI`, `Georgia`) combined with authentic brand geometric emblems, badges, and color tokens.
3. **Contrast & Theming**: Every mark is calibrated for readability against:
   - Light backgrounds (`#FAF7F0`, `#FFFFFF`)
   - Dark headers (`#16283E`, `#0F1C2C`)
4. **Zero External Dependencies**: Pure standalone SVGs with zero external font or stylesheet dependencies, preventing layout shift or network failure.

## Adding New Brands to the Registry
1. Add reference dossier record to `brand_reference_dossier.json`.
2. Author SVG with standardized `viewBox="0 0 100 24"` and save to `assets/brands/svg/<slug>.svg`.
3. Update `brands_manifest.json` and rebuild `preview_logos.html`.
